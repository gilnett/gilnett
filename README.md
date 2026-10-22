<div align="center">

# Gilnett

<a href="https://github.com/gilnett">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Low-Latency+Systems+Engineering+in+Rust;Windows+Internals+%26+Windhawk+Mod+Author;Author+of+wstrace+%26+learned_index_lab;Zero-Drop+ETW+%26+Win32+Hooking" alt="Typing SVG" />
</a>

<p align="center">
  <img src="https://img.shields.io/badge/Rust-CE412B?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <a href="https://windhawk.net"><img src="https://img.shields.io/badge/Windhawk-Mod_Author-d29922?style=flat-square&logo=cplusplus&logoColor=white" alt="Windhawk" /></a>
  <a href="https://ko-fi.com/gilnet"><img src="https://img.shields.io/badge/Support-Ko--fi-FF5E5B?style=flat-square&logo=kofi&logoColor=white" alt="Ko-fi" /></a>
</p>

</div>

---

### Core Engineering Focus

<!-- OPTION 1: TABLE -->
#### Option 1: Structured Table
| Project | Domain | Tech Stack | Architecture & Role |
| :--- | :--- | :--- | :--- |
| **[wstrace](https://github.com/gilnett/wstrace)** | Windows Kernel Tracing | `Rust` `ETW` `Win32` | Zero-drop microsecond event capture, lock-free ring buffer & TUI |
| **[learned_index_lab](https://github.com/gilnett/learned_index_lab)** | Learned Index Structures | `Rust` `PGM` `Eytzinger` | Mathematical CDF approximation replacing B-Trees in LSM/OLAP |
| **[Windhawk Mods](https://windhawk.net)** | Windows Internals & Tuning | `C++` `Win32 Hooking` | Thread-safe OS injection, priority scheduling & memory trimming |

<!-- OPTION 2: COMPACT MERMAID -->
#### Option 2: Compact Graph
```mermaid
graph LR
    subgraph S1[" "]
        ETW["Windows ETW"] -->|Zero-drop| W["wstrace"]
        RAM["Cache Hierarchy"] -->|CDF PLA| P["learned_index_lab"]
        WIN["Win32 Hooking"] -->|Injection| M["Windhawk Mods"]
    end

    W --> TUI["Interactive TUI"]
    P --> DB["LSM / OLAP Engines"]
    M --> OS["Shell & OS Tuning"]

    style S1 fill:none,stroke:none
    style W fill:#161b22,stroke:#58a6ff,stroke-width:2px,color:#fff
    style P fill:#161b22,stroke:#3fb950,stroke-width:2px,color:#fff
    style M fill:#161b22,stroke:#d29922,stroke-width:2px,color:#fff
    style ETW fill:#0d1117,stroke:#30363d,color:#8b949e
    style RAM fill:#0d1117,stroke:#30363d,color:#8b949e
    style WIN fill:#0d1117,stroke:#30363d,color:#8b949e
    style TUI fill:#0d1117,stroke:#30363d,color:#8b949e
    style DB fill:#0d1117,stroke:#30363d,color:#8b949e
    style OS fill:#0d1117,stroke:#30363d,color:#8b949e
```

<!-- OPTION 3: VISUAL CARDS -->
#### Option 3: Visual Cards
<table align="center" width="100%">
  <tr>
    <td width="33%" align="center" valign="top">
      <h3><a href="https://github.com/gilnett/wstrace">wstrace</a></h3>
      <p><code>Rust</code> · <code>ETW</code> · <code>Kernel</code></p>
      <p><b>Low-latency tracing</b><br/>Zero-drop syscall & API monitor via lock-free ring buffers.</p>
    </td>
    <td width="33%" align="center" valign="top">
      <h3><a href="https://github.com/gilnett/learned_index_lab">learned_index_lab</a></h3>
      <p><code>Rust</code> · <code>PGM</code> · <code>Math</code></p>
      <p><b>Learned Indexes</b><br/>Mathematical CDF regressions outperforming B-Trees in CPU cache.</p>
    </td>
    <td width="33%" align="center" valign="top">
      <h3><a href="https://windhawk.net">Windhawk Mods</a></h3>
      <p><code>C++</code> · <code>Win32</code> · <code>Hooks</code></p>
      <p><b>OS Internals Tuning</b><br/>Thread-safe hooking, dynamic priority scheduling & RAM trimming.</p>
    </td>
  </tr>
</table>

---

### Windows Internals & Windhawk Mods (C++ / Win32 Hooking)

Author of production mods for the [Windhawk](https://windhawk.net/) platform, focusing on low-level Win32 hooks, memory safety, and thread-safe OS tuning:

#### Published Mods:
- **[Smart Process Priority & RAM Optimizer](https://windhawk.net/mods/smart-process-priority-ram-optimizer)**: Dynamic working-set memory trimming, background CPU throttling, and intelligent priority scheduling.
- **[Taskbar Volume Percentage Indicator](https://windhawk.net/mods/taskbar-volume-percentage)**: Replaces the Windows 11 system tray volume icon with real-time master volume level percentage.
- **[Hide Taskbar Tooltips](https://windhawk.net/mods/hide-taskbar-tooltips)**: Suppresses native Windows 11 XAML hover tooltips in Explorer, with selective area filtering for taskbar apps and tray icons.

#### Upcoming Mods:
- `[Coming Soon]` **Quick Search for Windows / Explorer Search Everything**: Low-latency search injection hooking directly into Windows Explorer and the Everything search engine.

---

### Activity & Performance Metrics

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=gilnett&theme=github-dark&hide_border=true&area=true" width="100%" alt="Activity Graph" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=gilnett&show_icons=true&theme=github_dark&hide_border=true&count_private=true&cache_seconds=1800" width="48%" alt="GitHub Stats" />
  <img src="language-distribution.svg" width="48%" alt="Language Distribution" />
</p>
