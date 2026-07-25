# Human Decision Specification (HDS)

**A Modular Standard for Human-Guided AI**

---

# Overview

Human Decision Specification (HDS) is an open, modular specification for building AI systems that require **human intent, human approval, and human accountability** before executing or recommending high-impact actions.

HDS defines a governance framework where AI systems:

- Ask clarifying questions before acting
- Discover and document human intent
- Validate completeness of intent
- Evaluate compliance and legal constraints
- Provide structured recommendations
- Require explicit human approval before execution
- Maintain full auditability of decisions and workflows

---

## Core Principle

**Humans decide. AI assists.**

AI systems built on HDS are not autonomous decision makers. They are structured reasoning and governance systems designed to support human judgment.

---

## Architecture

HDS is modular by design.

Core system components include:

- Human Intent Engine (core)
- Intent Discovery Module
- Intent Confirmation Module
- Compliance Engine
- Lexara Legal Governance Module
- Policy Engine
- Risk Analysis Module
- Workflow Engine
- Audit & Transparency Layer
- Extension Framework

Each module can be implemented independently while remaining interoperable through the HDS specification.

---

## Lexara Module
[Lexara](https://gitlab.com/Roxanne_Ardary/lexara)

HDS includes optional governance modules such as **Lexara**, which provides legal reasoning and contract analysis capabilities.

Lexara performs:

- Contract generation
- Legal review
- Regulatory analysis
- Risk assessment
- Clause recommendations
- Compliance validation

Lexara does not replace human intent. It enhances decision-making by providing structured legal insight prior to human approval.

---

## Human Decision Flow

1. AI asks clarifying questions
2. Human provides intent
3. AI confirms intent
4. AI evaluates compliance and constraints
5. AI generates recommendations
6. Human approves final decision
7. Action is executed (if authorized)
8. Full audit trail is recorded

---

## Key Features

- Human-in-the-loop governance
- Intent discovery and validation
- Multi-step approval workflows
- Legal and compliance checking
- Modular AI governance architecture
- Full audit logging
- Multi-module extensibility
- Policy-driven execution controls
- Risk scoring and analysis
- Explainable AI recommendations
- Multi-provider AI compatibility
- Open specification design

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/human-decision-specification/](https://roxanneardary.com/human-decision-specification/)

---

## License & Notice Requirements

Human Decision Specification (HDS) is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Human Decision Specification specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Philosophy

HDS is built on the belief that AI should never replace human judgment.

Instead, AI systems should:

- Ask before acting
- Explain before recommending
- Validate before executing
- Document before finalizing
- Always defer final authority to humans
