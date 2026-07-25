# MCP4RS Open Earth Roadmap

## Status Key

- Done: completed and publicly available
- In Progress: active work underway
- Planned: committed next work
- Exploratory: options under evaluation

## Roadmap Table

| Stage | Component | Task Type | Current Asset | Purpose | Status | Next Step |
| --- | --- | --- | --- | --- | --- |
| 1 | MCP Server | Infrastructure | https://github.com/MCP4RemoteSensing/mcp4rs-open-earth | Core remote-sensing MCP tools for source discovery, analysis, and explanation. | Done | Expose and document all `server.py` tools. |
| 2 | MCP Demo Space | Product | https://huggingface.co/spaces/zlysunshine/mcp4rs-open-earth | Demonstrates the MCP server through Hugging Face Gradio MCP support. | Done | Add clearer MCP endpoint and client setup docs. |
| 3 | Media Gallery Workflow | Product | https://github.com/MCP4RemoteSensing/mcp4rs-media-gallery | Turns source queries into provenance JSON and rendered media. | Done | Connect live MCP calls in future. |
| 4 | Media Gallery Space | Product | https://huggingface.co/spaces/zlysunshine/mcp4rs-media-gallery | Demonstrates practical use cases of MCP-enabled remote-sensing workflows. | Done | Improve gallery UX and provenance display. |
| 5 | Gallery Dataset | Data | https://huggingface.co/datasets/MCP4RemoteSensing/mcp4rs-media-gallery-outputs | Publishes generated images, GIFs, and provenance records. | Done | Add metadata, limitations, and examples. |
| 6 | Agent Skills | Ecosystem | Future repo or skill package | Wrap Python workflows as reusable agent-executable skills. | Planned | Define first skill: query to render to provenance report. |
| 7 | Model Releases | Data/Model | Future Hugging Face model repo | Fine-tune or adapt models using MCP-retrieved images and metadata. | Planned | Select base model and dataset scope. |
| 8 | MCP Registries | Distribution | Official MCP Registry, GitHub MCP Registry, Glama, Smithery, PulseMCP, MCP.so, awesome lists | Make MCP4RS discoverable by agents and developers. | In Progress | Prepare registry metadata package. |
| 9 | Commercialization | Business | API gateway, hosted skills, enterprise deployment, token economics | Sustain the ecosystem while keeping open-science assets public. | Exploratory | Compare API pricing and web3 incentive models. |

## Progress Checklist

### Completed Foundations

- [x] Core MCP server published
- [x] Public MCP demo launched
- [x] Reproducible media-gallery workflow published
- [x] Public use-case gallery Space launched
- [x] Gallery outputs dataset published

### Active and Near-Term Work

- [ ] Finalize complete MCP tool reference documentation
- [ ] Improve client onboarding and endpoint setup guide
- [ ] Package and submit MCP registry metadata
- [ ] Define and ship first Agent Skill specification
- [ ] Scope first model release and evaluation criteria
- [ ] Define commercialization guardrails before monetization tracks

## Roadmap Diagram

```mermaid
flowchart LR
    classDef done fill:#E8F5E9,stroke:#2E7D32,stroke-width:1px,color:#1B5E20;
    classDef progress fill:#E3F2FD,stroke:#1565C0,stroke-width:1px,color:#0D47A1;
    classDef planned fill:#FFF8E1,stroke:#E65100,stroke-width:1px,color:#BF360C;
    classDef explore fill:#FBE9E7,stroke:#D84315,stroke-width:1px,color:#BF360C;
    classDef infra stroke-dasharray: 4 2;
    classDef product stroke-width:2px;
    classDef data stroke-width:2px;
    classDef business stroke-dasharray: 2 2;

    S1["MCP Server"]:::done
    S2["MCP Demo Space"]:::done
    S3["Media Gallery Workflow"]:::done
    S4["Gallery Space"]:::done
    S5["Gallery Dataset"]:::done
    S6["Agent Skills"]:::planned
    S7["Model Releases"]:::planned
    S8["MCP Registries"]:::progress
    S9["Commercialization"]:::explore

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

    class S1,S8 infra;
    class S2,S3,S4 product;
    class S5,S7 data;
    class S9 business;
```

Diagram legend:

- Green fill: done
- Blue fill: in progress
- Amber fill: planned
- Orange fill: exploratory
- Dashed border: infrastructure/distribution tasks
- Thick border: product or data tasks
- Fine dashed border: business-track tasks

## Roadmap Narrative

MCP4RS Open Earth begins with a working MCP server for open remote-sensing data.
The server exposes tools for discovering, analyzing, and explaining Earth
observation sources. The Hugging Face MCP demo Space gives users a public web
entry point and an MCP-compatible demonstration surface.

The Media Gallery extends the server concept into reproducible workflows:
source discovery, provenance export, Python rendering, and generated images or
GIFs. The gallery outputs are published as a Hugging Face dataset so they can be
used in documentation, teaching, demos, and future model-release experiments.

The next layer is Agent Skills. These skills can wrap repeatable Python
workflows around MCP calls, validate provenance, and return reports or media.
Future model releases can fine-tune or adapt existing remote-sensing and
multimodal models using MCP-retrieved images and source metadata.

The ecosystem then expands through MCP registries and platform listings, while
commercialization can be explored through hosted API access, managed workflows,
enterprise deployment, and web3 token-economic mechanisms for credits,
provenance, contributor rewards, and governance.

## Immediate Priorities

| Priority | Work Item | Output |
| --- | --- | --- |
| P0 | Document all MCP server tools | Tool reference with inputs, outputs, use cases, and examples. |
| P0 | Link every public asset | Cross-links in GitHub READMEs, Hugging Face cards, and dataset cards. |
| P0 | Stabilize Hugging Face demo releases | Clear sync workflow and release checklist. |
| P1 | Prepare MCP registry package | Description, tags, screenshots, endpoint/package metadata, badges. |
| P1 | Define first Agent Skill | A reproducible query-render-report workflow. |
| P1 | Draft model release scope | Base model, dataset scope, evaluation task, model card requirements. |
| P2 | Explore commercialization | Hosted API, managed workflows, enterprise services, token economics. |
