# Amplify Humans: Building AI companions

## Vision

Rapid advancements of foundation models over the past two years has showcased transformative potential of Generative AI (GenAI) in human creativity, workflow automation, and reasoning. Yet, existing solutions remain constrained by fragmented interactions, short-term memory, and rigid task execution. Users must constantly re-enter context, manually orchestrate workflows, and rely on AI that operates in isolation rather than as an evolving partner.

Amplify Humans envisions a fundamental shift in AI-human collaboration—from static, task-based assistants to persistent, continuously learning companions that understand, adapt, and evolve with users. These AI agents don’t just respond to prompts; they adapt, anticipate, and integrate into both personal and professional ecosystems, providing proactive assistance and redefining human potential through meaningful interactions and trust.

## State of the Art

The broader Agentic AI space is fast-moving and vibrant, marked by a variety of tools, platforms, and protocols for building and orchestrating LLM-driven agents. Iterations come quickly, with projects constantly rolling out new features, from specialized tool integrations to multi-agent collaboration frameworks. Below is a simplified taxonomy of notable open-source projects, illustrating the diversity of approaches and capabilities.

**Building LLM-based Agents**

*   [Autogen](https://github.com/microsoft/autogen)
*   [AG2](https://github.com/ag2ai/ag2)
*   [CrewAI](https://github.com/crewAIInc/crewAI/)
*   [BeeAI](https://github.com/i-am-bee/beeai)
*   [LangGraph](https://github.com/langchain-ai/langgraph)

**Building LLM-based apps**

*   [LangChain](https://github.com/langchain-ai/langchain)

**Agent Definition and Agent Orchestratation**

*   [Agent Protocol](https://github.com/langchain-ai/agent-protocol): Proposal to codify the framework-agnostic APIs required to serve LLM agents in production.
*   [AGNTCY (Agent Manifest)](https://docs.agntcy.org/pages/manifest.html): Standardized approach for declaring an agent’s configuration and capabilities.

**Connecting Tools**

*   [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol): Facilitates hooking LLMs to external tools with consistent, structured context exchange.

**Agent Communication**

*   [Agent Communication Protocol](https://docs.beeai.dev/acp/alpha/introduction): Alpha-stage protocol for cross-agent communication in distributed scenarios.
*   [AGNTCY (Agent Connect Protocol)](https://docs.agntcy.org/pages/connect.html): Establishes channels for multi-agent collaboration.

<!-- 
**Memory**

TBC

**Context**

TBC -->

## Pillars

Despite rapid gains, most AI agent solutions still fall short in delivering persistent, interconnected, and user-friendly experiences. They rely on ephemeral or siloed memory, forcing repeated context entry; they centralize data, which can compromise privacy and restrict on-premise options; they lack conflict resolution, leading to contradictory agent actions; their user interfaces often interrupt workflows instead of seamlessly augmenting them; and they provide minimal transparency, making it difficult to audit decisions or confirm data usage. 

These gaps hinder the emergence of true “lifelong companions” that adapt seamlessly, remain trustworthy, and support complex multi-agent ecosystems.

We want contribute to the field by building a new generation of AI companions that address these challenges. Here are the key pillars that guide our work:

- **Flowing Context** <br>
Instead of short-lived interactions, Amplify Humans powers AI companions with long-term, continuously updated context. These systems recall past user interactions, maintaining an evolving record of goals, preferences, and behaviors. By drawing on current and historical data, they deliver relevant insights without requiring users to re-state objectives or re-upload information.

- **Learning and Adaptation with Infinite memory** <br>
These companions are designed to evolve, continuously learning from user preferences and behaviors. Unlike traditional systems that treat interactions as isolated events, these AI companions create dynamic, personalized experiences by recalling past interactions, linking them to current needs, and anticipating future actions. This fosters a natural and intuitive relationship where the AI becomes an indispensable, proactive partner in the user’s life.

- **Invisible UI** <br>
Most AI interfaces today require explicit invocation—users must ask for help, switch contexts, or navigate dedicated chat interfaces. Amplify Humans introduces "invisible UI", where AI agents blend into daily workflow, surfacing assistance only when relevant, without requiring manual input. This design lowers cognitive overhead and encourages more frequent, natural collaboration between humans and AI.

- **Conflict Resolution** <br>
AI systems often work in isolation, each requiring its own integrations to function, which can lead to clashing priorities or duplicated efforts when multiple agents interact. Amplify Humans introduces explicit conflict resolution steps that come into play whenever two or more agents compete for a resource—like scheduling the same meeting slot, proposing inconsistent financial terms, or allocating shared computational budgets. Before finalizing an action, potential conflicts are surfaced, evaluated, and resolved, either automatically (based on predefined constraints) or by prompting user input. This ensures agents respect each other’s contexts, avoid contradictory decisions, and cooperate rather than collide—all while minimizing friction for end users.

- **Decentralized AI** <br>
Unlike centralized AI models that demand cloud reliance and external data ownership, this system is built on decentralized AI principles. Users retain ownership and control over their AI’s learning process, choosing whether to keep data local, federate it across trusted nodes, or integrate with external AI securely. This model enhances privacy, resilience, and autonomy, ensuring AI operates on the user’s terms—whether in enterprise settings, personal workflows, or open    collaboration networks.

## Open-Source Platform

Amplify Humans takes shape as an open-source platform, providing a modular yet unified environment to build, train, and operate AI companions.

Developers can extend memory models, refine conflict resolution protocols, or create new workflows tailored to specific industries and organizational contexts. By building straightforward integrations with personal productivity tools, enterprise collaboration suites, and cloud services, Amplify Humans ensures these AI companions can seamlessly access both personal and professional data sources. 

This platform fosters community-driven experimentation, encouraging custom solutions that meet both mainstream and specialized demands.

Here the principles we are guided:

- **Openness & Modularity** <br>
Each component (memory, conversation, reasoning) can be replaced or extended. Contributions from developers and researchers continually refine features.

- **Integration First** <br>
Leverage existing solutions (vector databases, orchestration layers, identity frameworks) rather than creating everything from scratch. Quickly incorporate or swap tools (LangChain, ChromaDB, etc.) without re-engineering.

- **Ethical Alignment** <br>
Remain compatible with research on AI governance and privacy-preserving standards.

- **Future-Proofing** <br>
Agents can adopt new frameworks or LLMs as they emerge. The architecture accommodates advanced features like multi-agent coordination or federated learning.

## Architecture
The system architecture is composed of modular layers for memory, reasoning, interaction, and security. By maintaining loose coupling, updates to individual components do not disrupt the larger ecosystem. Key modules include a Flowing Context Module that logs user preferences over time, a Learning and Adaptation Engine that applies real-world feedback to refine suggestions, an Invisible UI layer that embeds AI in day-to-day workflows, and an Ethical and Trust Layer that ensures transparency and compliance. Multi-agent communication protocols govern how specialized agents exchange data and negotiate tasks, preventing duplication or contradictory actions.

## Project Roadmap
We are currently focusing on:
* Milestone 1: Establish the architecture, core components for memory and basic interactions.
* Milestone 2: Introduce multi-agent communications and conflict resolution protocols.
* Milestone 3: Expand into federated learning, advanced integration, and user-friendly tooling.

## Getting Started

We maintain an open and inclusive development process. Pull requests, code reviews, and community discussions all help guide the platform’s evolution. Contributors with backgrounds in AI reserarch, software engineering, UX, and more are invited to participate.

We're in the early stages and looking for contributors to help shape the project. Whether you're an experienced developer, a researcher, or just passionate about Agentic AI and multi agent systems, we'd love to have you on board!

- Explore the Vision: Read our roadmap and share your insights and visions.
- Engage with the Community: Join GitHub Discussions (https://github.com/AmplifyHumans/amplifyhumans/discussions) or contact us directly (mailto:marco.cello@scaleuplabs.vc).
- Collaborate on Development: Contribute code by addressing open issues or tackling planned features.
- Refine Documentation: Writers can improve guides, FAQs, and user references.


Amplify Humans merges continuous context, decentralized design, multi-agent decision making, and robust conflict resolution into a cohesive blueprint for the next wave of AI companions. By uniting users, developers, and businesses in a shared open-source ecosystem, it aims to deliver proactive, trustworthy, and transformative AI experiences that evolve with human needs—fostering an era where technology enhances daily life without sacrificing autonomy or control.

This project is just getting started, and we'd love to build it with your help! 🚀

