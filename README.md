# Custom Tools – ADK Tooling Guide

**By Harsha Vardhani

# 🚀 Project Overview

In this notebook, we deep dive into Custom Tools in ADK, exploring how user-defined logic, function tools, agent tools, and built-in executors come together to create powerful agent workflows. The focus is on understanding when to build custom tools, how to define them correctly, and how they interact inside multi-agent pipelines.

We also extend the architecture using a dedicated calculation agent, showing how agents can delegate tasks reliably using ADK’s tool system.

# 🧠 Motivation

Real-world systems require custom business logic that generic tools cannot capture.

Built-in tools (like Google Search) are powerful, but companies need logic that aligns with internal rules, compliance, workflows, and domain-specific requirements.

ADK’s Custom Tools and Agent Tools allow full flexibility for building specialist processing layers, delegating tasks, and ensuring agents behave deterministically.

This enables developers to design robust, reusable, and enterprise-friendly agent pipelines.

# 📋 Contents

- What Are Custom Tools?
- When to Use Custom Tools
- Building Custom Function Tools
- Defining Tools in ADK
- Best Practices for Reliable Tools
- Using a Calculation Agent (Built-in Code Executor)
- Agent Tools vs Sub-Agents
- Complete Guide to ADK Tool Types
- Future Extensions

# 🧮 Key Concepts
** Custom Tools

- Tools you create using your own Python functions. They allow you to implement domain-specific logic, connect internal systems, and extend agent capabilities beyond built-in defaults.

** Function Tools

- Standard Python functions converted into agent tools. Great for lookup operations, validations, transformations, and simple business logic.

** Agent Tools

- Agents treated as callable tools. Enables specialist delegation—for example, sending math tasks to a calculation agent.

** Built-in Executors

- Tools like BuiltInCodeExecutor that run Python code safely and reliably for computation-heavy operations.

# 📝 Future Work & Extensions

- Add more domain-specific custom tools (finance, healthcare, validation systems).
- Integrate MCP tools for file systems, databases, or enterprise services.
- Use OpenAPI Tools to automatically convert entire API suites into agent tools.
- Build hybrid pipelines mixing multiple agents and tool categories.
- Introduce learning agents that optimize tool-selection based on context.

### 📚 Learn More  
Refer to the following documentation to learn more:  
- [ADK Documentation](https://www.kaggle.com/code/kaggle5daysofai/day-2a-agent-tools#ADK-Documentation)  
- [ADK Tools Documentation](https://www.kaggle.com/code/kaggle5daysofai/day-2a-agent-tools#ADK-Tools-Documentation)  
- [ADK Custom Tools Guide](https://www.kaggle.com/code/kaggle5daysofai/day-2a-agent-tools#ADK-Custom-Tools-Guide)  
- [ADK Function Tools](https://www.kaggle.com/code/kaggle5daysofai/day-2a-agent-tools#ADK-Function-Tools)  
- [ADK Plugins Overview](https://www.kaggle.com/code/kaggle5daysofai/day-2a-agent-tools#ADK-Plugins-Overview)  