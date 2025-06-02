# Comprehensive OpenAI Agents SDK Quiz

This quiz is designed for graduate-level understanding of the OpenAI Agents SDK, covering its core components, architecture, and practical implementation as detailed in the official documentation.

## Conceptual MCQs

1. **What is the primary design philosophy of the OpenAI Agents SDK?**  
   a) To provide a high-abstraction framework for machine learning model training  
   b) To simplify the creation of autonomous, multi-agent AI systems with minimal abstractions  
   c) To optimize hardware performance for AI deployments  
   d) To focus on static rule-based systems for task automation  
   **Answer**: b  
   **Explanation**: The SDK is designed to simplify building complex, autonomous multi-agent systems with minimal abstractions, as stated in the documentation’s introduction.

2. **Which component of the OpenAI Agents SDK is responsible for orchestrating agent execution?**  
   a) Agent  
   b) Runner  
   c) Guardrails  
   d) Tracer  
   **Answer**: b  
   **Explanation**: The `Runner` class orchestrates agent execution, managing prompts, tools, and handoffs until task completion.

3. **What is the role of Guardrails in the OpenAI Agents SDK?**  
   a) To train large language models  
   b) To validate inputs and outputs for safe and controlled agent behavior  
   c) To manage cloud deployments  
   d) To optimize API latency  
   **Answer**: b  
   **Explanation**: Guardrails ensure agents operate within defined constraints by validating inputs and outputs, as per the documentation’s safety features.

4. **Which feature of the SDK allows agents to delegate tasks to other specialized agents?**  
   a) Tracing  
   b) Handoffs  
   c) State Management  
   d) Tool Invocation  
   **Answer**: b  
   **Explanation**: Handoffs enable agents to delegate tasks to other agents with specialized capabilities, as described in the SDK’s architecture.

5. **What is the purpose of the Tracing feature in the OpenAI Agents SDK?**  
   a) To reduce model inference time  
   b) To provide visualization and debugging of agent workflows  
   c) To manage persistent storage  
   d) To automate model retraining  
   **Answer**: b  
   **Explanation**: Tracing offers built-in capabilities to visualize and debug agent actions, as highlighted in the documentation.

6. **Which API format must LLMs support to be compatible with the OpenAI Agents SDK?**  
   a) REST API  
   b) GraphQL API  
   c) Chat Completions API  
   d) SOAP API  
   **Answer**: c  
   **Explanation**: The SDK requires LLMs to support the OpenAI Chat Completions API format for seamless integration.

7. **How does the OpenAI Agents SDK handle state management for complex tasks?**  
   a) By storing state in a local database  
   b) By maintaining a shared state dictionary across agent interactions  
   c) By using external cloud storage  
   d) By resetting state after each task  
   **Answer**: b  
   **Explanation**: The SDK uses a shared state dictionary to manage context across agent interactions, as per the state management section.

8. **What is a key benefit of the SDK’s Python-first design?**  
   a) It supports cross-platform hardware integration  
   b) It simplifies development with a familiar Pythonic interface  
   c) It optimizes for TypeScript-based applications  
   d) It reduces dependency on external APIs  
   **Answer**: b  
   **Explanation**: The Python-first design ensures a familiar and accessible interface for developers, as noted in the documentation.

9. **Which component allows the SDK to dynamically invoke external tools?**  
   a) Runner  
   b) Tools  
   c) Guardrails  
   d) Handoffs  
   **Answer**: b  
   **Explanation**: The Tools component enables agents to dynamically invoke external functions, as described in the documentation.

10. **What happens when an agent reaches a maximum iteration limit in the OpenAI Agents SDK?**  
    a) The agent continues indefinitely  
    b) The Runner terminates the task with an error  
    c) The agent retrains the model  
    d) The task is delegated to a new agent  
    **Answer**: b  
    **Explanation**: The Runner enforces a maximum iteration limit to prevent infinite loops, terminating with an error if exceeded.

11. **Which protocol is referenced for standardizing tool interactions in the SDK?**  
    a) HTTP/2  
    b) Model Context Protocol (MCP)  
    c) gRPC  
    d) WebSocket  
    **Answer**: b  
    **Explanation**: The SDK supports MCP for standardized tool and data integration, as mentioned in the documentation.

12. **What is a key challenge when integrating the OpenAI Agents SDK with non-OpenAI models?**  
    a) Lack of Python support  
    b) Ensuring compatibility with the Chat Completions API format  
    c) High computational requirements  
    d) Limited documentation  
    **Answer**: b  
    **Explanation**: Non-OpenAI models must support the Chat Completions API format, which can be a challenge, as noted in the SDK’s compatibility section.

