<div align="center">

# Gilnett

<a href="https://github.com/gilnett">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Low-Latency+Systems+Engineering+in+Rust;Windows+Internals+%26+Windhawk+Mod+Author;Author+of+wstrace+%26+learned_index_lab;Zero-Drop+ETW+%26+Win32+Hooking;High-Performance+C%2B%2B%2C+Rust%2C+C%23+%26+Python" alt="Typing SVG" />
</a>

<p align="center">
  <img src="https://img.shields.io/badge/Rust-CE412B?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white" alt="PowerShell" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Windows_Internals-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows" />
  <a href="https://windhawk.net"><img src="https://img.shields.io/badge/Windhawk-Mod_Author-d29922?style=flat-square&logo=cplusplus&logoColor=white" alt="Windhawk" /></a>
  <a href="https://ko-fi.com/gilnet"><img src="https://img.shields.io/badge/Support-Ko--fi-FF5E5B?style=flat-square&logo=kofi&logoColor=white" alt="Ko-fi" /></a>
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=rust,cpp,cs,python,powershell,ts,windows,git,github&theme=dark" alt="Skill Icons" />
</p>

</div>

---

### Core Engineering Focus

```mermaid
graph LR
    subgraph "Hardware & Kernel Boundary"
        ETW["Windows ETW / Syscalls"] -->|Zero-drop lock-free| WSTRACE["<b>wstrace</b><br/><i>Microsecond Tracing</i>"]
        RAM["DRAM & Cache Hierarchy"] -->|CDF PLA Regressions| PGM["<b>learned_index_lab</b><br/><i>PGM Learned Index</i>"]
        HOOK["Win32 / Shell Hooking"] -->|Low-overhead injection| WINDHAWK["<b>Windhawk Mods</b><br/><i>OS Customization & Optimization</i>"]
    end

    WSTRACE --> TUI["Interactive TUI & Stream"]
    PGM --> DB["LSM SSTables & OLAP Engines"]
    WINDHAWK --> SHELL["Taskbar & Explorer Shell Hooks"]

    click WSTRACE "https://github.com/gilnett/wstrace" "Open wstrace repo"
    click PGM "https://github.com/gilnett/learned_index_lab" "Open learned_index_lab repo"
    click WINDHAWK "https://windhawk.net" "Open Windhawk mods"

    style WSTRACE fill:#1f2430,stroke:#58a6ff,stroke-width:2px,color:#fff
    style PGM fill:#1f2430,stroke:#3fb950,stroke-width:2px,color:#fff
    style WINDHAWK fill:#1f2430,stroke:#d29922,stroke-width:2px,color:#fff
    style TUI fill:#161b22,stroke:#30363d,color:#8b949e
    style DB fill:#161b22,stroke:#30363d,color:#8b949e
    style SHELL fill:#161b22,stroke:#30363d,color:#8b949e
    style ETW fill:#161b22,stroke:#30363d,color:#8b949e
    style RAM fill:#161b22,stroke:#30363d,color:#8b949e
    style HOOK fill:#161b22,stroke:#30363d,color:#8b949e
```

---

### Featured Repositories

| Project | Description | Performance Highlights |
| :--- | :--- | :--- |
| **[wstrace](https://github.com/gilnett/wstrace)** | Zero-overhead ETW tracer & system profiler | Sub-microsecond latency, lock-free ring-buffer, interactive TUI |
| **[learned_index_lab](https://github.com/gilnett/learned_index_lab)** | PGM Learned Index structure in pure Rust | **4.45x faster** than BTreeMap, **99.97% less RAM**, zero-copy range queries |

---

### Windows Internals & Windhawk Mods (C++ / Win32 Hooking)

Author of production mods for the [Windhawk](https://windhawk.net/) platform, focusing on low-level Win32 hooks, memory safety, and thread-safe OS tuning:

#### Published Mods:
- **[Taskbar Volume Percentage Indicator](https://windhawk.net/mods/taskbar-volume-percentage)**: Replaces the Windows 11 system tray volume icon with real-time master volume level percentage.
- **[Hide Taskbar Tooltips](https://windhawk.net/mods/hide-taskbar-tooltips)**: Suppresses native Windows 11 XAML hover tooltips in Explorer, with selective area filtering for taskbar apps and tray icons.

#### Upcoming Mods:
- `[Coming Soon]` **Smart Process Priority & RAM Optimizer**: Dynamic working-set memory trimming, background CPU throttling, and intelligent priority scheduling.
- `[Coming Soon]` **Quick Search for Windows / Explorer Search Everything**: Low-latency search injection hooking directly into Windows Explorer and the Everything search engine.

---

### Technical Stack & Language Matrix

| Language / Domain | Primary Applications & Repositories | Key Frameworks & Technologies |
| :--- | :--- | :--- |
| **Rust** | [wstrace](https://github.com/gilnett/wstrace), [learned_index_lab](https://github.com/gilnett/learned_index_lab) | Kernel ETW tracing, PGM learned index algorithms, lock-free ring-buffers, ratatui TUI |
| **C++ (Win32)** | [Windhawk Mods](https://windhawk.net/mods/taskbar-volume-percentage) | Low-level Win32 API hooking, Explorer Shell extensions, thread scheduling, UI non-blocking |
| **C# / .NET** | Windows Shell & UI mods | WinUI 3, XAML, Windows Explorer & Taskbar integrations |
| **Python** | Auditing & performance suites | Static code analysis, binary profiling, resource leak detection, automated benchmarks |
| **PowerShell** | Tooling & package management | Windows deployment automation, WinGet / Scoop release automation |
| **TypeScript / JS** | Dashboards & web tooling | Real-time observability webviews, interactive dashboards |

---

### Activity & Performance Metrics

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=gilnett&theme=github-dark&hide_border=true&area=true" width="100%" alt="Activity Graph" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=gilnett&show_icons=true&theme=github_dark&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gilnett&layout=compact&theme=github_dark&hide_border=true&fork=true" width="48%" alt="Top Languages" />
</p>
