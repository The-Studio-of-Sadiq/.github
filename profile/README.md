<div align="center">

# The Studio of Sadiq

Open engineering software: structural analysis, debate tools, open textbooks and nuclear physics workbenches.

[thestudioofsadiq.tech](https://thestudioofsadiq.tech/) · [Project boards](https://github.com/orgs/The-Studio-of-Sadiq/projects)

</div>

The Studio of Sadiq builds free, open-source tools for engineering practice, research and teaching: desktop engineering workbenches, offline-first apps, browser front ends for established scientific codes, and open textbooks. Everything here is public; most projects are usable today, with their known gaps listed in each repo.

## The five projects

All work is organised into five public project boards.

| Project | What it is | Repos | Board |
| --- | --- | --- | --- |
| [SAEngine](#saengine) | Structural analysis and design, from soil report to design package | 6 | [#8](https://github.com/orgs/The-Studio-of-Sadiq/projects/8) |
| [Debate Operating System](#debate-operating-system) | SimpleTab, Debate Adjudicator and CrabbyTab: offline-first tools for debate tournaments and rounds | 5 | [#9](https://github.com/orgs/The-Studio-of-Sadiq/projects/9) |
| [Electrical Basics](#electrical-basics) | Eight open textbooks, from mathematics and physics to machines and systems integration | 8 | [#7](https://github.com/orgs/The-Studio-of-Sadiq/projects/7) |
| [Nuclear IDE](#nuclear-ide) | Browser workbenches for ELSEPA, FRESCO and DFMSPH, with the Fortran compiled to WebAssembly | 3 | [#4](https://github.com/orgs/The-Studio-of-Sadiq/projects/4) |
| [Prefab RCC Feasibility](#prefab-rcc-feasibility-bangladesh) | Research data and models on precast RCC buildings in Bangladesh under BNBC 2020 | 1 | [#3](https://github.com/orgs/The-Studio-of-Sadiq/projects/3) |

## SAEngine

<img src="https://raw.githubusercontent.com/The-Studio-of-Sadiq/SAEngine/main/docs/images/fem-visuals/after-run-all-results.png" alt="SAEngine FEM results after Run All" width="720">

Takes a building from the soil report to a finished design package: FEM analysis in OpenSees, reinforced concrete and foundation design, drawings, bill of quantities and a calculation report in one program. Building codes ship as code packs: BNBC 2020 by default, plus ACI/ASCE, Eurocodes and Indian Standards. Native fork of Code - OSS. AGPL-3.0.

- Repo: [SAEngine](https://github.com/The-Studio-of-Sadiq/SAEngine) · Site: [thestudioofsadiq.tech/SAEngine](https://thestudioofsadiq.tech/SAEngine/) · [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/8)
- Status: Pre-Alpha 9 (0.0.48), released for trying and feedback, not for signed design work. Strongest path is RC buildings end to end. Pushover, time history, P-delta, construction staging, isolators and bridges are built but not yet verified. Steel design depth, MEP (coordination grade) and the architecture layer are partial.
- Recent: live co-editing over the office's own Yjs relay, a UI/UX round with a stage bar and New Project wizard, a 10-storey Run All cut from 7.2 to 2.7 minutes, and an AI assistant that builds a whole project from one prompt.
- Next: shared editing actions and terminal commands, electrical design, post-tensioned slabs, steel auto-sizing, Bangla language, depth tests and verification examples. Board: 22 done, 24 to do.
- Companions: [saengine-design-codes](https://github.com/The-Studio-of-Sadiq/saengine-design-codes) (code packs), [saengine-structure-templates](https://github.com/The-Studio-of-Sadiq/saengine-structure-templates) (parametric trusses, arches, domes, cable nets), [saengine-building-templates](https://github.com/The-Studio-of-Sadiq/saengine-building-templates), [saengine-index](https://github.com/The-Studio-of-Sadiq/saengine-index) (signed package index), [saengine-steel-design](https://github.com/The-Studio-of-Sadiq/saengine-steel-design) (read-only mirror).

## Debate Operating System

<img src="https://raw.githubusercontent.com/The-Studio-of-Sadiq/simpletab/main/docs/brand/banner.png" alt="SimpleTab banner" width="720">

Free, offline-first tools that cover a debate tournament end to end. [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/9).

| Product | What it does | Repos | Status |
| --- | --- | --- | --- |
| **SimpleTab** | Tabulation for British Parliamentary and two-team formats up to WUDC size. One host laptop runs the tournament without internet, tab staff join over a local network and edit live, and optional phone ballots go through a Cloudflare Worker + D1 service. Static public results, a hash-chained verifiable change log, English and Bangla. AGPL-3.0. | [simpletab](https://github.com/The-Studio-of-Sadiq/simpletab), [simpletab-ballots](https://github.com/The-Studio-of-Sadiq/simpletab-ballots), [simpletab-public](https://github.com/The-Studio-of-Sadiq/simpletab-public) | Done: M0, M1, M5, M6, M8. In progress: M2, M3, M4, M7, M9. To do: M10, M11. |
| **Debate Adjudicator** | Runs each debate room from the chair's phone or laptop: synced timer and bells over local Wi-Fi, POIs from debaters' phones, recordings, offline Whisper transcription, ballots and a PDF report. 49 formats. Android and Windows. | [debate-adjudicator](https://github.com/The-Studio-of-Sadiq/debate-adjudicator) · [Site](https://the-studio-of-sadiq.github.io/debate-adjudicator/) | v0.6.0 |
| **CrabbyTab** | Tabbycat-inspired offline-first tab web app (Next.js). | [crabbytab](https://github.com/The-Studio-of-Sadiq/crabbytab) | Legacy, superseded by SimpleTab |

## Electrical Basics

Open textbooks in Markdown and LaTeX, with script-computed figures, one-command PDF builds, and most with an MCP server so AI assistants can read them. [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/7).

| Repo | Scope | Size |
| --- | --- | --- |
| [Engineering-Mathematics](https://github.com/The-Studio-of-Sadiq/Engineering-Mathematics) | The Mathematics Universe: 25-chapter core, 74 chapters in 9 tracks, research frontier | 1,422-page PDF |
| [Engineering-Physics](https://github.com/The-Studio-of-Sadiq/Engineering-Physics) | Top-down descent from fundamental physics to engineering equations | In progress |
| [Circuits-Signals-and-Communications](https://github.com/The-Studio-of-Sadiq/Circuits-Signals-and-Communications) | Book 3: networks, signals, DSP, communications, intro control | 35 chapters, 780-page PDF, v1.0.0 |
| [Electronics-and-Computing](https://github.com/The-Studio-of-Sadiq/Electronics-and-Computing) | Book 4: devices, analog and digital, architecture, embedded, VLSI | 35 chapters, 654-page PDF, v1.0.0 |
| [Electrical-Energy-and-Machines](https://github.com/The-Studio-of-Sadiq/Electrical-Energy-and-Machines) | Book 5: machines, drives, power systems, protection | 30 chapters, 600-page PDF, v1.0.0 |
| [Applications-and-Integrations](https://github.com/The-Studio-of-Sadiq/Applications-and-Integrations) | Book 6: project-oriented systems integration | 38+ chapters, 953-page PDF, v1.0.0 |
| [Advanced-Chemistry](https://github.com/The-Studio-of-Sadiq/Advanced-Chemistry) | Quantum chemistry built up from physics | 37 chapters, 249 figures |
| [Materials-Science-and-Engineering](https://github.com/The-Studio-of-Sadiq/Materials-Science-and-Engineering) | Structure and thermodynamics to processing, characterization and design | 59 chapters |

## Nuclear IDE

Browser workbenches for established Fortran nuclear and atomic physics codes. The official Fortran is compiled to WebAssembly, so each app runs in the browser and offline as an installable PWA. [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/4).

| Repo | What it does | Status |
| --- | --- | --- |
| [Electron-Scattering](https://github.com/The-Studio-of-Sadiq/Electron-Scattering) | GUI for ELSEPA 2021: Dirac partial-wave elastic scattering of electrons and positrons by atoms, ions and molecules. Built with the HSTU Research Society. | v2.0.0 with a [Zenodo DOI](https://doi.org/10.5281/zenodo.21716740); live at [electron-scattering.onrender.com](https://electron-scattering.onrender.com/) |
| [FRESCO-GUI-PWA](https://github.com/The-Studio-of-Sadiq/FRESCO-GUI-PWA) | FRESCO coupled-channels nuclear reaction calculations and SFRESCO fitting. | Live at [fresco-gui-pwa.onrender.com](https://fresco-gui-pwa.onrender.com/) |
| [DFMSPH-PWA](https://github.com/The-Studio-of-Sadiq/DFMSPH-PWA) | DFMSPH double-folding potentials with a GUI. | Live at [dfmsph-pwa.vercel.app](https://dfmsph-pwa.vercel.app) |

## Prefab RCC Feasibility (Bangladesh)

[Prefab-RCC-feasibility-in-BD](https://github.com/The-Studio-of-Sadiq/Prefab-RCC-feasibility-in-BD): supplementary data, ETABS and Revit models for "Techno-Economic Feasibility of Modular Precast Concrete Systems in Bangladesh: A Case Study Based on BNBC 2020", now split into a pre-feasibility paper and a structural and seismic performance paper. [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/3).

## Also in the studio

| Repo | What it does |
| --- | --- |
| [MAEngine](https://github.com/The-Studio-of-Sadiq/MAEngine) | Mechanical engineering IDE and simulation workbench on Code - OSS: build123d/OpenCASCADE, Gmsh, CalculiX, Elmer, OpenRadioss. Apache-2.0, early stage. |
| [Bish-Pani-Radar](https://github.com/The-Studio-of-Sadiq/Bish-Pani-Radar) | NASA Space Apps entry: InSAR early warning of groundwater arsenic intrusion in the Bengal Delta. Live at [bish-pani-radar.vercel.app](https://bish-pani-radar.vercel.app) |
| [MUN-Mesh](https://github.com/The-Studio-of-Sadiq/MUN-Mesh) | Offline multi-hop chat and file sharing for MUN conferences of 400–500. Tested at 503 simulated devices. |
| [Discord-Audit-Bot](https://github.com/The-Studio-of-Sadiq/Discord-Audit-Bot) | Self-hosted Discord audit logging bot. |

## About

Maintained by Sadiq Khan, Electrical & Electronic Engineering, HSTU, Bangladesh. Issues and feedback on any repo are welcome.
