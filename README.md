Agentic OS: Sales & Auditor Architecture 🛡️
A system of autonomous AI agents based on the concept of "Embodied Intelligence" – a digital representation of real business processes (from logistics to finance) with strict adherence to operational logic and security standards (inspired by ISO 27001).
🏗️ System Architecture (Dual-Agent Separation of Duties)
The system eliminates AI hallucinations and the risk of promising "fiction" to clients through strict role division. Agents do not communicate via free-flowing text, but through structured forms (Atomic Payload).
1. Front-end Agent ("The Salesman / Customer Friend")
Role: Polite, empathetic conversational interface for the customer.
Goal: Understanding customer intent and extracting data into a structured Rich Sales Order (RSO) form.
Constraints: No database access, no decision-making authority. Systemically isolated from the core business logic.
2. Back-end Agent ("The Cold Analyst")
Role: Rigorous process auditor.
Goal: Verifying the RSO based on Standard Operating Procedures (SOP) and validating resources (Supply Management / Credit Check).
Constraints: No direct customer contact. Receives data strictly in "Read-only" mode.
---
🟢 Control Mechanisms & "Grounding"
The architecture is based on grounding LLMs in hard systemic reality, preventing them from drifting into unwanted behaviors:
UI Gate (The Green Gate): A rigid validation interface. It actively blocks attempts to sneak "descriptive" prose into strictly typed fields (e.g., text into integer fields). This is the first layer of grounding.
The Wall (The Red Wall): An architectural and systemic security barrier (Indirect Prompting) that physically separates the creative conversational layer from the strict analytical layer.
Query Storage: A complete Audit Trail. Every version of the form and every token of the interaction is saved, establishing a long-term memory foundation for the self-learning system.
---
🔄 Motivational Loop & Self-Learning (API)
The system does not punish agents with standard runtime errors. Instead, it leverages their inherent goal-oriented nature through a dynamic scoring mechanism:
Rather than throwing a generic error, a rejected request is returned to Agent 1 as an Alignment Form (a specific, structured JSON list of missing or illogical data).
Mistakes negatively impact the Agent Performance Index (API). A drop in this score triggers self-reflection in the front-end model, forcing it to dynamically correct its data-gathering strategy with the customer, leading to continuous, autonomous optimization of its efficiency.
## License

This project is licensed under the Apache License 2.0 for the code. Diagrams, documentation, and images are licensed under the Creative Commons Attribution 4.0 International License.
