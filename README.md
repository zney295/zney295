<div align="center">

# <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=25&duration=3200&pause=1000&color=00F0FF&center=true&vCenter=true&width=820&lines=SYSTEM.BOOT(ZNEY)+%E2%80%94+Systems+%26+Full-Stack+Engineer;Architecting+Low-Level+Rust+Engines+%26+AI+MCP+Sandboxes;Crafting+Immersive+3D+WebGL+%2F+Three.js+Experiences;Information+Technology+%40+University+of+Economics+HCMC+(UEH)" alt="Typing SVG Banner" />

<p>
  <a href="https://zney295.id.vn/"><img src="https://img.shields.io/badge/Portfolio-00D4E8?style=for-the-badge&amp;logo=googlechrome&amp;logoColor=0D1117" alt="Visit 3D portfolio" /></a>
  <a href="https://github.com/zney295/resc"><img src="https://img.shields.io/badge/resc_%E2%86%97-Rust_%C2%B7_MCP-CE7148?style=for-the-badge&amp;logo=rust&amp;logoColor=white" alt="resc — Rust forensics MCP" /></a>
  <a href="mailto:lequangkhanh295@gmail.com"><img src="https://img.shields.io/badge/Email-30363D?style=for-the-badge&amp;logo=gmail&amp;logoColor=white" alt="Email Le Quang Khanh" /></a>
  <a href="https://www.facebook.com/psyotic.zney/"><img src="https://img.shields.io/badge/Facebook-30363D?style=for-the-badge&amp;logo=facebook&amp;logoColor=white" alt="Facebook" /></a>
</p>

<img src="./assets/terminal.svg" width="720" alt="$ building Rust engines / crafting 3D web experiences / learning at UEH" />

</div>

<div align="center">

<img src="./assets/profile.svg" width="920" alt="Zney — Systems &amp; full-stack engineering. Rust, SIMD, MCP, Three.js, React, TypeScript, .NET. IT student at UEH, Ho Chi Minh City." />

