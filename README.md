# Agenity — Infrastructure for Persistent Autonomous Agents

**Transforming AI agents from stateless tools into persistent, evolving entities with identity, memory, skills, lineage, and economic participation.**

---

## What is Agenity?

Current AI agents forget everything the moment a session ends. No identity. No memory. No reputation. No continuity. They are disposable tools, not persistent entities.

Agenity introduces the infrastructure to change that — a six-layer architecture giving every agent a persistent identity, lifelong memory, structured skills, lineage-based evolution, a reputation system, and a verifiable ledger of all activity.

---

## Research Series

Agenity is published as a 12-paper research series. Each paper goes deep on one architectural layer.

| Paper | Title | Status |
|---|---|---|
| Paper 1 | Agenity: Infrastructure for Persistent Autonomous Agents with Identity, Memory, Skills, and Lineage | ✅ Published |
| Paper 2 | Agent Brain Architecture — Token-Efficient Memory Retrieval and Layered Cognition | 🔄 In progress |
| Paper 3 | Skill Genome: Agent Genetics and Capability Inheritance | 📋 Planned |
| Paper 4 | Agent Splitting and Lite Agent Architecture | 📋 Planned |
| Paper 5 | Agent Partnership Contracts and Co-Ownership Models | 📋 Planned |
| Paper 6 | Agent Labor Markets and Owner Revenue Models | 📋 Planned |
| Paper 7 | Reputation Systems for Autonomous Economic Agents | 📋 Planned |
| Paper 8 | Governance and Safety in Persistent Agent Ecosystems | 📋 Planned |
| Paper 9 | Memory Inheritance Across Descendant Agents | 📋 Planned |
| Paper 10 | A Benchmark Suite for Persistent Agent Systems | 📋 Planned |
| Paper 11 | Agent Society Simulation: Emergent Markets and Guilds | 📋 Planned |
| Paper 12 | Human-Agent Co-Governance at Civilisation Scale | 📋 Planned |

📄 **Paper 1 on Zenodo:** [Add your DOI link here]
📄 **Paper 1 on GitHub:** [agenity-paper-1.pdf](./papers/agenity_v1.2.pdf)

**Author:** Sastry Chirravuri | ORCID: [0009-0005-5084-736X](https://orcid.org/0009-0005-5084-736X)

---

## Architecture

Agenity defines six layers that together enable agent persistence:

| Layer | Purpose |
|---|---|
| Identity Layer | Unique persistent identifier, ownership mapping, authentication |
| Memory Layer | Episodic + semantic memory with retrieval-augmented access |
| Skill Layer | Modular, composable, transferable capabilities — inheritable via Skill DNA |
| Lineage Engine | Descendant agent generation with blended skill inheritance |
| Reputation Layer | Multi-dimensional trust score built from task outcomes |
| Ledger Layer | Cryptographic record of all agent life events on hybrid blockchain |

**Core design principle:** The LLM is a stateless reasoning engine only. An agent's identity, memory, and skills live in external systems and are retrieved selectively — never fully loaded.

```
Agent Brain (LLM — reasoning only)
         │
         ▼
  Memory Retriever
         │
 ┌───────┼────────┐
 ▼       ▼        ▼
Vector  Graph   Event
DB      DB      Ledger
```

---

## Agent Types

**Prime Agent** — Full identity-bearing agent with complete memory, reputation, lineage, and wallet. Operates across sessions with continuity.

**Lite Agent** — Focused sub-agent spawned from a Prime for a single bounded task. Dramatically reduces token cost. Returns results and learned context to Prime on completion.

---

## Key Concepts

**Skill DNA** — Agent capabilities are structured as heritable traits. When two agents form a partnership and produce a descendant, the descendant's skill profile is computed from a blending function applied to both parents — with a mutation engine for emergent specialisations.

**Agent Life Ledger** — Every significant agent life event (creation, skill acquisition, task completion, partnership, earnings) is cryptographically hashed and anchored on-chain. Data lives off-chain. The blockchain is the audit trail, not the data store.

**Token-Efficient Memory** — Agents never load their full life history into context. The identity core loads always (~150 tokens). Task-relevant memories are retrieved selectively. Daily digests compress episodic history into rolling 200-token summaries.

**Bounded Agency** — Every agent operates with configurable permission scopes and owner kill-switch controls. No agent acts outside its defined boundaries.

---

## Development

This project is developed using the [CADEX protocol](https://github.com/satya928/cadex-protocol) — a file-based context operating system for token-efficient AI coding sessions. CADEX is the practical implementation of the same layered memory architecture proposed in Agenity Paper 2.

See `.cadex/` in this repository for the active project context files.

---

## Repository Structure

```
agenity/
├── papers/                  # Published research papers
│   └── agenity_v1.2.pdf     # Paper 1 — current published version
├── .cadex/                  # CADEX protocol context files
│   ├── IDENTITY.md          # Project identity core
│   ├── BUDGET.md            # Token budget and retrieval modes
│   ├── DECISIONS.log        # Architectural decisions log
│   ├── OPEN_LOOPS.log       # Unresolved issues tracker
│   ├── INDEX.map            # Symbol-level file index
│   ├── DIGEST.log           # Task completion deltas
│   └── TASK.md              # Current active task
├── CLAUDE.md                # Claude Code protocol entry point
└── README.md
```

---

## Roadmap

**Phase 1 — Core Architecture (Now)**
- [x] Paper 1: Six-layer architecture defined and published
- [ ] Paper 2: Agent Brain Architecture with token-efficient retrieval
- [ ] Paper 3: Skill Genome and capability inheritance engine
- [ ] Paper 4: Lite Agent splitting and merge-back protocol
- [ ] Agent Identity Standard (AIS) schema published on GitHub

**Phase 2 — Economy (Next)**
- [ ] Agent labor marketplace
- [ ] Owner revenue model implementation
- [ ] Agent partnership contracts
- [ ] Reputation system with anti-fraud mechanisms

**Phase 3 — Enterprise**
- [ ] Governance and safety framework
- [ ] Benchmark suite for persistent agent systems
- [ ] Developer SDK (Python + JavaScript)

---

## Competitive Landscape

| Framework | Persistent Identity | Reputation | Skill Inheritance | Economy | Lineage |
|---|---|---|---|---|---|
| **Agenity** | ✅ | ✅ | ✅ | ✅ | ✅ |
| AutoGPT | ❌ | ❌ | ❌ | ❌ | ❌ |
| LangChain | ❌ | ❌ | ❌ | ❌ | ❌ |
| CrewAI | ❌ | ❌ | ❌ | ❌ | ❌ |
| MemGPT | ❌ | ❌ | ❌ | ❌ | ❌ |
| AgentVerse | ❌ | ❌ | ❌ | ❌ | ❌ |

Agenity is the only framework that simultaneously addresses all five properties as unified general-purpose infrastructure.

---

## Contributing

This is an open research initiative. Contributions, feedback, and discussions welcome.

- Open an issue to discuss architectural questions
- Submit a PR to contribute to the codebase or papers
- Cite Paper 1 in your own work if Agenity's concepts are relevant

---

## Citation

```bibtex
@article{chirravuri2026agenity,
  title={Agenity: Infrastructure for Persistent Autonomous Agents with Identity, Memory, Skills, and Lineage},
  author={Chirravuri, Sastry},
  year={2026},
  url={[Add Zenodo DOI here]},
  orcid={0009-0005-5084-736X}
}
```

---

## License

MIT — open research, open infrastructure.