13. **How does the SDK handle dynamic tool discovery?**  
    a) By hard-coding tool configurations  
    b) By allowing agents to query available tools at runtime  
    c) By using a static database  
    d) By requiring manual tool registration  
    **Answer**: b  
    **Explanation**: The SDK supports dynamic tool discovery, allowing agents to identify tools at runtime, as per the Tools section.

14. **What is the purpose of the `max_iterations` parameter in the Runner?**  
    a) To limit the number of API calls  
    b) To control the number of task iterations before termination  
    c) To set the maximum number of agents  
    d) To restrict response length  
    **Answer**: b  
    **Explanation**: The `max_iterations` parameter prevents infinite loops by limiting task iterations, as described in the Runner documentation.

15. **Which feature of the SDK supports real-time monitoring of agent performance?**  
    a) Guardrails  
    b) Tracing  
    c) Handoffs  
    d) State Management  
    **Answer**: b  
    **Explanation**: Tracing provides real-time visualization of agent actions for performance monitoring.

16. **What is a key application of the OpenAI Agents SDK mentioned in the documentation?**  
    a) Hardware simulation  
    b) Building conversational AI assistants  
    c) Optimizing database queries  
    d) Designing static websites  
    **Answer**: b  
    **Explanation**: The SDK is used for applications like conversational AI assistants and customer support systems.

17. **How does the SDK ensure interoperability with third-party LLMs?**  
    a) By using a custom API format  
    b) By requiring models to support the Chat Completions API  
    c) By embedding models in the SDK  
    d) By limiting support to OpenAI models  
    **Answer**: b  
    **Explanation**: Third-party LLMs must support the Chat Completions API for interoperability.

18. **What is the role of the `instructions` parameter in the Agent class?**  
    a) To define hardware requirements  
    b) To specify the system prompt or behavior for the agent  
    c) To configure network settings  
    d) To set API endpoints  
    **Answer**: b  
    **Explanation**: The `instructions` parameter defines the agent’s system prompt or behavior, as per the Agent class documentation.

19. **Which component of the SDK is responsible for managing persistent context?**  
    a) Runner  
    b) State Management  
    c) Guardrails  
    d) Tools  
    **Answer**: b  
    **Explanation**: State Management maintains persistent context across agent interactions using a shared state dictionary.

20. **What is a limitation of the OpenAI Agents SDK mentioned in the documentation?**  
    a) Lack of Python support  
    b) Dependency on OpenAI’s API for some features  
    c) Inability to handle multiple agents  
    d) No support for tool integration  
    **Answer**: b  
    **Explanation**: The SDK’s reliance on OpenAI’s API can be a limitation for cost or compatibility with non-OpenAI models.

## Coding-Based MCQs

21. **Which code snippet correctly initializes an Agent with the OpenAI Agents SDK?**  
    a)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", instructions="You are a research assistant.")
    ```  
    b)  
    ```python
    from openai import Agent
    agent = Agent(model="gpt-4o", prompt="You are a research assistant.")
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", system_prompt="You are a research assistant.")
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(instructions="You are a research assistant.")
    ```  
    **Answer**: a  
    **Explanation**: The `Agent` class requires a `model` and `instructions` parameter, as per the documentation.

22. **How do you add a custom tool to an agent in the OpenAI Agents SDK?**  
    a)  
    ```python
    def search_tool(query):
        return f"Search results for {query}"
    agent = Agent(model="gpt-4o", instructions="Perform searches.")
    agent.add_tool({"name": "search", "function": search_tool})
    ```  
    b)  
    ```python
    def search_tool(query):
        return f"Search results for {query}"
    agent = Agent(model="gpt-4o")
    agent.tools["search"] = search_tool
    ```  
    c)  
    ```python
    def search_tool(query):
        return f"Search results for {query}"
    agent = Agent(model="gpt-4o")
    agent.register_tool(search_tool)
    ```  
    d)  
    ```python
    def search_tool(query):
        return f"Search results for {query}"
    agent = Agent(model="gpt-4o")
    agent.add_tool(search_tool)
    ```  
    **Answer**: a  
    **Explanation**: Tools are added using a dictionary with `name` and `function` keys, as per the Tools section.

23. **Which code snippet correctly runs an agent using the Runner class?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="Answer questions.")
    Runner.run(agent, user_prompt="What is AI?")
    ```  
    b)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o")
    Runner.execute(agent, "What is AI?")
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.run("What is AI?")
    ```  
    d)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner(agent, "What is AI?")
    ```  
    **Answer**: a  
    **Explanation**: The `Runner.run` classmethod executes the agent with a user prompt, as shown in the documentation.

