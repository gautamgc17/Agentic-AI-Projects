### Concepts:

1. [Multi-Agent Architecture](https://github.com/langchain-ai/langgraph/tree/main/examples/multi_agent)

A multi-agent architecture when multiple different agents work on the same shared state, and so these agents can be a prompt, list of tools and a LLM.

2. [Supervisor](https://github.com/langchain-ai/langgraph/tree/main/examples/multi_agent)

A Supervisor LLM that is in charge of routing and coordinaing among these different sub-agents and also determines what input goes into them and so, those agents could themselves have different states inside them.

3. Flow Engineering: Based on [AlphaCodium Flow](https://github.com/Codium-ai/AlphaCodium)

In this [paper](https://arxiv.org/abs/2401.08500), the flow is divided into two main phases:

    – The pre-processing phase represents a linear flow where we reason about the problem, in natural language.
    – The code iterations phase includes iterative stages where we generate, run, and fix a code against certain tests.

4. [Plan and Execute](https://github.com/langchain-ai/langgraph/tree/main/examples/plan-and-execute)

Here, we first do explicit planning step upfront and then you execute them. The agent works until it achieves the plan; replanning maybe required or maybe not.

5. [Language Agent Tree Search](https://github.com/langchain-ai/langgraph/tree/main/examples/lats)

This basically does a tree search over the state of possible actions.

6. `LangGraph` is a graph-based workflow system built on LangChain, designed for building AI-driven applications. Unlike traditional linear workflows, LangGraph allows branching, looping, and dynamic routing, making it an ideal choice for complex, multi-step workflows.

7. In AI applications, traditional workflows often follow a step-by-step process (sequential flow). However, real-world AI applications require:

✅ Decision-making (Branching logic based on conditions)

✅ Looping Mechanisms (Re-evaluating inputs dynamically)

✅ Parallel Processing (Executing multiple actions simultaneously)

LangGraph solves these problems by offering graph-based execution, where nodes can be dynamically linked, and state management ensures data persistence.

8. Key Concepts in LangGraph

- `Nodes` represent individual tasks or actions in the workflow. Each node executes a function, processes data, and determines what should happen next. Nodes define the modular components of the system and execute specific logic at each step.

- `Edges` define the connection between nodes and determine how the workflow progresses. Edges decide the next step based on conditions or user input. Edges act as decision-making pathways that control the movement between different tasks in the workflow. `Conditional Edges` are used to make decisions.

- `State` stores contextual data between steps, ensuring memory persistence. The state allows nodes to access and modify information while executing a task. State management is crucial because it ensures that data is carried across different steps and that the system operates smoothly.

- `StateGraph`: The directed graph that models the entire decision-making process of the agent.


<br>

### References

1. https://python.langchain.com/docs/introduction/
2. https://github.com/langchain-ai/langchain/tree/master/cookbook
3. https://github.com/langchain-ai/langgraph/tree/main/examples 
4. https://smith.langchain.com/hub
5. https://learn.deeplearning.ai/
6. https://www.qodo.ai/blog/qodoflow-state-of-the-art-code-generation-for-code-contests/
7. https://github.com/Codium-ai/AlphaCodium