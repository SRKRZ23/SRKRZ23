# Hi, I'm Sardor 👋

**Independent AI/ML engineer · Cost-efficient & on-prem LLM infrastructure · AI governance · Tashkent, Uzbekistan**

I build open-source infrastructure for running LLMs affordably and safely — cost routing & metering, on-prem/local-first inference, model evaluation, and agent governance. AMD Developer Hackathon **ACT I winner** (REPOMIND). Latest: **[Frugal](https://github.com/SRKRZ23/frugal)** — the layer that keeps agent inference cheap, local, and verified.

---

## 🌟 Featured — Frugal (open-source LLM cost ops)

<p align="center"><a href="https://github.com/SRKRZ23/frugal"><img src="https://raw.githubusercontent.com/SRKRZ23/frugal/main/assets/banner.png" alt="Frugal" width="100%"></a></p>

**[Frugal](https://github.com/SRKRZ23/frugal)** — run AI agents cheap, local, and verified. Meters every
model call, routes the cheap/local model first, and escalates to a strong model only when a real check
fails — then proves quality in CI. Inference is now **~85% of the enterprise AI budget** (Uber burned its
whole 2026 coding budget by April; one firm spent $500M/mo on Claude) — Frugal routes around it.

- 📊 Measured on a real cluster: a **3B model matched a 14B on 83% of hard tasks**, ~4.7–11× faster → **~75–97% cheaper**
- 🧪 **56 tests**, CI green, 0 runtime deps · 8 real bugs found & fixed by our own pressure/fuzz/concurrency suites
- 💸 Modeled enterprise saving: at **$10M/mo** inference spend → **$60–90M/yr** ([math + company roster](https://github.com/SRKRZ23/frugal/blob/main/ENTERPRISE.md))
- 🌐 **[Live site + interactive deck](https://frugal-cost-router.netlify.app)** · ★ **[Repo](https://github.com/SRKRZ23/frugal)** · Apache-2.0

## 🏆 Recent highlights (2026)

- 🥇 **REPOMIND — WON 1st place**, AMD Developer Hackathon **ACT I** (AI Agents track) **+ Outstanding Social Engagement** — prize: AMD Radeon AI PRO R9700 GPU + cash. [repo](https://github.com/SRKRZ23/repomind)
- 🚀 **REPOMIND v3** — submitted to AMD Developer Hackathon **ACT II** (Track 3 · Unicorn); qualified in the automated pre-screen (human panel pending). On-prem coding agent + LLM cost-router.
- 🌟 **Frugal** — new open-source LLM cost-routing / eval / MCP toolkit (above).

---

## 🧩 The 4-Product AI Safety Ecosystem

```
                ┌───────────────────────────────────┐
                │  CITADEL — Model Evaluation       │  ← evaluates which models are safe
                │  github.com/SRKRZ23/citadel        │
                └─────────────┬─────────────────────┘
                              │
        ┌─────────────────────┼─────────────────────┐
        │                     │                     │
┌───────▼────────┐  ┌─────────▼─────────┐  ┌────────▼────────┐
│  FORGE         │  │  SOUF AI          │  │  ATLAS          │
│  Policy Gen    │  │  Inline Firewall  │  │  Agent Routing  │
│  (IBM Bob)     │  │  (Veea Lobster T) │  │  (multi-agent)  │
└────────────────┘  └───────────────────┘  └─────────────────┘
                              │
                  ┌───────────▼───────────┐
                  │  Shared Ed25519       │
                  │  audit chain          │
                  │  (built once, reused) │
                  └───────────────────────┘
```

**60%+ cross-product code reuse.** One codebase. One mission: governance infrastructure that's free, open, and reproducible.

---

## ⚡ Resource Compounding Story

I shipped 4 hackathon submissions in 3 days (May 17–19) via **shared infrastructure earned from prior submissions**:

- 🔥 **AMD MI300X GPU access** (earned at REPOMIND, AMD Hackathon May 11) → real Gemma 3 27B benchmark in CITADEL (87.5% authority resistance, 72.8 tok/s on 192GB HBM3)
- 🔧 **IBM Bob coding agent credits** (40 Bobcoins from IBM Bob Hackathon) → 27 to FORGE + 13 to CITADEL extension (multilingual prompts, edge adapters, compliance docs)
- ⚙️ **SOUF AI Ed25519 audit chain** → reused as CITADEL L7 provenance layer + ATLAS ingress audit core

Each prize funds the next submission. Each architecture decision pays for two more products.

---

## 📊 Active Open-Source Products

### [SOUF AI](https://github.com/SRKRZ23/souf-ai) — Sub-millisecond LLM Governance
F1=1.000 on 231 adversarial prompts across 5 benchmarks. **1,800× faster than Meta Prompt Guard 2** (measured 0.079ms vs 92.4ms on A100 per Meta's model card). Built-in HIPAA + PCI-DSS packs. Ed25519-signed audit chain.
[Video walkthrough](https://youtu.be/IwLt1OTehcQ) · [Lablab submission](https://lablab.ai/ai-hackathons/techex-intelligent-enterprise-solutions-hackathon/souf-ai/souf-ai-sub-millisecond-llm-governance)

### [CITADEL](https://github.com/SRKRZ23/citadel) — Open AI Evaluation Infrastructure
13-layer L0–L12 architecture. Gemma 4 27B benchmarked against 5 frontier models. EU AI Act / NIST / ISO 42001 / HIPAA compliance reports. **Real AMD MI300X pilot run.**
[Live Streamlit demo](https://citadel-srkrz23.streamlit.app) · [Video](https://youtu.be/X0-hIwePRXs)

### [FORGE](https://github.com/SRKRZ23/ibm-bob-forge) — LLM Security Policy Generator
OWASP LLM Top 10 mapping → YAML policies → BobShell audit trail. Built with IBM Bob coding agent.
[Video walkthrough](https://youtu.be/_9PXGN_nxn8)

### [ATLAS](https://github.com/SRKRZ23/atlas) — Enterprise Multi-Agent System with Governance
6-layer governed pipeline: Voice → SOUF AI DPI gate → Gemini orchestrator → Featherless router → Tool executor → Ed25519 audit. 29/29 tests PASS in under 1 second. All 5 Milan AI Week sponsors integrated (Speechmatics + Featherless + Gemini + Vultr + Kraken).
[Video walkthrough](https://youtu.be/i78OdyRYiOs) · [Lablab submission](https://lablab.ai/ai-hackathons/milan-ai-week-hackathon/atlas/atlas-enterprise-multi-agent-governance)

### [REPOMIND](https://github.com/SRKRZ23/repomind) — Repo-Scale Coding Agent on AMD MI300X 🥇
Open-source large-context (256K) FP8 inference on AMD MI300X. **WON 1st place — AMD Developer Hackathon ACT I (AI Agents track) + Outstanding Social Engagement.** ACT II (v3: on-prem agent + LLM cost-router) submitted, qualified in the automated pre-screen.

### [ECB v1](https://github.com/SRKRZ23/ecb) — Epistemic Curie Benchmark
Quantitative framework for measuring when LLMs surrender independent reasoning under authority pressure. 7 frontier models, 2,520 measurements. Wilson 95% CI methodology.
[**Zenodo DOI: 10.5281/zenodo.19791329**](https://doi.org/10.5281/zenodo.19791329)

---

## 🎓 Background

- **Founded UCAR** (2023, Tashkent) — U-Start Demo Day **1st place** + 85M UZS grant; Korea-Uzbekistan Startup Exchange **2nd place in Seoul**
- **Youngest student in UJC's PMP-43 senior executive cohort**
- **Scholarship to Zhejiang University**
- **Foundation Year at Leeds Beckett University**, UK
- **Kaggle SPR Mammography: 7/371** (Top 1.9%, Medical AI)
- **CVPR 2026 CV4CHL Gait Challenge** — Kaggle LB 2nd (0.90271); official 6th on the held-out set; Proceedings co-author
- **AMD Developer Hackathon 2026 Track 1** with REPOMIND

---

## 🔗 Links

- **ORCID:** [0009-0007-0731-4247](https://orcid.org/0009-0007-0731-4247)
- **Zenodo:** [10.5281/zenodo.19791329](https://doi.org/10.5281/zenodo.19791329)
- **HuggingFace:** [@ZeroR3](https://huggingface.co/ZeroR3)
- **LinkedIn:** [sardor-razikov-569a5327b](https://linkedin.com/in/sardor-razikov-569a5327b)
- **X / Twitter:** [@SardorRazi99093](https://x.com/SardorRazi99093)
- **Email:** razikovsardor1@gmail.com

---

> *"Every researcher deserves the same evaluation infrastructure OpenAI has internally. Free. Open. Reproducible."*
>
> — Built solo from Tashkent · MIT licensed · Available for strategic conversations.
