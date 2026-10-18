<div align="center">

# Gilnett

<a href="https://github.com/gilnett">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Low-Latency+Systems+Engineering+in+Rust;Windows+Internals+%26+Windhawk+Mod+Author;Author+of+wstrace+%26+learned_index_lab;Zero-Drop+ETW+%26+Win32+Hooking" alt="Typing SVG" />
</a>

<p align="center">
  <img src="https://skillicons.dev/icons?i=rust,cpp,python&theme=dark" alt="Top 3 Languages: Rust, C++, Python" />
</p>

<p align="center">
  <a href="https://ko-fi.com/gilnet">Support on Ko-fi</a> &nbsp;|&nbsp; <a href="https://windhawk.net">Windhawk Mod Author</a>
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
| **Python** | Auditing & performance suites | Static code analysis, binary profiling, resource leak detection, automated benchmarks |
| **C# / .NET** | Windows Shell & UI mods | WinUI 3, XAML, Windows Explorer & Taskbar integrations |
| **PowerShell** | Tooling & package management | Windows deployment automation, WinGet / Scoop release automation |
| **TypeScript / JS** | Dashboards & web tooling | Real-time observability webviews, interactive dashboards |

---

### Activity & Performance Metrics

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=gilnett&theme=github-dark&hide_border=true&area=true" width="100%" alt="Activity Graph" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=gilnett&show_icons=true&theme=github_dark&hide_border=true&count_private=true" width="60%" alt="GitHub Stats" />
</p>

```mermaid
pie title Multi-Language Ecosystem Distribution
    "Rust" : 35
    "C++" : 25
    "Python" : 15
    "C#" : 10
    "PowerShell" : 8
    "TypeScript / JavaScript" : 7
```
