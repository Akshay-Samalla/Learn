# AI Engineer Roadmap

Foundations to production: 147 topics across 17 phases, about 48 weeks at 12-15 hrs/week. Tick topics as you finish; progress saves in this browser.

**AI / LLM Engineer**P3-P6, P10-P14

**Agentic Developer**P4, P6-P9, P11-P14

**ML / MLOps Engineer**P1-P2, P10, P13-P14

**AI Data Engineer**P0, P5-P6, P13-P14

0Foundations4 wks · 0%

Engineering basics every AI role assumes.

- [ ] **Python core** *Must*types, OOP, dataclasses, generators, errors · \~15h
- [ ] **Async Python** *Must*asyncio, httpx, concurrency, rate limits · \~6h
- [ ] **Python tooling** *Must*venv/uv, pytest, typing, ruff, pydantic · \~6h
- [ ] **Git & GitHub** *Must*branching, PRs, rebase, Actions CI, README craft · \~6h
- [ ] **Linux & CLI** *Should*bash, curl, env vars, ssh, make · \~4h
- [ ] **APIs & JSON** *Must*REST, OAuth/JWT, pagination, webhooks, OpenAPI · \~6h
- [ ] **SQL & databases** *Must*joins, indexes, window functions, Postgres, ORM, NoSQL · \~12h
- [ ] **NumPy & Pandas** *Must*arrays, broadcasting, groupby, merge, cleaning · \~8h
- [ ] **Math for ML** *Should*linear algebra, probability, statistics, gradients · \~10h

**Free resources:** CS50P, Real Python, Pro Git book, SQLBolt, Kaggle Pandas\
**Build:** FastAPI + Postgres CRUD service on GitHub with CI

1Machine Learning Basics3 wks · 0%

Classic ML intuition: data, models, metrics.

- [ ] **ML workflow** *Must*problem framing, split, train, evaluate, iterate · \~4h
- [ ] **Supervised learning** *Must*regression, classification, trees, XGBoost · \~10h
- [ ] **Unsupervised learning** *Should*clustering, PCA, anomaly detection · \~5h
- [ ] **sklearn pipelines** *Must*preprocessing, ColumnTransformer, tuning · \~6h
- [ ] **Metrics** *Must*precision, recall, F1, ROC-AUC, confusion matrix · \~4h
- [ ] **Overfitting & validation** *Must*bias-variance, cross-validation, data leakage · \~4h
- [ ] **Feature engineering & data quality** *Should*encoding, missing data, drift basics · \~5h
- [ ] **Experiment tracking** *Should*MLflow or Weights & Biases · \~3h

**Free resources:** Andrew Ng ML Specialization, scikit-learn docs, StatQuest\
**Build:** Churn or price prediction with sklearn pipeline + MLflow

2Deep Learning3 wks · 0%

How neural nets learn; get PyTorch-comfortable.

- [ ] **Neural networks** *Must*neurons, layers, activations, loss functions · \~5h
- [ ] **Backpropagation & gradient descent** *Must*chain rule, SGD, Adam, learning rates · \~6h
- [ ] **PyTorch** *Must*tensors, autograd, Dataset/DataLoader, training loop · \~10h
- [ ] **CNNs** *Should*convolutions, pooling, image classification · \~5h
- [ ] **RNN / LSTM** *Nice*sequence modeling and why transformers replaced them · \~3h
- [ ] **Training craft** *Should*dropout, batchnorm, schedulers, mixed precision · \~5h
- [ ] **Transformers intro** *Must*attention, encoder vs decoder, positional encoding · \~6h
- [ ] **GPU basics** *Should*Colab/Kaggle GPUs, memory, batch sizing · \~3h

**Free resources:** Karpathy Zero to Hero, fast.ai, PyTorch tutorials, 3Blue1Brown\
**Build:** Train a small CNN, then a tiny GPT (nanoGPT style)

3LLM Fundamentals3 wks · 0%

Understand what is inside the model you call.

