[< Back to the TPS Toolkit](./README.md)

# TPS User Adoption Guidance

This document provides a comprehensive guide for integrating the TeeZe Prompting System (TPS) into your workflows, from individual use to enterprise-level deployment. It is intended for users who understand the basics of the [TPS Methodology](../TPS-MethodologyREADME.md) and are ready to apply the system in practical, scalable ways.

---

## 1. Foundational Guidance: How to Get Started

Whether you are a single user or a team lead, we recommend a structured progression to master TPS.

#### Individual Adoption Path
1.  **Understand the Methodology:** Begin by reviewing the `TPS Methodology` to internalize the core concepts of the three Tiers.
2.  **Start with Tier 1:** Use the `Tier 1` templates from the Toolkit for your daily, simple AI requests. This builds the habit of structured prompting.
3.  **Advance to Tier 2:** When a task requires multiple steps or a specific output, use a `Tier 2` template. This is ideal for managing small projects.
4.  **Explore with Tier 3:** For ambiguous or creative challenges, engage with `Tier 3` to experience collaborative, iterative problem-solving with an AI.

#### For Experienced Practitioners
Seasoned users can bypass the structured progression and navigate directly to the Tier best suited for their task. The key is to adapt and refine the provided templates to your specific needs.

---

## 2. Advanced Strategies: Thinking with TPS

Once you are comfortable with the basics, you can leverage more sophisticated strategies.

#### Hybrid Interaction Models
Don't think of the Tiers as rigid categories. The most effective use of TPS often involves combining them:
*   **Tier 3 to Tier 2:** Start with an open-ended `Tier 3` brainstorming session to explore a new idea. Once a clear path emerges, switch to a `Tier 2` framework to systematically plan its execution.
*   **Tier 1 within Tier 2:** Use quick `Tier 1` prompts to accomplish smaller sub-tasks within a larger `Tier 2` project plan.

#### Scaling Interaction Sophistication
*   **Ascending Complexity:** A simple `Tier 1` query ("What are the main features of product X?") can evolve into a `Tier 2` project ("Create a competitive analysis of product X vs. its top 3 rivals.").
*   **Descending Complexity:** If a `Tier 2` project feels overwhelming ("Create a full marketing plan"), break it down into a series of smaller, manageable `Tier 1` tasks ("Write three headlines for the new ad campaign.").

---

## 3. The Building Blocks: Advanced Modular Components

For maximum precision, especially in `Tier 2` and `Tier 3` prompts, you can explicitly define these modular components:

*   **`Role Definition (RD)`:** Defines the AI's persona, expertise, and perspective. This is the single most powerful way to shape the quality of the output.
*   **`Constraint Definition (CD)`:** Sets specific rules, limitations, or requirements (e.g., tone, format, style guides, ethical boundaries).
*   **`Checkpoint Definition (CP)`:** Establishes points for review and feedback within a long-running task, preventing the AI from going too far in the wrong direction.

---

## 4. Implementation Scenarios: Deploying TPS in the Real World

TPS is designed to be deployed in a variety of contexts.

#### Business Applications
*   **Marketing:** Use `Tier 1` for rapid ad copy generation, `Tier 2` for creating detailed campaign strategies, and `Tier 3` for high-level brand visioning sessions.
*   **Data Analysis:** Use `Tier 1` for quick data retrieval queries, `Tier 2` for generating comprehensive reports from a dataset, and `Tier 3` for exploring data to uncover strategic insights.
*   **Software Development:** Use `Tier 1` for generating code snippets or debugging functions, `Tier 2` for architectural planning, and `Tier 3` for high-level system design exploration.

#### Technical Deployment
TPS can be integrated directly into your applications and automated workflows (e.g., using LangChain, n8n, or custom code).

1.  **Cloud/API-Based Interaction:**
    *   **Workflow:** A user interacts with your application. Your application's backend constructs a TPS-structured prompt (using a Tier template) based on the user's input and sends it to the LLM API.
    *   **Example:** A project management app could have a "Generate Project Plan" button. When clicked, it gathers project details from the user and inserts them into a `Tier 2` template before calling the AI.

2.  **Local/Agent-Based Integration:**
    *   **Workflow:** For autonomous agents or complex local applications, the **Master System Prompt** is loaded into the agent's memory at the beginning of its lifecycle.
    *   **Example:** A data curation agent is initialized with the `Master System Prompt`, customized with a "Data Curator" persona and a directive that all output must be valid JSON. This ensures every task it performs is guided by the full TPS framework.

---

## 5. The Role of the Master System Prompt

For any serious or continuous use of TPS, the **Master System Prompt** is the core engine. It primes the AI, making it fully "TPS-aware" for an entire session.

> The System Prompt is not just a template; it's a configuration file for the AI's "operating system." It loads the Moral Compass (EMF) and the definitions of all three Tiers into the AI's context.

By customizing the `Persona`, `Constraints`, and `Directives` in the System Prompt, you can create highly specialized and more reliable AI collaborators across different domains.

<p align="center">
  <a href="./TPS-System-Prompt-Template.md">
    <img src="https://img.shields.io/badge/View_the-Master_System_Prompt_Template-blue?style=for-the-badge" alt="Master System Prompt Template">
  </a>
</p>

---

<p align="center">
  Copyright 2025 TeeZe Solutions, LLC
  <br>
  Licensed under the <a href="http://www.apache.org/licenses/LICENSE-2.0">Apache License, Version 2.0</a>.
</p>
