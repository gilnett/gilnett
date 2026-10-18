<div align="center">

# Gilnett

<a href="https://github.com/gilnett">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Low-Latency+Systems+Engineering+in+Rust;Author+of+wstrace+%26+learned_index_lab;Cache-Conscious+Architecture+%26+Zero-Drop+ETW" alt="Typing SVG" />
</a>

<p align="center">
  <a href="https://ko-fi.com/gilnet"><img src="https://img.shields.io/badge/Support-Ko--fi-FF5E5B?style=flat-square&logo=kofi&logoColor=white" alt="Ko-fi" /></a>
  <img src="https://img.shields.io/badge/Language-Rust_100%25-DEA584?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/OS-Windows_Kernel_%26_User--mode-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows" />
</p>

</div>

---

### Core Engineering Focus

```mermaid
graph LR
    subgraph "Hardware & Kernel Boundary"
        ETW["Windows ETW / Syscalls"] -->|Zero-drop lock-free| WSTRACE["<b>wstrace</b><br/><i>Microsecond Tracing</i>"]
        RAM["DRAM & Cache Hierarchy"] -->|CDF PLA Regressions| PGM["<b>learned_index_lab</b><br/><i>PGM Learned Index</i>"]
    end

    WSTRACE --> TUI["Interactive TUI & Stream"]
    PGM --> DB["LSM SSTables & OLAP Engines"]

    click WSTRACE "https://github.com/gilnett/wstrace" "Open wstrace repo"
    click PGM "https://github.com/gilnett/learned_index_lab" "Open learned_index_lab repo"

    style WSTRACE fill:#1f2430,stroke:#58a6ff,stroke-width:2px,color:#fff
    style PGM fill:#1f2430,stroke:#3fb950,stroke-width:2px,color:#fff
    style TUI fill:#161b22,stroke:#30363d,color:#8b949e
    style DB fill:#161b22,stroke:#30363d,color:#8b949e
    style ETW fill:#161b22,stroke:#30363d,color:#8b949e
    style RAM fill:#161b22,stroke:#30363d,color:#8b949e
```

---

### Featured Repositories

| Project | Description | Performance Highlights |
| :--- | :--- | :--- |
| **[wstrace](https://github.com/gilnett/wstrace)** | Zero-overhead ETW tracer & system profiler | Sub-microsecond latency, lock-free ring-buffer, interactive TUI |
| **[learned_index_lab](https://github.com/gilnett/learned_index_lab)** | PGM Learned Index structure in pure Rust | **4.45x faster** than BTreeMap, **99.97% less RAM**, zero-copy range queries |

---

### Activity & Performance Metrics

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=gilnett&theme=github-dark&hide_border=true&area=true" width="100%" alt="Activity Graph" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=gilnett&show_icons=true&theme=github_dark&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gilnett&layout=compact&theme=github_dark&hide_border=true" width="48%" alt="Top Languages" />
</p>

---

<details>
<summary><b>Detailed Benchmark Snapshot (learned_index_lab v0.2.0)</b></summary>
<br/>

| Structure | Hit Latency | Miss Latency | Index Memory (1M Keys) |
| :--- | :--- | :--- | :--- |
| `BTreeMap` | ~216 ns | ~61 ns | 45.78 MB |
| `slice::binary_search` | ~141 ns | ~40 ns | 0 KB (data resident) |
| **`PGM-Index`** | **~48 ns** | **~38 ns** | **12.1 KB (-99.97%)** |

</details>
