# resume_portfolio
My 6 months portfolio, exploring the world of Agentic AI and it's used cases. Using my background in human patterns (Bachelor of Psychology), operational systems, and developed skills in AI Prompting, my current directive is to build working digital ecosystems.

This is my digital master architecture blueprint to design my very first digital ecosystem, by building a Autonomous AI Helpdesk Triage


# 🛡️ Autonomous AI Helpdesk Triage Orchestrator

This repository contains the architecture and core implementation files for a multi-agentic AI ecosystem designed to automate helpdesk support workflows. The system is built not just to "chat," but to take robust, reliable operational action that protects SLAs and reduces manual data entry.

## 🚀 The Core Business Problem

Manual support triage is expensive and prone to bottlenecks and SLA breaches. Generic chatbots lack the governance and logic to route requests effectively. This project builds the orchestration layer that connects advanced language reasoning to existing helpdesk tools and knowledge repositories.

## 🛠️ System Architecture

![Alt Text](resume_portfolio/TicketingTriageFramework.png "Ticketing Triage Framework")

![Alt Text](resume_portfolio/Updated_by_Gemini-Refined_Knowledge_Interface_to_The_Framework.png.png "Framework Sketches")

The ecosystem operates through specialized agents working in sync:

1.  **Incoming Data Stream:** Receives raw support text.
2.  **Intent Classification:** Instantly detects urgency (validity, complaint type) using a tailored **Thoughtful Agent Persona**.
3.  **Dynamic Routing:** Based on classification, data is directed to either:
    *   **Live Agent Layer:** Where an **AI Assistant** provides smart reply templates, suggestions, and S-curve prediction.
    *   **Automated Action Layer:** Where a **File Sorter Agent** processes data, and a **Teacher/Expert Agent (RAG)** provides automated root-cause analysis based on a validated **Knowledge Base**.
4.  **Governance Layer:** An external algorithmic **Watchdog** script (for loop prevention) and a Hallucination Prevention layer run parallel to all processes to ensure stability and adherence to SLA metrics.

## ⚙️ Key Technical Features Demonstrated

*   **Agentic Orchestration:** Structured multi-agent cooperation using [CrewAI/LangChain].
*   **SLA Governance:** Independent watchdog script with countdown logic and escalation triggers.
*   **RAG Implementation:** Specialized data retriever and reasoning agent accessing a searchable knowledge index.
*   **Production Guardrails:** Explicit error handling and loop prevention protocols.

## 📁 Repository Structure

```text
/config/agents.yaml       # AI Agent Personas defined
/config/tasks.yaml        # Multistep workflow logic
/src/
    main_router.py       # The central orchestrator (your 'Routing' block)
    watchdog.py          # SLA tracker & loop prevention
    expert_agent.py      # RAG-driven helpdesk analyst
/requirements.txt        # Required python packages