24. **How do you enable tracing for debugging in the OpenAI Agents SDK?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="Analyze data.")
    Runner.run(agent, user_prompt="Analyze trends.", trace=True)
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", trace=True)
    agent.run("Analyze trends.")
    ```  
    c)  
    ```python
    from openai_agents import Tracer
    Tracer.enable(agent)
    ```  
    d)  
    ```python
    from openai_agents import Runner
    Runner.trace(agent, "Analyze trends.")
    ```  
    **Answer**: a  
    **Explanation**: Tracing is enabled by passing `trace=True` to `Runner.run`, as per the Tracing section.

25. **Which code snippet correctly implements a handoff between two agents?**  
    a)  
    ```python
    from openai_agents import Agent
    agent1 = Agent(model="gpt-4o", instructions="Research topic.")
    agent2 = Agent(model="gpt-4o", instructions="Summarize findings.")
    agent1.handoff(agent2, task="Summarize this research.")
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    agent1.delegate(agent2, "Summarize this research.")
    ```  
    c)  
    ```python
    from openai_agents import Runner
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    Runner.handoff(agent1, agent2, "Summarize this research.")
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    agent1.transfer(agent2, "Summarize this research.")
    ```  
    **Answer**: a  
    **Explanation**: The `handoff` method delegates tasks between agents, as described in the Handoffs section.

26. **How do you define a dynamic system prompt for an agent?**  
    a)  
    ```python
    def dynamic_prompt(user):
        return f"You are assisting {user}."
    agent = Agent(model="gpt-4o", instructions=dynamic_prompt("Alice"))
    ```  
    b)  
    ```python
    def dynamic_prompt(user):
        return f"You are assisting {user}."
    agent = Agent(model="gpt-4o", prompt=dynamic_prompt)
    ```  
    c)  
    ```python
    def dynamic_prompt(user):
        return f"You are assisting {user}."
    agent = Agent(model="gpt-4o", system_prompt=dynamic_prompt("Alice"))
    ```  
    d)  
    ```python
    def dynamic_prompt(user):
        return f"You are assisting {user}."
    agent = Agent(model="gpt-4o", callable=dynamic_prompt)
    ```  
    **Answer**: a  
    **Explanation**: The `instructions` parameter accepts a callable function that returns a string, as per the Agent class documentation.

27. **Which code snippet correctly integrates a custom OpenAI client with the SDK?**  
    a)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key", base_url="https://api.openai.com/v1")
    agent = Agent(model="gpt-4o", client=client, instructions="Assist users.")
    ```  
    b)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key")
    agent = Agent(model="gpt-4o", api_key="your_api_key")
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", base_url="https://api.openai.com/v1")
    ```  
    d)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key")
    agent = Agent(model="gpt-4o", client=client, api_key="your_api_key")
    ```  
    **Answer**: a  
    **Explanation**: A custom OpenAI client with the correct base URL and API key is passed to the `Agent` class.

28. **How do you add a tool to fetch current time in the OpenAI Agents SDK?**  
    a)  
    ```python
    from datetime import datetime
    def time_tool():
        return datetime.now().strftime("%H:%M:%S")
    agent = Agent(model="gpt-4o", instructions="Provide time.")
    agent.add_tool({"name": "get_time", "function": time_tool})
    ```  
    b)  
    ```python
    from datetime import datetime
    def time_tool():
        return datetime.now().strftime("%H:%M:%S")
    agent = Agent(model="gpt-4o")
    agent.tools["get_time"] = time_tool
    ```  
    c)  
    ```python
    from datetime import datetime
    def time_tool():
        return datetime.now().strftime("%H:%M:%S")
    agent = Agent(model="gpt-4o")
    agent.register_tool(time_tool)
    ```  
    d)  
    ```python
    from datetime import datetime
    def time_tool():
        return datetime.now().strftime("%H:%M:%S")
    agent = Agent(model="gpt-4o")
    agent.add_tool(time_tool)
    ```  
    **Answer**: a  
    **Explanation**: Tools are added using a dictionary with `name` and `function`, as per the Tools section.