- [ ] **Tokens & tokenization** *Must*BPE, tiktoken, token cost, multilingual gotchas · \~4h
- [ ] **Embeddings** *Must*meaning as vectors, cosine similarity · \~4h
- [ ] **Transformer architecture** *Must*blocks, residuals, layer norm, decoder-only · \~6h
- [ ] **Self-attention** *Must*Q/K/V, multi-head, complexity, flash attention idea · \~5h
- [ ] **Next-token prediction & decoding** *Must*temperature, top-p, top-k, greedy, beam · \~3h
- [ ] **Context window & KV cache** *Must*limits, long-context trade-offs, lost in the middle · \~3h
- [ ] **Pre-training, SFT, RLHF/DPO** *Must*how base models become assistants · \~5h
- [ ] **LLM vs SLM vs LRM vs VLM** *Must*sizes, reasoning models, multimodal, when to use which · \~4h
- [ ] **Hallucination causes** *Must*knowledge gaps, sycophancy, mitigation overview · \~2h
- [ ] **Provider APIs & model choice** *Must*Claude, OpenAI, Gemini, Azure OpenAI, open-weights, pricing · \~5h

**Free resources:** Hugging Face LLM Course, Karpathy Let us build GPT, Anthropic and OpenAI docs\
**Build:** Token/cost calculator + side-by-side model comparison script

4Prompting & Structured Outputs2 wks · 0%

Reliable, testable prompts that return machine-readable results.

- [ ] **Prompt patterns** *Must*zero/few-shot, role, delimiters, examples · \~4h
- [ ] **Reasoning prompting** *Must*chain-of-thought, extended thinking, when not to · \~3h
- [ ] **System prompts & instruction hierarchy** *Must*roles, constraints, tone, refusal handling · \~3h
- [ ] **Structured outputs** *Must*JSON schema, Pydantic, Instructor, constrained decoding · \~5h
- [ ] **Prompt programming** *Should*DSPy, automatic prompt optimization · \~4h
- [ ] **Prompt versioning & testing** *Must*prompt registry, regression sets · \~3h
- [ ] **Prompt caching** *Must*cache prefixes to cut cost and latency · \~2h
- [ ] **Streaming responses** *Must*token streaming, partial JSON, UX · \~3h

**Free resources:** Anthropic prompt docs, DeepLearning.AI prompt courses, DSPy docs\
**Build:** Invoice/ticket extractor returning validated JSON

5Embeddings, Vector DBs & RAG3 wks · 0%

Ground LLMs in your own data.

- [ ] **Embedding models** *Must*choosing models, dimensions, multilingual, fine-tuned embeddings · \~4h
- [ ] **Chunking strategies** *Must*fixed, semantic, hierarchical, overlap, metadata · \~4h
- [ ] **Vector databases** *Must*FAISS, Chroma, pgvector, Qdrant, Pinecone, Azure AI Search · \~6h
- [ ] **ANN indexing** *Should*HNSW, IVF, quantization, recall vs latency · \~3h
- [ ] **Hybrid search** *Must*BM25 + vector, reciprocal rank fusion · \~3h
- [ ] **Rerankers** *Must*cross-encoder, ColBERT, LLM reranker · \~4h
- [ ] **Basic RAG pipeline** *Must*ingest, retrieve, augment, generate, cite · \~6h
- [ ] **Document parsing** *Must*PDF/OCR/tables, Unstructured, layout-aware · \~4h
- [ ] **RAG evaluation** *Must*faithfulness, context precision/recall, answer relevance · \~4h
- [ ] **Fine-tuning vs RAG** *Must*decision framework and combined use · \~2h

**Free resources:** LangChain/LlamaIndex docs, Pinecone and Qdrant learn, Azure AI Search docs, Ragas docs\
**Build:** Doc Q&A with hybrid search, reranker, citations

6Advanced RAG3 wks · 0%

Make retrieval smarter, safer and cheaper.

- [ ] **Query transformation** *Must*rewriting, multi-query, HyDE, step-back · \~3h
- [ ] **Agentic RAG** *Must*agent decides when/what/where to retrieve, self-correct · \~5h
- [ ] **GraphRAG & knowledge graphs** *Should*entities, relations, Neo4j, community summaries · \~6h
- [ ] **Long-context vs RAG** *Must*when to stuff context vs retrieve · \~2h
- [ ] **Context compression** *Should*summarize, prune, LLMLingua-style compression · \~3h
- [ ] **Metadata filtering & access control** *Must*multi-tenancy, per-user ACLs, data security · \~4h
- [ ] **Text-to-SQL** *Should*schema grounding, validation, safe execution · \~5h
- [ ] **Multimodal RAG** *Nice*images, tables, charts, ColPali-style retrieval · \~4h

