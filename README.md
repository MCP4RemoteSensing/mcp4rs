# MCP4RS Open Earth Ecosystem

[![Roadmap](https://img.shields.io/badge/Roadmap-Active-0A7A3C)](ROADMAP.md)
[![Assets](https://img.shields.io/badge/Public%20Assets-5-1B5EAA)](ASSET_MAP.md)
[![Status](https://img.shields.io/badge/Stage-MVP%20to%20Scale-C67F00)](ROADMAP.md)

Public roadmap and asset map for the MCP4RS Open Earth ecosystem: MCP server,
Hugging Face demos, reproducible media gallery, datasets, future Agent Skills,
model releases, registry distribution, and commercialization paths.

## Ecosystem At a Glance

| Category | Asset | Type | Link | Status | Next |
| --- | --- | --- | --- | --- | --- |
| 🧩 Core Platform | MCP4RS Open Earth | <img alt="GitHub" src="https://img.shields.io/badge/GitHub-Repository-181717?logo=github&logoColor=white"> | https://github.com/MCP4RemoteSensing/mcp4rs-open-earth | 🟢 Live | Complete tool-level documentation |
| 🚀 Public Demo | MCP4RS Open Earth Demo | <img alt="Hugging Face Space" src="https://img.shields.io/badge/Hugging%20Face-Space-FF9D00?logo=huggingface&logoColor=black"> | https://huggingface.co/spaces/zlysunshine/mcp4rs-open-earth | 🟢 Live | Improve endpoint and client quickstart |
| ⚙️ Workflow Engine | MCP4RS Media Gallery | <img alt="GitHub" src="https://img.shields.io/badge/GitHub-Repository-181717?logo=github&logoColor=white"> | https://github.com/MCP4RemoteSensing/mcp4rs-media-gallery | 🟢 Live | Connect more live MCP-integrated workflows |
| 🖼️ Use-Case Demo | MCP4RS Media Gallery Demo | <img alt="Hugging Face Space" src="https://img.shields.io/badge/Hugging%20Face-Space-FF9D00?logo=huggingface&logoColor=black"> | https://huggingface.co/spaces/zlysunshine/mcp4rs-media-gallery | 🟢 Live | Enhance UX and provenance browsing |
| 🗂️ Output Archive | Media Gallery Outputs | <img alt="Hugging Face Dataset" src="https://img.shields.io/badge/Hugging%20Face-Dataset-FF9D00?logo=huggingface&logoColor=black"> | https://huggingface.co/datasets/MCP4RemoteSensing/mcp4rs-media-gallery-outputs | 🟢 Live | Add richer metadata and examples |
| 🤖 Agent Skills | Skill package roadmap | Planned package | docs/AGENT_SKILLS_PLAN.md | 🟡 Planned | Publish first query -> render -> report skill |
| 🧠 Model Releases | Model release roadmap | Planned package | docs/MODEL_RELEASE_PLAN.md | 🟡 Planned | Select baseline model and evaluation setup |
| 🧭 Registry Distribution | Registry submission roadmap | Planned listing | docs/MCP_PLATFORM_REGISTRATION.md | 🔵 In Progress | Submit metadata package to target registries |
| 💼 Commercialization | Commercialization roadmap | Strategic plan | docs/COMMERCIALIZATION_PLAN.md | 🟠 Exploratory | Define staged service and governance model |
| ➕ Future Categories | Additional ecosystem tracks | ... | ... | ⚪ ... | ... |

Status legend: 🟢 Live | 🔵 In Progress | 🟡 Planned | 🟠 Exploratory | ⚪ Placeholder

## Delivery Status

### 🧩 Core Platform

- [x] Publish MCP4RS Open Earth repository
- [ ] Complete tool-by-tool documentation and examples

### 🚀 Public Demo

- [x] Release MCP demo on Hugging Face Spaces
- [ ] Improve endpoint and client onboarding quickstart

### ⚙️ Workflow Engine

- [x] Open-source Media Gallery workflow repository
- [ ] Add more live MCP-integrated workflow paths

### 🖼️ Use-Case Demo

- [x] Release Media Gallery demonstration Space
- [ ] Enhance UX and provenance exploration

### 🗂️ Output Archive

- [x] Publish outputs dataset with provenance artifacts
- [ ] Expand metadata quality and usage examples

### 🤖 Agent Skills

- [ ] Publish first skill: query -> render -> report

### 🧠 Model Releases

- [ ] Select baseline model and evaluation setup

### 🧭 Registry Distribution

- [ ] Prepare and submit registry metadata package

### 💼 Commercialization

- [ ] Define staged service model and governance guardrails

## Ecosystem Roadmap (Done vs Planned)

```mermaid
flowchart LR
    classDef doneInfra fill:#E8F5E9,stroke:#1565C0,stroke-width:2px,color:#1B5E20;
    classDef doneProduct fill:#E8F5E9,stroke:#6A1B9A,stroke-width:2px,color:#1B5E20;
    classDef doneGrowth fill:#E8F5E9,stroke:#AD1457,stroke-width:2px,color:#1B5E20;
    classDef planInfra fill:#FFF8E1,stroke:#1565C0,stroke-width:2px,color:#BF360C;
    classDef planProduct fill:#FFF8E1,stroke:#6A1B9A,stroke-width:2px,color:#BF360C;
    classDef planGrowth fill:#FFF8E1,stroke:#AD1457,stroke-width:2px,color:#BF360C;

    S1["🧩 MCP Server"]:::doneInfra
    S2["🚀 MCP Demo Space"]:::doneProduct
    S3["⚙️ Media Gallery Repo"]:::doneGrowth
    S4["🖼️ Gallery Space"]:::doneProduct
    S5["🗂️ Gallery Dataset"]:::doneGrowth
    S6["🤖 Agent Skills"]:::planProduct
    S7["🧠 Model Releases"]:::planGrowth
    S8["🧭 MCP Registries"]:::planInfra
    S9["💼 Commercialization"]:::planGrowth

    S1 --> S2
    S1 --> S3
    S3 --> S4
    S3 --> S5
    S5 --> S7
    S3 --> S6
    S1 --> S8
    S6 --> S9
    S7 --> S9
    S8 --> S9

```

Legend:

- ✅ Status fill #E8F5E9 🟩: completed or live assets
- 🗓️ Status fill #FFF8E1 🟨: planned or exploratory assets
- 🧩🧭 Border #1565C0 □🟦: infrastructure and distribution nodes
- 🚀🖼️🤖 Border #6A1B9A □🟪: product and user experience nodes
- ⚙️🗂️🧠💼 Border #AD1457 □🩷: growth, ecosystem, and business nodes

Legend marker note: filled rules use solid color squares; border rules use hollow square markers (□) plus matching color chips.

## Roadmap Documents

| Document | Purpose |
| --- | --- |
| [ROADMAP.md](ROADMAP.md) | Stage-by-stage roadmap with status and immediate priorities. |
| [ASSET_MAP.md](ASSET_MAP.md) | Public asset inventory and relationship map. |
| [docs/AGENT_SKILLS_PLAN.md](docs/AGENT_SKILLS_PLAN.md) | Plan for packaging repeatable workflows as agent-executable skills. |
| [docs/MODEL_RELEASE_PLAN.md](docs/MODEL_RELEASE_PLAN.md) | Model adaptation and release direction from MCP-derived assets. |
| [docs/MCP_PLATFORM_REGISTRATION.md](docs/MCP_PLATFORM_REGISTRATION.md) | Registry listing strategy and readiness checklist. |
| [docs/COMMERCIALIZATION_PLAN.md](docs/COMMERCIALIZATION_PLAN.md) | Sustainable commercialization options with open-science guardrails. |