29. **Which code snippet correctly handles errors during agent execution?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    try:
        agent = Agent(model="gpt-4o", instructions="Analyze data.")
        Runner.run(agent, user_prompt="Invalid task.")
    except Exception as e:
        print(f"Error: {e}")
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.run("Invalid task.").catch(print)
    ```  
    c)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner.run(agent, user_prompt="Invalid task.", error_handler=print)
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.handle_error("Invalid task.")
    ```  
    **Answer**: a  
    **Explanation**: Standard Python try-except blocks are used to handle errors during agent execution.

30. **How do you configure a guardrail to limit response length in the OpenAI Agents SDK?**  
    a)  
    ```python
    agent = Agent(model="gpt-4o", instructions="Keep answers short.", guardrails={"max_length": 100})
    ```  
    b)  
    ```python
    agent = Agent(model="gpt-4o")
    agent.set_guardrail(max_length=100)
    ```  
    c)  
    ```python
    agent = Agent(model="gpt-4o")
    agent.limit_response(100)
    ```  
    d)  
    ```python
    agent = Agent(model="gpt-4o", guardrails=True)
    ```  
    **Answer**: a  
    **Explanation**: Guardrails are configured during agent initialization with specific constraints like `max_length`.

31. **Which code snippet correctly runs a multi-agent system with the Runner class?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent1 = Agent(model="gpt-4o", instructions="Research topic.")
    agent2 = Agent(model="gpt-4o", instructions="Summarize findings.")
    Runner.run([agent1, agent2], user_prompt="Study AI trends.")
    ```  
    b)  
    ```python
    from openai_agents import Agent, Runner
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    Runner.run(agent1, agent2, "Study AI trends.")
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    agent1.run(agent2, "Study AI trends.")
    ```  
    d)  
    ```python
    from openai_agents import Runner
    agent1 = Agent(model="gpt-4o")
    agent2 = Agent(model="gpt-4o")
    Runner.execute([agent1, agent2], "Study AI trends.")
    ```  
    **Answer**: a  
    **Explanation**: The `Runner.run` method accepts a list of agents and a shared user prompt.

32. **How do you integrate a third-party LLM like Anthropic’s Claude with the SDK?**  
    a)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key", base_url="https://api.anthropic.com/v1")
    agent = Agent(model="claude-3.5-sonnet", client=client, instructions="Assist users.")
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="claude-3.5-sonnet", api_key="your_api_key")
    ```  
    c)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key")
    agent = Agent(model="claude-3.5-sonnet", client=client)
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="anthropic/claude-3.5-sonnet", instructions="Assist users.")
    ```  
    **Answer**: a  
    **Explanation**: A custom OpenAI client with Anthropic’s API base URL is required, assuming Claude supports the Chat Completions format.

33. **Which code snippet correctly implements a tool with parameters in the SDK?**  
    a)  
    ```python
    def add_tool(a, b):
        return a + b
    agent = Agent(model="gpt-4o", instructions="Perform calculations.")
    agent.add_tool({"name": "add", "function": add_tool, "parameters": ["a", "b"]})
    ```  
    b)  
    ```python
    def add_tool(a, b):
        return a + b
    agent = Agent(model="gpt-4o")
    agent.add_tool({"name": "add", "function": add_tool})
    ```  
    c)  
    ```python
    def add_tool(a, b):
        return a + b
    agent = Agent(model="gpt-4o")
    agent.register_tool(add_tool, ["a", "b"])
    ```  
    d)  
    ```python
    def add_tool(a, b):
        return a + b
    agent = Agent(model="gpt-4o")
    agent.tools["add"] = add_tool
    ```  
    **Answer**: a  
    **Explanation**: Tools can include a `parameters` field to define input arguments, as per the Tools section.

34. **How do you manage state across agent interactions in the SDK?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="Track user data.")
    state = {"user_id": "123"}
    Runner.run(agent, user_prompt="Update user data.", state=state)
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.set_state({"user_id": "123"})
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", state={"user_id": "123"})
    ```  
    d)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner.run(agent, user_prompt="Update user data.", context={"user_id": "123"})
    ```  
    **Answer**: a  
    **Explanation**: The `state` parameter in `Runner.run` manages a shared state dictionary across interactions.

35. **Which code snippet correctly queries an agent with a system and user prompt?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="You are an expert.")
    Runner.run(agent, user_prompt="Explain AI agents.")
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.run(system="You are an expert.", user="Explain AI agents.")
    ```  
    c)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner.run(agent, system_prompt="You are an expert.", user_prompt="Explain AI agents.")
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", system="You are an expert.")
    agent.run("Explain AI agents.")
    ```  
    **Answer**: a  
    **Explanation**: The system prompt is set via the `instructions` parameter, and `Runner.run` uses `user_prompt`.

36. **How do you handle a tool call response in the OpenAI Agents SDK?**  
    a)  
    ```python
    def search_tool(query):
        return f"Results for {query}"
    agent = Agent(model="gpt-4o", instructions="Search data.")
    agent.add_tool({"name": "search", "function": search_tool})
    response = Runner.run(agent, user_prompt="Search AI trends.")
    ```  
    b)  
    ```python
    def search_tool(query):
        return f"Results for {query}"
    agent = Agent(model="gpt-4o")
    agent.on_tool_call("search", search_tool)
    ```  
    c)  
    ```python
    def search_tool(query):
        return f"Results for {query}"
    agent = Agent(model="gpt-4o")
    agent.call_tool("search", query="AI trends")
    ```  
    d)  
    ```python
    def search_tool(query):
        return f"Results for {query}"
    agent = Agent(model="gpt-4o")
    agent.handle_tool(search_tool, "AI trends")
    ```  
    **Answer**: a  
    **Explanation**: The Runner automatically handles tool calls when a tool is added and invoked during execution.

37. **Which code snippet correctly integrates OpenRouter with the SDK?**  
    a)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key", base_url="https://openrouter.ai/api/v1")
    agent = Agent(model="google/gemini-2.0-flash", client=client, instructions="Assist users.")
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="google/gemini-2.0-flash", api_key="your_api_key")
    ```  
    c)  
    ```python
    from openai import OpenAI
    from openai_agents import Agent
    client = OpenAI(api_key="your_api_key")
    agent = Agent(model="google/gemini-2.0-flash", client=client)
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="openrouter/gemini-2.0-flash", instructions="Assist users.")
    ```  
    **Answer**: a  
    **Explanation**: OpenRouter requires a custom OpenAI client with its base URL, as shown in the documentation.