**Free resources:** LlamaIndex advanced guides, Microsoft GraphRAG repo, Neo4j GraphAcademy\
**Build:** GraphRAG or agentic RAG over a messy knowledge base

7Tool Calling, MCP & Protocols2 wks · 0%

Connect models to the real world.

- [ ] **Function & tool calling** *Must*schemas, parallel calls, forced tool choice · \~4h
- [ ] **Tool design** *Must*clear names, error messages, idempotency, pagination · \~3h
- [ ] **MCP fundamentals** *Must*servers, clients, resources, prompts, tools, transports · \~5h
- [ ] **Build an MCP server** *Must*Python/TypeScript SDK, auth, remote servers · \~6h
- [ ] **A2A (Google)** *Should*agent-to-agent protocol, agent cards · \~3h
- [ ] **IBM ACP** *Nice*agent communication protocol and how it compares · \~2h
- [ ] **Computer/browser tools** *Should*sandboxed execution, code interpreter patterns · \~3h

**Free resources:** MCP docs and SDKs, Anthropic tool use docs, A2A spec, OpenAI function calling guide\
**Build:** Custom MCP server exposing Azure/DevOps tools

8AI Agents & Agentic Workflows4 wks · 0%

Design agents that finish tasks reliably.

- [ ] **Workflow vs agent patterns** *Must*chaining, routing, parallelization, orchestrator-workers, evaluator-optimizer · \~5h
- [ ] **ReAct & planning loops** *Must*reason-act-observe, plan-and-execute, reflection · \~5h
- [ ] **LangChain** *Must*LCEL, retrievers, tools, callbacks · \~5h
- [ ] **LangGraph** *Must*state, nodes, edges, checkpoints, streaming, persistence · \~8h
- [ ] **Other frameworks** *Should*OpenAI Agents SDK, Claude Agent SDK, CrewAI, Microsoft Agent Framework · \~6h
- [ ] **Agent memory types** *Must*short-term, long-term, episodic, semantic, working, procedural · \~5h
- [ ] **Multi-agent systems** *Must*supervisor, swarm, handoffs, shared state · \~6h
- [ ] **Human-in-the-loop** *Must*approvals, interrupts, escalation, review queues · \~3h
- [ ] **Context engineering** *Must*what to load, trim, summarize, persist per step · \~4h
- [ ] **Harness, graph & loop engineering** *Must*the loop inside the graph inside the harness · \~5h
- [ ] **Agent reliability** *Must*timeouts, retries, loop limits, idempotent actions, cost caps · \~4h

**Free resources:** Anthropic Building Effective Agents, LangChain Academy, OpenAI Agents SDK docs, Claude Agent SDK docs\
**Build:** Multi-agent ticket triage with human approval (LangGraph)

9Agentic Dev Kit & AI-Assisted Engineering2 wks · 0%

Work 5x faster with agentic coding tools and ship your own.

- [ ] **Claude Code fundamentals** *Must*install, permissions, plan mode, workflows · \~4h
- [ ] **CLAUDE.md / AGENTS.md** *Must*project memory and conventions · \~2h
- [ ] **Skills** *Must*packaged instructions and scripts loaded on demand · \~3h
- [ ] **Hooks** *Must*pre/post tool automation, guardrails, formatting · \~3h
- [ ] **Subagents** *Must*parallel specialists with isolated context · \~3h
- [ ] **Plugins & MCP in Claude Code** *Should*bundle commands, skills, MCP servers · \~3h
- [ ] **Headless mode & CI** *Should*run agents in GitHub Actions for review/triage · \~3h
- [ ] **Reviewing AI-written code** *Must*tests first, diffs, security review, spec-driven dev · \~3h

**Free resources:** Claude Code docs, Anthropic Skills repo, MCP registry\
**Build:** A reusable plugin: CLAUDE.md + skills + hooks + subagent

10Fine-Tuning & Model Customization3 wks · 0%

Customize small models when prompting and RAG are not enough.

