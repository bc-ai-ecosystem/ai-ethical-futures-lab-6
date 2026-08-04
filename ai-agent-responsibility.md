# 5. Advancing Ways to Better Track the Activity and Interactions of AI Agents

## Challenge
Agentic systems that plan, use tools and take multi-step actions introduce new opacity around permissions, actions taken, human oversight and accountability. Multi-agent systems amplify coordination and liability challenges.

## Relevant Proposed Questions Addressed
* Are you concerned about the use of AI agents? In what contexts is it most important to know that an AI agent is operating, and why? Who should be responsible for disclosing agent use? What information should be recorded about agent activities, what disclosures should be made, and to whom?  
* What information do businesses need to use AI agents confidently and safely? Do they currently have access to it? Are existing technical solutions, market practices and legal frameworks sufficient for transparency around agentic systems? If not, where are the gaps and what actions should the Government take?

## Existing Practical Solutions
Observability platforms (LangSmith, Maxim AI and similar) that log trajectories, tool calls and outcomes. OpenTelemetry extensions for agent workflows. Provenance patterns using C2PA-style assertions or authenticated data structures (e.g., AT Protocol signed repositories and DIDs for verifiable activity trails). Permission scoping, human-in-the-loop checkpoints and sandboxed execution.

## EU AI Act
AI agents that interact with natural persons fall under Article 50(1) transparency obligations: providers must design them so users know they are interacting with AI. Where an agent generates synthetic content or deepfakes, the corresponding Article 50(2)/(4)/(5) marking and disclosure duties apply. High-risk agentic systems are subject to the full high-risk documentation, logging, human-oversight and serious-incident reporting obligations. Product-liability rules (updated for software and AI) further reinforce accountability. Compliant providers build disclosure and logging primitives into agent frameworks; deployers configure appropriate monitoring, permission boundaries and human oversight, and ensure end-users receive clear information about agent capabilities and actions.