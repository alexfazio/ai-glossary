---
share: true
---
Agentic workflows refer to a new way of interacting with large language models (LLMs) where multiple instances of LLM performs actions in an iterative way, rather than just responding to a single prompt.

Agents can be customized and augmented using prompt engineering techniques and external tools that enable them to retrieve information or execute code. [^2]

Multi-agent applications can be fully autonomous or moderated through “human proxy agents,” which allow users to step into the conversation between the AI agents, acting as another voice to provide oversight and control over their process. In a way, the human user is turned into a team leader overseeing a team of multiple AIs. [^2]

> "Today, we mostly use LLMs in zero-shot mode, prompting a model to generate final output token by token without revising its work. This is akin to asking someone to compose an essay from start to finish, typing straight through with no backspacing allowed, and expecting a high-quality result. Despite the difficulty, LLMs do amazingly well at this task!"
> "With an agentic workflow, however, we can ask the LLM to iterate over a document many times. For example, it might take a sequence of steps such as: 
> - Plan an outline. 
> - Decide what, if any, web searches are needed to gather more information. 
> - Write a first draft. 
> - Read over the first draft to spot unjustified arguments or extraneous information. 
> - Revise the draft taking into account any weaknesses spotted. 
> - And so on. 
> This iterative process is critical for most human writers to write good text. With AI, such an iterative workflow yields much better results than writing in a single pass."
> — Andrew Ng, Co-founder of Google Brain and Former Chief Scientist at Baidu [^2]

Agentic workflows, like in programming can abide to different [Agentic Al Design Patterns](./Agentic%2520Al%2520Design%2520Patterns.md#).
### Agentic Workflows Tools
- Programming frameworks for agentic AI.
	- [Microsoft Autogen](https://github.com/microsoft/autogen)
	- [CrewAI](https://github.com/joaomdmoura/crewai)
- [ChatDev](https://github.com/OpenBMB/ChatDev)
### Footnotes

https://www.youtube.com/embed/sal78ACtGTc?si=H4mU6MDkj6tAGspu

[^1]: https://twitter.com/AndrewYNg/status/1770897666702233815
[^2]: https://venturebeat.com/ai/microsofts-autogen-framework-allows-multiple-ai-agents-to-talk-to-each-other-and-complete-your-tasks/