- [ ] **When to fine-tune** *Must*decision tree: prompt, RAG, fine-tune, distill · \~2h
- [ ] **Dataset curation** *Must*cleaning, formats, synthetic data, dedup, splits · \~6h
- [ ] **Hugging Face ecosystem** *Must*transformers, datasets, Hub, Spaces · \~6h
- [ ] **LoRA / QLoRA / PEFT** *Must*adapters, ranks, merging · \~8h
- [ ] **Training with TRL / Unsloth** *Should*SFT trainer, hyperparameters, GPU limits · \~6h
- [ ] **Preference tuning** *Nice*DPO, RLHF overview, reward models · \~4h
- [ ] **Distillation & small models** *Should*teacher-student, SLM deployment · \~3h
- [ ] **Quantization** *Should*GGUF, AWQ, GPTQ, quality vs speed · \~3h

**Free resources:** Hugging Face courses, Unsloth notebooks, TRL docs, Sebastian Raschka LLM book\
**Build:** LoRA fine-tune of a small model for ticket classification

11Evaluation & Quality3 wks · 0%

If you cannot measure it, you cannot ship it.

- [ ] **Eval metrics that matter** *Must*task success, accuracy, tool accuracy, latency, cost, groundedness, safety, human intervention rate · \~4h
- [ ] **Golden datasets** *Must*build from real traffic, edge cases, versioning · \~5h
- [ ] **Classic text metrics** *Should*BLEU, ROUGE, BERTScore and their limits · \~2h
- [ ] **LLM-as-judge** *Must*G-Eval, rubrics, juries, bias and calibration · \~5h
- [ ] **Agent evaluation** *Must*trajectory, multi-turn, tool-call correctness · \~5h
- [ ] **Safety & hallucination evals** *Must*groundedness checks, red-team sets · \~3h
- [ ] **Eval tooling** *Must*LangSmith, Promptfoo, DeepEval, Ragas, Braintrust · \~5h
- [ ] **Online evals & CI gating** *Must*regression tests on every prompt/model change · \~4h
- [ ] **Human evaluation** *Should*annotation guidelines, inter-rater agreement · \~2h

**Free resources:** DeepLearning.AI eval courses, Hamel Husain evals posts, Promptfoo, DeepEval, Ragas, LangSmith docs\
**Build:** Eval harness with golden set, LLM judge and CI quality gate

12Guardrails, Safety & Security2 wks · 0%

Protect users, data and your company.

- [ ] **Guardrail layers** *Must*input, output, topic, format, tool-level checks · \~4h
- [ ] **Prompt injection** *Must*direct, indirect, data exfiltration, defenses · \~5h
- [ ] **OWASP LLM Top 10** *Must*threat modeling for LLM apps · \~3h
- [ ] **PII & data privacy** *Must*redaction, retention, secrets handling · \~3h
- [ ] **Red teaming & jailbreaks** *Should*adversarial testing, automated attack suites · \~4h
- [ ] **Least privilege for agents** *Must*tool permissions, sandboxes, approval gates · \~3h
- [ ] **Moderation APIs** *Should*content safety classifiers · \~2h
- [ ] **Compliance & responsible AI** *Should*GDPR, EU AI Act, SOC 2, audit trails · \~3h

**Free resources:** OWASP LLM Top 10, Guardrails AI, NeMo Guardrails, Azure AI Content Safety docs\
**Build:** Guardrail layer + red-team test suite for your agent

13Deployment & Serving3 wks · 0%

Ship models and agents as reliable services (your cloud edge).

- [ ] **FastAPI for LLM apps** *Must*async endpoints, dependency injection, validation · \~6h
- [ ] **Streaming APIs** *Must*SSE and WebSockets for token streaming · \~3h
- [ ] **Docker** *Must*images, compose, multi-stage builds, slim images · \~5h
- [ ] **Kubernetes & container platforms** *Should*AKS, Azure Container Apps, autoscaling · \~8h
- [ ] **Managed AI platforms** *Must*Azure AI Foundry/OpenAI, AWS Bedrock, Vertex AI · \~8h
- [ ] **Self-hosting** *Should*Ollama vs vLLM vs SGLang, when each wins · \~6h
- [ ] **GPU inference** *Should*batching, KV cache, paged attention, throughput · \~5h
- [ ] **Async jobs & queues** *Must*Celery, Redis, Service Bus, retries, dead letters · \~5h
- [ ] **IaC & CI/CD** *Must*Terraform/Bicep, GitHub Actions, environments, secrets · \~6h