[Portfolio ↗](https://zney295.id.vn/) &nbsp; · &nbsp; [resc engine ↗](https://github.com/zney295/resc)

</div>

---

## ⚡ Executive Summary & Engineering Philosophy

<table>
<tr>
<td width="55%" valign="top">

### 👨‍💻 Who I Am
I am an **Information Technology Engineer** in training at the **University of Economics Ho Chi Minh City (UEH)** with a deep focus on bridging two worlds that rarely meet:
* **Low-Level Systems & Defensive Engineering:** Building memory-safe **Rust** engines, direct DMA/unbuffered hardware I/O layers, **SIMD (AVX2)** scanners, and zero-copy binary parsers.
* **Interactive 3D & Full-Stack Web:** Designing real-time collaborative applications (`WebRTC`, `WebSockets`), spatial **Three.js / WebGL** interfaces, and scalable backend services (`C# / .NET`, `Node.js`, `PostgreSQL`).

> *"Whether it is rendering 60FPS shaders on a browser canvas or parsing corrupted NTFS `$MFT` sectors in a RAM overlay, great engineering is about **precision, safety boundaries, and zero wasted cycles**."*

</td>
<td width="45%" valign="top">

### 🎯 Current Technical Focus
```yaml
name: Le Quang Khanh (Zney)
role: Systems & Full-Stack Engineer
institution: UEH University (HCMC)

active_research:
  - AI Agent Sandboxing via MCP (JSON-RPC)
  - In-Memory Copy-on-Write (CoW) Disk Overlays
  - 3D Web Graphics & Spatial UI (Three.js)
  - Windows System Daemons & Security (C#/Rust)

core_principles:
  - "100% Read-Only Hardware Safety"
  - "Zero-Copy & Token-Efficient Telemetry"
  - "Fuzz-Tested Defensive Parsing"
```

</td>
</tr>
</table>

---

## 🛡️ Flagship Systems Spotlight: [`resc`](https://github.com/zney295/resc)

<div align="center">
<table>
<tr>
<td width="100%">

### 🛡️ **resc** — Low-Level Disk Forensics & Data Recovery MCP Engine in Rust
*An AI-driven digital forensics sandbox that allows LLMs (Claude, Cursor, Gemini) to diagnose damaged drives, repair partition tables/boot sectors in RAM, and salvage data—without ever writing a single byte to physical hardware.*

<p align="center">
  <img src="https://img.shields.io/badge/Language-Rust_2021-orange?style=flat-square&logo=rust" />
  <img src="https://img.shields.io/badge/Protocol-MCP_(stdio_JSON--RPC)-00F0FF?style=flat-square" />
  <img src="https://img.shields.io/badge/Parser_Fuzzing-1,000,000+_Inputs_Passed-brightgreen?style=flat-square" />
  <img src="https://img.shields.io/badge/Physical_I/O-4KB_Aligned_Overlapped_DMA-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/Safety-In--Memory_CoW_Overlay_+_WAL-success?style=flat-square" />
</p>

**Key Architectural Highlights:**
- **🧠 Hybrid "Brain & Muscle" Design:** Offloads multi-gigabyte raw sector scanning (`AVX2 SIMD`), Shannon entropy calculation ($0.0 - 8.0\text{ bits/byte}$), and zero-copy struct casting (`MBR`, `GPT`, `NTFS`, `FAT32`) to Rust, while sending `< 5KB` JSON anomaly maps to the AI Agent.
- **🔒 Hardware-Level Write Blocking & RAM Overlay:** Physical drives are opened strictly `GENERIC_READ` with `FILE_FLAG_OVERLAPPED` + `CancelIoEx` kernel watchdogs[cite: 2]. AI hex patches are applied to a `BTreeMap` in-memory Copy-on-Write overlay backed by a persistent Write-Ahead Log (`.wal`) and verified via native filesystem traversal before extraction[cite: 2].
- **📑 Forensic Chain-of-Custody:** Asynchronous non-blocking extraction with `O_NOFOLLOW` / `FILE_FLAG_OPEN_REPARSE_POINT` handle verification (TOCTOU protection), atomic `.part` clone/mapfile commits, and automated SHA-256 `.manifest.json` audit generation[cite: 2].

<p align="right">
  <a href="https://github.com/zney295/resc"><b>Explore the Architecture & Source Code →</b></a>
</p>

</td>
</tr>
</table>
</div>

---

## 🌟 Featured Engineering Portfolio

<div align="center">
<table>
<tr>
<td width="50%" valign="top">

### 🌌 [3D Cyberpunk Creator Portfolio](https://github.com/zney295/zney295.github.io)
**Interactive Spatial Web Experience**
- Custom 3D desktop workspace rendered in real-time with **Three.js / WebGL** & **React 18**.
- Features physics-based mechanical keyboard audio/visual simulation, custom shaders, and smooth camera transitions.
- **Tech:** `React 18` `TypeScript` `Three.js` `Tailwind CSS` `Vite`
- 🔗 **[Live Experience](https://zney295.id.vn/)** • **[GitHub Repo](https://github.com/zney295/zney295.github.io)**

</td>
<td width="50%" valign="top">

### 🎧 [BeatSync](https://github.com/zney295/beatsync)
**Real-Time Collaborative Audio Platform**
- Low-latency synchronized music listening rooms built on **WebRTC** data/audio channels and **WebSockets**.
- Sub-millisecond playback drift compensation and distributed room state synchronization.
- **Tech:** `TypeScript` `WebRTC` `WebSockets` `Node.js`
- 🔗 **[GitHub Repo](https://github.com/zney295/beatsync)**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 [Windows Security & Cloud Relay](https://github.com/zney295/Security)
**Proactive System Monitoring Daemon**
- Background Windows Service engineered in **C# / .NET** and **PowerShell** for hardware-level telemetry and anti-theft tracking.
- Evaluates virtualization-based security readiness and streams encrypted heartbeats through a cloud relay.
- **Tech:** `C#` `.NET` `Windows Services` `PowerShell`
- 🔗 **[GitHub Repo](https://github.com/zney295/Security)**

</td>
<td width="50%" valign="top">

### 🧠 [AI Heuristic TSP Solver](https://github.com/zney295/AI_Hill_Climbing_TSP) & [LearningEnglish](https://github.com/zney295/LearningEnglish)
**Algorithmic Optimization & NLP Parsing**
- **TSP Solver:** Heuristic Hill-Climbing search optimization solving complex routing graphs.
- **LearningEnglish:** Automated grammatical tense verification and syntactic structure parser.
- **Tech:** `Algorithms` `NLP` `Full-Stack Web`
- 🔗 **[TSP Repo](https://github.com/zney295/AI_Hill_Climbing_TSP)** • **[NLP App Repo](https://github.com/zney295/LearningEnglish)**

</td>
</tr>
</table>
</div>

---

## 🛠️ Technical Arsenal & Ecosystem

<div align="center">

[![Skill Icons](https://skillicons.dev/icons?i=rust,cs,dotnet,ts,js,react,threejs,tailwind,nodejs,express,flutter,dart,postgres,mysql,docker,linux,git,github,powershell,vscode&perline=10)](https://skillicons.dev)

</div>

<br />

<div align="center">

| Domain | Core Competencies & Production Tooling |
| :--- | :--- |
| **⚙️ Systems & Forensics** | ![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white) ![Tokio](https://img.shields.io/badge/Tokio_Async-383838?style=flat-square) ![SIMD](https://img.shields.io/badge/AVX2_SIMD-FF5733?style=flat-square) ![MCP](https://img.shields.io/badge/MCP_JSON--RPC-00F0FF?style=flat-square&logoColor=black) ![Win32](https://img.shields.io/badge/Win32_Kernel_I/O-0078D6?style=flat-square&logo=windows) |
| **🎨 Frontend & 3D Graphics** | ![React](https://img.shields.io/badge/React_18-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Three.js](https://img.shields.io/badge/Three.js_/_WebGL-000000?style=flat-square&logo=three.js&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) ![Flutter](https://img.shields.io/badge/Flutter_&_Dart-02569B?style=flat-square&logo=flutter&logoColor=white) |
| **🚀 Backend & Distributed** | ![C#](https://img.shields.io/badge/C%23_/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) ![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black) |
| **🗄️ Data & Infrastructure** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![SQL Server](https://img.shields.io/badge/MS_SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |

</div>

<details>
<summary><b>🔍 Click to expand: Deep-Dive into My Engineering Workflow & Environments</b></summary>
<br />

- **Systems & Virtualization Lab:** Experienced in configuring multi-OS virtualization environments (`VMware Workstation`, `WSL 2`, `Docker Containers`, `Linux / Pop!_OS`) and low-level hardware debugging.
- **Database Architecture & Process Mining:** Skilled in complex relational schema design, stored procedures, set operations in `SQL Server (SSMS)` / `PostgreSQL`, and transforming raw interaction logs into event pipelines for `Celonis Process Mining`.
- **AI-Native Engineering:** Designing structured `.agents/skills/` playbooks, decision trees, and deterministic tool schemas to turn LLMs into reliable systems co-pilots[cite: 2].

</details>

---

## 📊 GitHub Telemetry & Contribution Analytics

<div align="center">

<!-- DÒNG 1: STATS & STREAK CÂN XỨNG -->
<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=zney295&amp;theme=tokyonight" height="200" alt="GitHub statistics for zney295" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=zney295&theme=tokyonight&hide_border=true&background=1a1b27&ring=00F0FF&fire=FF5733&currStreakLabel=00F0FF" height="165" alt="GitHub Streak" />
</p>

<!-- Top languages ranked by repository count. -->
<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=zney295&amp;theme=tokyonight" height="200" alt="Top languages by repository count for zney295" />
</p>

<!-- DÒNG 3: NẾU VẪN MUỐN DÙNG GRAPH, DÙNG THÊM CỜ CACHE_SECONDS ĐỂ GIẢM LỖI -->
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=zney295&theme=tokyo-night&hide_border=true&bg_color=1a1b27&color=00F0FF&line=00F0FF&point=FF5733&area=true&area_color=00F0FF" width="96%" alt="Activity Graph" />
</p>

</div>
---

## 📫 Connect & Collaborate

<div align="center">

I am always open to discussing **Systems Programming (Rust/C#)**, **AI Agent Infrastructure (MCP)**, **Interactive 3D Web Projects**, or **Software Engineering Opportunities**.

| Platform | Handle / Endpoint | Action |
| :---: | :---: | :---: |
| **🌐 3D Web Portfolio** | `zney295.id.vn` | **[Launch Interactive Portfolio ↗](https://zney295.id.vn/)** |
| **🛡️ Flagship Project** | `github.com/zney295/resc` | **[Explore `resc` Forensics Engine ↗](https://github.com/zney295/resc)** |
| **📫 Direct Email** | `lequangkhanh295@gmail.com` | **[Send an Email ↗](mailto:lequangkhanh295@gmail.com)** |
| **💬 Facebook** | `fb.com/psyotic.zney` | **[Connect on Facebook ↗](https://www.facebook.com/psyotic.zney/)** |

<br />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00F0FF,100:512BD4&height=100&section=footer&text=Engineered%20with%20Precision%20by%20Zney&fontSize=18&fontColor=ffffff&fontAlignY=65" width="100%" alt="Footer Banner" />

</div>
