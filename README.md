# Awesome Elixir AI [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> **Help us curate the higher-level AI stack for Elixir—PRs welcome!** See [Contributing](CONTRIBUTING.md) to add packages, examples, and learning resources.

A curated list of Elixir AI libraries, tools, frameworks, and resources for building production - ready agentic and LLM-driven applications on the BEAM.

## About the Swarm

The **Elixir AI Swarm Collective** advances the higher-level AI ecosystem for Elixir/BEAM—empowering developers who ship production-ready agentic and LLM-driven applications.

### What We Do

- **Curate** an awesome-list of packages that work seamlessly together
- **Educate** through tutorials, examples, and partnerships
- **Maintain** packages to ensure compatibility and ease of use
- **Share** production patterns and real-world examples
- **Support** developers via Discord discussions and office hours
- **Build** starter templates and integration guides
- **Showcase** monthly highlights of production AI applications
- **Fund** integration bounties for connecting to AI services

### How to Join

Want your package or content included? Simple PR to this awesome-list. If it helps developers build AI applications on Elixir, it belongs.

## Join the Community

- **Discord** — Home base for real-time discussion and support: https://discord.gg/9JAbhRRZ
- **GitHub** — [`agentjido`](https://github.com/agentjido) org for awesome-list, templates, and examples
- **X/Twitter** — [@agentjido](https://x.com/agentjido) for announcements and highlights
- **ElixirForum** — Monthly showcases and major announcements
- **Elixir Weekly** — Submit highlights for newsletter inclusion

## Featured Learning: Elixir Mentor

- **[Elixir Mentor YouTube](https://www.youtube.com/@ElixirMentor)** — Tutorials, deep dives, and monthly showcases focused on agentic AI with Elixir. Subscribe for expert content on building AI applications with Phoenix, LiveView, and the BEAM.

## Contents

- [Awesome Elixir AI ](#awesome-elixir-ai-)
  - [About the Swarm](#about-the-swarm)
    - [What We Do](#what-we-do)
    - [How to Join](#how-to-join)
  - [Join the Community](#join-the-community)
  - [Featured Learning: Elixir Mentor](#featured-learning-elixir-mentor)
  - [Contents](#contents)
  - [Ecosystem Map](#ecosystem-map)
  - [High-Level Agent Frameworks](#high-level-agent-frameworks)
  - [LangChain-Style Components](#langchain-style-components)
  - [LLM Clients \& SDKs](#llm-clients--sdks)
  - [RAG \& Embeddings](#rag--embeddings)
  - [Vector Databases \& Indexers](#vector-databases--indexers)
  - [Observability, Evaluation \& Guardrails](#observability-evaluation--guardrails)
  - [Data Ingestion \& ETL](#data-ingestion--etl)
  - [Speech \& Audio](#speech--audio)
  - [Vision \& Image Processing](#vision--image-processing)
  - [Evolutionary \& Genetic Algorithms](#evolutionary--genetic-algorithms)
  - [Starters, Templates \& Examples](#starters-templates--examples)
  - [Resources](#resources)
    - [Tutorials \& Learning](#tutorials--learning)
    - [Model Context Protocol (MCP)](#model-context-protocol-mcp)
    - [Community \& Ecosystem](#community--ecosystem)
  - [Contributing](#contributing)
  - [License](#license)

## Ecosystem Map

Quick overview of how the pieces fit together:

- **Build agents and orchestrations** → [High-Level Agent Frameworks](#high-level-agent-frameworks)
- **Call LLMs** → [LLM Clients & SDKs](#llm-clients--sdks)
- **Compose prompts, chains, tools, memory** → [LangChain-Style Components](#langchain-style-components)
- **Do RAG: chunk, embed, index, retrieve** → [RAG & Embeddings](#rag--embeddings), [Vector Databases](#vector-databases--indexers)
- **Observe, evaluate, and add guardrails** → [Observability & Evaluation](#observability-evaluation--guardrails)
- **Integrate with your data** → [Data Ingestion & ETL](#data-ingestion--etl)
- **Add speech and vision** → [Speech & Audio](#speech--audio), [Vision & Image Processing](#vision--image-processing)
- **Use starters and examples to ship faster** → [Starters & Templates](#starters-templates--examples)

## High-Level Agent Frameworks

*Build autonomous agents, workflows, and multi-agent systems.*

- [AshAi](https://github.com/ash-project/ash_ai) - Structured outputs, vectorization and tool calling for your Ash application with LangChain integration and MCP server capabilities.
- [Jido](https://github.com/agentjido/jido) - Framework for building autonomous, distributed agent systems with modular actions, stateful agents, and sensors. AI-framework agnostic.
- [LangChain](https://github.com/brainlid/langchain) - Framework for developing applications powered by language models, with support for OpenAI, Anthropic, Google, and Bumblebee models.
- [SwarmEx](https://github.com/nrrso/swarm_ex) - Lightweight library for AI agent orchestration with built-in telemetry and tool integration.

## LangChain-Style Components

*Prompts, chains, tools, memory, and structured outputs.*

- [Instructor.ex](https://github.com/thmsmlr/instructor_ex) - Structured outputs from LLMs using Ecto schemas. Works with OpenAI, llama.cpp and Bumblebee.
- [InstructorLite](https://github.com/martosaur/instructor_lite) - Lightweight structured outputs for LLMs using JSON schemas with multi-provider support including OpenAI, Anthropic, and Gemini.
- [Mentor](https://github.com/zoedsoupe/mentor) - Library for generating validated structured outputs from LLMs with automatic retries and schema validation.

## LLM Clients & SDKs

*Connect to LLM providers with unified or specialized clients.*

- [ExLLM](https://github.com/azmaveth/ex_llm) - Multi-provider LLM library with unified API for Anthropic, OpenAI, Gemini, Groq, Ollama, and more. Features streaming, cost tracking, and structured outputs.
- [Honeycomb](https://github.com/seanmor5/honeycomb) - Fast LLM inference service and library built on Elixir, Bumblebee, and EXLA with OpenAI API compatibility.
- [LLM Composer](https://github.com/doofinder/llm_composer) - An Elixir library for integrating and managing multiple LLM backends including OpenAI, Ollama, and Google Gemini.
- [Ollama-ex](https://github.com/lebrunel/ollama-ex) - Elixir client for Ollama API with support for completions, chat, tools, and function calling.
- [ReqLLM](https://github.com/agentjido/req_llm) - Composable LLM client built on Req. Plugin-based providers for Anthropic, OpenAI, Google, and more with typed data structures.

## RAG & Embeddings

*Retrieval Augmented Generation, chunking, and embedding pipelines.*

- [Rag](https://github.com/bitcrowd/rag) - Library for building Retrieval Augmented Generation (RAG) systems with support for vector stores like pgvector and chroma.
- [TextChunker](https://github.com/revelrylabs/text_chunker_ex) - Semantic text chunking library optimized for vector embedding and RAG applications.

## Vector Databases & Indexers

*Similarity search and vector storage for AI applications.*

- [ExFaiss](https://github.com/elixir-nx/ex_faiss) - Elixir front-end to Facebook AI Similarity Search (Faiss) for efficient similarity search and clustering of dense vectors.
- [pgvector-elixir](https://hex.pm/packages/pgvector) - Ecto type and helpers for pgvector. Use Postgres as your vector store.

## Observability, Evaluation & Guardrails

*Track, evaluate, and protect your AI applications.*

- [Evals](https://github.com/ash-project/evals) - Tool for evaluating AI language models on Elixir code generation with side-by-side model comparisons and automated testing.
- [Usage Rules](https://github.com/ash-project/usage_rules) - Tool for synchronizing LLM rules files with dependencies to prevent AI hallucinations and ensure consistent usage patterns.

## Data Ingestion & ETL

*Web crawling, data extraction, and preprocessing for AI pipelines.*

- [Crawly](https://github.com/elixir-crawly/crawly) - Powerful Elixir web crawler for building corpora and data extraction pipelines.
- [Explorer](https://github.com/elixir-explorer/explorer) - Series and dataframes for data exploration in Elixir. Essential for preprocessing and feature pipelines.
- [Floki](https://github.com/philss/floki) - HTML parser for extraction pipelines.

## Speech & Audio

*Text-to-speech, speech recognition, and audio processing.*

- [Membrane Framework](https://github.com/membraneframework/membrane_core) - Real-time multimedia processing framework. Great for TTS/STT pipelines and streaming audio applications.

## Vision & Image Processing

*Image processing, computer vision, and OCR for AI applications.*

- [Evision](https://github.com/cocoa-xu/evision) - OpenCV bindings for Elixir/Erlang with comprehensive computer vision capabilities.
- [NxImage](https://github.com/elixir-nx/nx_image) - Image processing in Nx for preprocessing and augmentation.
- [Vix](https://github.com/akash-akya/vix) - Fast image processing via libvips for preprocessing and augmentation.
- [YOLO](https://github.com/poeticoding/yolo_elixir) - Real-time object detection using YOLOv8 models with 38ms processing time and optional Rust NIF for performance.

## Evolutionary & Genetic Algorithms

*Evolution-based optimization and problem solving.*

- [Genex](https://github.com/seanmor5/genex) - Genetic Algorithms in Elixir. Simple library for evolutionary computing and optimization problems.

## Starters, Templates & Examples

*Get started quickly with pre-built templates and example applications.*

- [Livebook](https://livebook.dev/) - Write interactive and collaborative notebooks with integrations to databases, messaging, visualization and AI workflows.
- [Kino](https://github.com/livebook-dev/kino) - Render rich and interactive output in Livebook for building AI demos and explorations.

## Resources

### Tutorials & Learning

- **[Elixir Mentor YouTube](https://www.youtube.com/@ElixirMentor)** — Tutorials, deep dives, and showcases for AI with Elixir.
- **[Elixir Mentor Podcast](https://podcasts.apple.com/gr/podcast/elixir-mentor/id1710056466)** — Community interviews and project showcases.
- **[Livebook Notebooks](https://livebook.dev/)** — Interactive notebooks and SmartCells for AI use-cases.
- **[Genetic Algorithms in Elixir](https://pragprog.com/titles/smgaelixir/genetic-algorithms-in-elixir/)** — Book by Sean Moriarity on evolutionary computing in Elixir.

### Model Context Protocol (MCP)

*Connect AI assistants to Elixir services and documentation.*

- [Anubis MCP](https://github.com/zoedsoupe/anubis-mcp) - SDK for the Model Context Protocol (MCP) with support for multiple transport options (STDIO, HTTP/SSE, WebSocket).
- [HexDocs MCP](https://github.com/bradleygolden/hexdocs-mcp) - Enables semantic search of Elixir package documentation for AI assistants via Model Context Protocol (MCP).
- [MCP Proxy](https://github.com/tidewave-ai/mcp_proxy_elixir) - Proxy that connects STDIO-based MCP clients to HTTP-based Server-Sent Events (SSE) MCP servers.
- [Tidewave Phoenix](https://github.com/tidewave-ai/tidewave_phoenix) - AI-powered development assistant for Phoenix web applications that connects editor AI assistants to web framework runtime via MCP.

### Community & Ecosystem

- **[Discord](https://discord.gg/9JAbhRRZ)** — Home base for the Elixir AI Swarm Collective.
- **[agentjido GitHub Org](https://github.com/agentjido)** — Packages, templates, and examples.
- **[@agentjido on X/Twitter](https://x.com/agentjido)** — Announcements and highlights.
- **[ElixirForum AI Topics](https://elixirforum.com/)** — Monthly showcases and discussions.

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting a PR.

**Quick Guidelines:**

- Format: `[Name](link) - Description.`
- Keep entries alphabetized within each section
- Descriptions should be short, clear, and descriptive
- Start with a capital letter and end with a period
- Ensure packages are generally useful, actively maintained, and documented

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the Elixir AI Swarm Collective has waived all copyright and related or neighboring rights to this work.