38. **How do you limit the number of iterations in the Runner class?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="Analyze data.")
    Runner.run(agent, user_prompt="Analyze trends.", max_iterations=10)
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", max_iterations=10)
    agent.run("Analyze trends.")
    ```  
    c)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner.run(agent, user_prompt="Analyze trends.", limit=10)
    ```  
    d)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.set_iterations(10)
    ```  
    **Answer**: a  
    **Explanation**: The `max_iterations` parameter in `Runner.run` limits task iterations.

39. **Which code snippet correctly queries an agent with a stateful context?**  
    a)  
    ```python
    from openai_agents import Agent, Runner
    agent = Agent(model="gpt-4o", instructions="Track user data.")
    state = {"user_id": "123", "history": []}
    Runner.run(agent, user_prompt="Add data to history.", state=state)
    ```  
    b)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o", state={"user_id": "123"})
    agent.run("Add data to history.")
    ```  
    c)  
    ```python
    from openai_agents import Agent
    agent = Agent(model="gpt-4o")
    agent.set_state({"user_id": "123", "history": []})
    ```  
    d)  
    ```python
    from openai_agents import Runner
    agent = Agent(model="gpt-4o")
    Runner.run(agent, user_prompt="Add data to history.", context={"user_id": "123"})
    ```  
    **Answer**: a  
    **Explanation**: The `state` parameter in `Runner.run` manages persistent context.

40. **How do you implement a tool that requires multiple parameters in the SDK?**  
    a)  
    ```python
    def multiply_tool(x, y):
        return x * y
    agent = Agent(model="gpt-4o", instructions="Perform calculations.")
    agent.add_tool({"name": "multiply", "function": multiply_tool, "parameters": ["x", "y"]})
    ```  
    b)  
    ```python
    def multiply_tool(x, y):
        return x * y
    agent = Agent(model="gpt-4o")
    agent.add_tool({"name": "multiply", "function": multiply_tool})
    ```  
    c)  
    ```python
    def multiply_tool(x, y):
        return x * y
    agent = Agent(model="gpt-4o")
    agent.register_tool(multiply_tool, ["x", "y"])
    ```  
    d)  
    ```python
    def multiply_tool(x, y):
        return x * y
    agent = Agent(model="gpt-4o")
    agent.tools["multiply"] = multiply_tool
    ```  
    **Answer**: a  
    **Explanation**: The tool definition includes a `parameters` field to specify input arguments, as per the Tools section.
