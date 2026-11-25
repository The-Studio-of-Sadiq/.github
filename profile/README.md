<div align="center">

# The Studio of Sadiq

Open engineering software: structural and mechanical analysis, debate tabulation, scientific tools, and open textbooks.

[thestudioofsadiq.tech](https://thestudioofsadiq.tech/) · [Project boards](https://github.com/orgs/The-Studio-of-Sadiq/projects)

</div>

The Studio of Sadiq builds free, open-source tools for engineering practice, research and teaching: desktop engineering workbenches, offline-first apps, and browser front ends for established scientific codes. The work runs from soil reports and finite-element models to nuclear scattering calculations and 1,400-page textbooks. Everything here is public; most projects are usable today, with their known gaps listed in each repo.

## Now building

Three flagships carry most of the current work.

### SAEngine — structural analysis and design

Takes a building from the soil report to a finished design package: FEM analysis in OpenSees, reinforced concrete and foundation design, drawings, bill of quantities and a calculation report in one program. Building codes ship as code packs: BNBC 2020 by default, plus ACI/ASCE, Eurocodes and Indian Standards. Native fork of Code - OSS.

- Repo: [SAEngine](https://github.com/The-Studio-of-Sadiq/SAEngine) · Site: [thestudioofsadiq.tech/SAEngine](https://thestudioofsadiq.tech/SAEngine/) · [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/8)
- Status: Pre-Alpha 9 (0.0.48), released for trying and feedback, not for signed design work. Strongest path is RC buildings end to end. Pushover, time history, P-delta, construction staging, isolators and bridges are built but not yet verified. Steel design depth, MEP (coordination grade) and the architecture layer are partial.
- Recent: live co-editing over the office's own Yjs relay, a UI/UX round with a stage bar and New Project wizard, a 10-storey Run All cut from 7.2 to 2.7 minutes, and an AI assistant that builds a whole project from one prompt.
- Next: shared editing actions and terminal commands, electrical design, post-tensioned slabs, steel auto-sizing, Bangla language, depth tests and verification examples. Board: 16 done, 30 to do.
- Companions: [saengine-design-codes](https://github.com/The-Studio-of-Sadiq/saengine-design-codes) (code packs), [saengine-structure-templates](https://github.com/The-Studio-of-Sadiq/saengine-structure-templates) (parametric trusses, arches, domes, cable nets), [saengine-building-templates](https://github.com/The-Studio-of-Sadiq/saengine-building-templates), [saengine-index](https://github.com/The-Studio-of-Sadiq/saengine-index) (signed package index), [saengine-steel-design](https://github.com/The-Studio-of-Sadiq/saengine-steel-design) (read-only mirror).

### MAEngine — mechanical analysis

An open-source mechanical engineering IDE and simulation workbench on Code - OSS. The rule is to integrate battle-tested open source rather than rewrite it: OpenCASCADE through build123d for CAD, Gmsh for meshing, meshio for exchange, and CalculiX, Elmer and OpenRadioss as solvers.

- Repo: [MAEngine](https://github.com/The-Studio-of-Sadiq/MAEngine) · Apache-2.0 · Early stage.

### SimpleTab — debate tabulation

Offline-first tabulation for British Parliamentary and two-team formats up to WUDC size, and the successor to CrabbyTab. One host laptop runs the tournament without internet, tab staff join over a local network and edit live, and optional phone ballots go through a Cloudflare Worker + D1 service. Also a static public results site, a hash-chained verifiable change log, and English and Bangla.

- Repos: [simpletab](https://github.com/The-Studio-of-Sadiq/simpletab), [simpletab-ballots](https://github.com/The-Studio-of-Sadiq/simpletab-ballots), [simpletab-public](https://github.com/The-Studio-of-Sadiq/simpletab-public) · [Board](https://github.com/orgs/The-Studio-of-Sadiq/projects/9) · AGPL-3.0
- Done: M0 core logic, M1 host app, M5 live collaboration, M6 terminal and AI helper.
- In progress: M2 Git panel, M3 online ballots and phone app, M4 public site and archive, M7 file explorer.
- To do: M8 command palette, M9 extensions, M10 open registration, M11 OMR paper ballots.

## Scientific software

| Repo | What it does | Status |
| --- | --- | --- |
| [Electron-Scattering](https://github.com/The-Studio-of-Sadiq/Electron-Scattering) | Browser GUI for ELSEPA 2021: Dirac partial-wave elastic scattering of electrons and positrons by atoms, ions and molecules, with the official Fortran compiled to WebAssembly. Built with the HSTU Research Society. | v2.0.0 with a Zenodo DOI; [board](https://github.com/orgs/The-Studio-of-Sadiq/projects/4) at 32 of 33 items |
| [FRESCO-GUI-PWA](https://github.com/The-Studio-of-Sadiq/FRESCO-GUI-PWA) | Web GUI for FRESCO coupled-channels nuclear reaction calculations. | Live at [fresco-gui-pwa.onrender.com](https://fresco-gui-pwa.onrender.com/) |
| [DFMSPH-PWA](https://github.com/The-Studio-of-Sadiq/DFMSPH-PWA) | DFMSPH with a PWA and GUI. | Live at [dfmsph-pwa.vercel.app](https://dfmsph-pwa.vercel.app) |
| [Bish-Pani-Radar](https://github.com/The-Studio-of-Sadiq/Bish-Pani-Radar) | NASA Space Apps entry: Sentinel-1 / NISAR InSAR early-warning surveillance of compaction-triggered groundwater arsenic intrusion in the Bengal Delta, checked against a published Araihazar site study. | Live at [bish-pani-radar.vercel.app](https://bish-pani-radar.vercel.app) |

## Open textbooks

Markdown and LaTeX, script-computed figures, one-command PDF builds, and most with an MCP server so AI assistants can read them.

| Repo | Scope | Size |
| --- | --- | --- |
| [Engineering-Mathematics](https://github.com/The-Studio-of-Sadiq/Engineering-Mathematics) | The Mathematics Universe: 25-chapter core, 74 chapters in 9 tracks, research frontier | 1,422-page PDF |
| [Engineering-Physics](https://github.com/The-Studio-of-Sadiq/Engineering-Physics) | Top-down descent from fundamental physics to engineering equations | In progress |
| [Circuits-Signals-and-Communications](https://github.com/The-Studio-of-Sadiq/Circuits-Signals-and-Communications) | Book 3: networks, signals, DSP, communications, intro control | 35 chapters, 780-page PDF |
| [Electronics-and-Computing](https://github.com/The-Studio-of-Sadiq/Electronics-and-Computing) | Book 4: devices, analog and digital, architecture, embedded, VLSI | 35 chapters, 654-page PDF, v1.0.0 |
| [Electrical-Energy-and-Machines](https://github.com/The-Studio-of-Sadiq/Electrical-Energy-and-Machines) | Book 5: machines, drives, power systems, protection | 30 chapters, 600-page PDF |
| [Applications-and-Integrations](https://github.com/The-Studio-of-Sadiq/Applications-and-Integrations) | Book 6: project-oriented systems integration | 38+ chapters, 953-page PDF, v1.0.0 |
| [Advanced-Chemistry](https://github.com/The-Studio-of-Sadiq/Advanced-Chemistry) | Quantum chemistry built up from physics | 37 chapters, 249 figures |
| [Materials-Science-and-Engineering](https://github.com/The-Studio-of-Sadiq/Materials-Science-and-Engineering) | Structure and thermodynamics to processing, characterization and design | 59 chapters |

## Debate and community tools

| Repo | What it does | Notes |
| --- | --- | --- |
| [debate-adjudicator](https://github.com/The-Studio-of-Sadiq/debate-adjudicator) | Offline timer, bells, POIs, Whisper transcription and ballots for Android and Windows | [Site](https://the-studio-of-sadiq.github.io/debate-adjudicator/) |
| [crabbytab](https://github.com/The-Studio-of-Sadiq/crabbytab) | Tabbycat-inspired offline-first tab web app | Superseded by SimpleTab |
| [MUN-Mesh](https://github.com/The-Studio-of-Sadiq/MUN-Mesh) | Offline multi-hop chat and file sharing for MUN conferences of 400–500 | Tested at 503 simulated devices |
| [Discord-Audit-Bot](https://github.com/The-Studio-of-Sadiq/Discord-Audit-Bot) | Self-hosted Discord audit logging bot | |

## Research

| Repo | Contents |
| --- | --- |
| [Prefab-RCC-feasibility-in-BD](https://github.com/The-Studio-of-Sadiq/Prefab-RCC-feasibility-in-BD) | Supplementary data for "Techno-Economic Feasibility of Modular Precast Concrete Systems in Bangladesh: A Case Study Based on BNBC 2020" |

## About

Maintained by Sadiq Khan, Electrical & Electronic Engineering, HSTU, Bangladesh. Issues and feedback on any repo are welcome.
