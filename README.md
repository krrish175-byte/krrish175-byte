<div align="center">

<!-- ANIMATED HEADER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Krrish%20Biswas&fontSize=52&fontColor=fff&animation=fadeIn&fontAlignY=38&desc=Open-Source%20Engineer%20%7C%20GSoC%202026%20%7C%20LFX%202026&descAlignY=60&descAlign=50" width="100%"/>

<!-- TYPING ANIMATION -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1000&color=00D084&center=true&vCenter=true&width=700&lines=60%2B+PRs+merged+across+15%2B+organizations;GSoC+2026+%E2%80%94+FOSSology+%2F+Linux+Foundation;LFX+2026+%E2%80%94+OpenSSF+%2F+Minder;mindersec+org+member+%E2%80%94+nominated+by+maintainer;I+build+things+that+make+devs%27+lives+easier" alt="Typing SVG" />
</a>

<br/>

<!-- PROFILE BADGES -->
[![Profile Views](https://komarev.com/ghpvc/?username=krrish175-byte&style=for-the-badge&color=00d084&label=PROFILE+VIEWS)](https://github.com/krrish175-byte)
[![GitHub followers](https://img.shields.io/github/followers/krrish175-byte?style=for-the-badge&color=00d084&labelColor=0a0a0a&label=FOLLOWERS)](https://github.com/krrish175-byte?tab=followers)
[![GitHub Stars](https://img.shields.io/github/stars/krrish175-byte?style=for-the-badge&color=00d084&labelColor=0a0a0a&label=TOTAL+STARS)](https://github.com/krrish175-byte)

</div>

---

<!-- ABOUT -->
## About Me

```go
package main

import "fmt"

type Engineer struct {
    Name        string
    Location    string
    CurrentWork []string
    Mentorships []string
    PRsMerged   string
    Orgs        string
    Since       string
}

func main() {
    krrish := Engineer{
        Name:     "Krrish Biswas",
        Location: "Bengaluru, India 🇮🇳",
        CurrentWork: []string{
            "LFX 2026 @ OpenSSF - Building Minder rule testing framework",
            "GSoC 2026 @ FOSSology - CycloneDX Spec 1.7 upgrade",
        },
        Mentorships: []string{
            "✓ LFX Mentorship 2026 - OpenSSF / Minder",
            "✓ Google Summer of Code 2026 - FOSSology / Linux Foundation",
        },
        PRsMerged: "60+",
        Orgs:      "15+",
        Since:     "December 2024",
    }
    fmt.Println("Selected for GSoC + LFX simultaneously - both in first year")
    fmt.Println("Nominated for mindersec org membership by OpenSSF maintainer")
    fmt.Printf("Contributed %s PRs to %s orgs since %s\n",
        krrish.PRsMerged, krrish.Orgs, krrish.Since)
}
```

---

<!-- MENTORSHIPS - MOST PROMINENT SECTION -->
## Mentorships & Fellowships

<div align="center">

| | Program | Organization | Year |
|---|---|---|---|
| <img src="https://img.shields.io/badge/LFX-2026-00d084?style=for-the-badge" /> | **Minder Rule Testing & CI Tooling** | OpenSSF / mindersec | Summer 2026 |
| <img src="https://img.shields.io/badge/GSoC-2026-4285F4?style=for-the-badge&logo=google" /> | **CycloneDX Spec 1.7 Upgrade** | FOSSology / Linux Foundation | Summer 2026 |

</div>

### LFX 2026 — OpenSSF / Minder
> *Building the testing infrastructure that makes Minder's security policy rules verifiable.*

-  Building `minder ruletype test` — a standalone CLI for **hermetic, offline rule evaluation** (no live GitHub token needed)
-  Implemented a custom `http.RoundTripper` mock layer intercepting **REST v3 and GraphQL v4** at the HTTP boundary
-  CI pipeline for `minder-rules-and-profiles` auto-discovering `*.test.yaml` files and running **parallel matrix jobs** on every PR
-  **Nominated for mindersec GitHub org membership** by mentor Evan Anderson (ex-Google SRE, 15 years) for contributions made *before* the mentorship started

`Go` `Rego/OPA` `Shell` `GitHub Actions` `gRPC` `OPA`

---

###  GSoC 2026 — FOSSology / Linux Foundation
> *Upgrading software supply chain tooling used by enterprises worldwide.*

-  Upgrading FOSSology's CycloneDX agent from **spec 1.4 → 1.7**
-  Adding formal **evidence layer** separating scanner findings from human clearing decisions
-  Implementing CycloneDX import support + **full PHPUnit test coverage**
-  Selected from **thousands of global applicants** — small-size 90hr project, high impact

`PHP` `JSON` `XML` `PHPUnit` `Docker` `REST API` `SBOM` `CycloneDX`

---

<!-- OPEN SOURCE STATS -->
## GitHub Analytics

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=krrish175-byte&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&hide_border=true&bg_color=0a0a0a&title_color=00d084&icon_color=00d084&text_color=f0f0f0"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=krrish175-byte&layout=compact&langs_count=8&theme=github_dark&hide_border=true&bg_color=0a0a0a&title_color=00d084&text_color=f0f0f0"/>
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=krrish175-byte&theme=github-dark-blue&hide_border=true&background=0a0a0a&stroke=00d084&ring=00d084&fire=00d084&currStreakLabel=00d084" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=krrish175-byte&bg_color=0a0a0a&color=00d084&line=00d084&point=ffffff&area=true&hide_border=true" width="100%"/>
</div>

---

<!-- CONTRIBUTIONS -->
## Open Source Contributions

> **60+ pull requests merged across 15+ organizations since December 2024**

<details>
<summary><b> mindersec/minder (Go)</b> — Security Policy Enforcement Platform</summary>

- GitHub API rate-limit handling with structured metrics
- Generalized OIDC authentication - removed Keycloak hard dependency
- Refactored PR actions for multi-VCS support (GitHub + GitLab)
- Fixed flaky `TestGrpcConnection` CI test using `bufconn` in-memory gRPC listener (eliminated real TCP port race condition)

</details>

<details>
<summary><b> fossology/fossology (PHP)</b> - License Compliance & SBOM</summary>

- SPDX3 API support
- License compliance workflow improvements
- Memory optimization for large-scale scans
- UI navigation and documentation enhancements

</details>

<details>
<summary><b> llm4s (Scala)</b> - LLM Infrastructure</summary>

- Composable middleware pipeline (logging, rate limiting, metrics)
- Semantic caching + vector similarity search
- Multimodal support (image/audio/video)
- OpenTelemetry tracing integration

</details>

<details>
<summary><b> scalameta/metals (Scala)</b> - Scala Language Server</summary>

- Memory leaks resolved via bounded caching
- LSP spec violations fixed (signature help, diagnostics)
- Worksheet recompilation and environment handling improvements

</details>

<details>
<summary><b> kubeedge/ianvs (Python)</b> - Edge AI Benchmarking</summary>

- Parallel execution architecture - **5-6× speedup**
- Dataset/config issue fixes
- Speculative decoding and cloud-edge LLM routing

</details>

<details>
<summary><b> Others - RISC-V DB · Scala 3 · Bloop · SW360</b></summary>

Compiler fixes, distributed tracing, API enhancements, and documentation across the broader open-source ecosystem.

</details>

---

<!-- PROJECTS -->
## Featured Projects

<div align="center">

[![flake-report](https://github-readme-stats.vercel.app/api/pin/?username=krrish175-byte&repo=flake-report&theme=github_dark&hide_border=true&bg_color=0a0a0a&title_color=00d084&icon_color=00d084&text_color=f0f0f0)](https://github.com/krrish175-byte/flake-report)
[![ai-slop-guardian](https://github-readme-stats.vercel.app/api/pin/?username=krrish175-byte&repo=ai-slop-guardian&theme=github_dark&hide_border=true&bg_color=0a0a0a&title_color=00d084&icon_color=00d084&text_color=f0f0f0)](https://github.com/krrish175-byte/ai-slop-guardian)

</div>

### flake-report
> Built at the request of an OpenSSF maintainer after identifying CI flakiness in mindersec/minder

Go CLI that parses JUnit XML from GitHub Actions artifacts and generates an interactive HTML report ranking flaky tests by **recency-weighted exponential decay**: `Σ(failures × 0.6^run_index)`. Zero external dependencies.

### AI Slop Guardian
> Because open source deserves better signal-to-noise

GitHub App that automatically detects and labels AI-generated content in PRs, issues, and comments — helping maintainers enforce human-review quality standards across their repositories.

### AgriLens — Crop Disease Detection
> Smart India Hackathon Finalist — 50,000+ teams

AI-driven mobile platform for real-time crop disease detection and nutrient deficiency analysis using TensorFlow/Keras and OpenCV. Built as a mobile-first experience with React Native.

---

<!-- TECH STACK -->
## Tech Stack

**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Scala](https://img.shields.io/badge/Scala-DC322F?style=for-the-badge&logo=scala&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)

**Security & OSS**

![OPA](https://img.shields.io/badge/OPA%2FRego-7D3C98?style=for-the-badge)
![CycloneDX](https://img.shields.io/badge/CycloneDX-00ADEF?style=for-the-badge)
![SPDX](https://img.shields.io/badge/SPDX-0066CC?style=for-the-badge)
![GitHub Apps](https://img.shields.io/badge/GitHub%20Apps-181717?style=for-the-badge&logo=github&logoColor=white)

**Infra & CI**

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**AI / ML**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)

---

<!-- TROPHIES -->
## GitHub Trophies

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=krrish175-byte&theme=darkhub&no-frame=true&no-bg=true&margin-w=6&column=6" />
</div>

---

<!-- CONNECT -->
## Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/krrish-biswas-797420380/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:krrishbiswas175@gmail.com)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=fadeIn" width="100%"/>

*"I started contributing to open source in December 2025. I haven't really stopped since."*

</div>