**Free resources:** FastAPI docs, Docker docs, Microsoft Learn AI Foundry, vLLM docs, Ollama docs, AWS Bedrock workshop\
**Build:** Containerized RAG/agent API on Azure Container Apps with CI/CD

14Production AI & LLMOps3 wks · 0%

Run AI systems at scale: observe, optimize, govern.

- [ ] **Observability & tracing** *Must*Langfuse, LangSmith, OpenTelemetry spans · \~6h
- [ ] **Cost & token optimization** *Must*prompt trimming, smaller models, batching, budgets · \~4h
- [ ] **Caching** *Must*prompt caching, semantic cache, response cache · \~3h
- [ ] **Latency optimization** *Must*streaming, parallel calls, speculative approaches, model choice · \~3h
- [ ] **Resilience** *Must*retries, fallbacks, model routing, rate-limit handling · \~4h
- [ ] **Versioning** *Must*prompts, models, datasets, rollback · \~3h
- [ ] **Feedback loops & data flywheel** *Must*thumbs, corrections, mining failures into evals · \~3h
- [ ] **A/B and shadow testing** *Should*safe rollouts, canaries, offline replay · \~3h
- [ ] **Drift & human intervention rate** *Must*monitor quality over time, escalation analytics · \~3h
- [ ] **Governance & incident response** *Should*audit logs, SLOs, runbooks, postmortems · \~3h

**Free resources:** Langfuse docs, OpenTelemetry docs, Chip Huyen AI Engineering, Eugene Yan blog\
**Build:** Observability + cost dashboard for your agent in Langfuse

15Automation, Multimodal & Specializations2 wks · 0%

Broaden into high-demand use cases; pick one to go deep.

- [ ] **Workflow automation** *Should*n8n, Zapier, Make, webhooks, triggers · \~4h
- [ ] **Chat integrations** *Should*Slack/Teams bots, email agents · \~4h
- [ ] **Voice agents** *Nice*STT, TTS, realtime APIs, turn-taking · \~6h
- [ ] **Vision & document AI** *Should*VLMs, OCR, invoices, forms · \~5h
- [ ] **Browser & computer-use agents** *Nice*web automation, sandboxing · \~4h
- [ ] **Coding agents** *Should*repo navigation, tests, PR automation · \~4h
- [ ] **Data & analytics agents** *Should*NL to SQL/BI, notebooks, charts · \~4h
- [ ] **Pick a specialization** *Must*choose one, build depth, write it up · \~6h

**Free resources:** n8n docs, LiveKit/Pipecat docs, Whisper docs, browser-use docs\
**Build:** One specialization demo (voice, docs, data or coding agent)

16Capstone, System Design & Career3 wks · 0%

Prove it, package it, get hired. Runs alongside earlier phases.

- [ ] **Portfolio projects** *Must*3 to 4 deployed projects with READMEs, demos, evals · \~30h
- [ ] **GitHub portfolio** *Must*pinned repos, architecture diagrams, tests, CI badges · \~5h
- [ ] **ATS-friendly resume** *Must*impact bullets with metrics, keywords, AI project framing · \~4h
- [ ] **LLM system design** *Must*design RAG/agent/chat systems with trade-offs · \~8h
- [ ] **Interview question bank** *Must*RAG, embeddings, MCP, tool calling, memory, evals, guardrails, latency · \~10h
- [ ] **Mock interviews** *Must*coding, system design, project deep-dive, behavioral · \~8h
- [ ] **Open source & community** *Nice*small PRs, blog posts, talks · \~6h
- [ ] **Role mapping** *Must*AI/LLM Engineer, Agentic Developer, ML/MLOps, AI Data Engineer · \~2h

**Free resources:** Chip Huyen book, ByteByteGo, Interviewing.io, LinkedIn, GitHub\
**Build:** Flagship end-to-end production agent app + 3 polished repos

**How to use:** go in order, but build the phase project before moving on. Phases 10-14 are what separate demo builders from production engineers. Run Phase 16 alongside everything else.