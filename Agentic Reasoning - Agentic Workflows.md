---
share: true
---
### Overview

Agentic workflows refer to a new way of interacting with large language models (LLMs) where multiple instances of LLM performs actions in an iterative way, rather than just responding to a single prompt.

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

Agentic workflows, like in programming can abide to different agentic Al design patterns.

### Agentic Workflows Design Patterns

Agentic workflows, like in programming can abide to different design patterns.

Here are some popular design patterns for agentic workflows:

- [Reflection](https://x.com/AndrewYNg/status/1773393357022298617): The LLM examines its own work to come up with ways to improve it. 
- [Tool use](https://x.com/AndrewYNg/status/1775951610059141147): The LLM is given tools such as web search, code execution, or any other function to help it gather information, take action, or process data. 
- [Planning](https://x.com/AndrewYNg/status/1779606380665803144): The LLM comes up with, and executes, a multistep plan to achieve a goal (for example, writing an outline for an essay, then doing online research, then writing a draft, and so on). 
- Multi-agent collaboration: More than one AI agent work together, splitting up tasks and discussing and debating ideas, to come up with better solutions than a single agent would.

### Agentic Workflows Tools
- Programming frameworks for agentic AI.
	- [Microsoft Autogen](https://github.com/microsoft/autogen)
	- [CrewAI](https://github.com/joaomdmoura/crewai)
- [ChatDev](https://github.com/OpenBMB/ChatDev)

### Resources

<iframe width="560" height="315" src="https://www.youtube.com/embed/sal78ACtGTc?si=H4mU6MDkj6tAGspu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
# Footnotes

[^1]: https://twitter.com/AndrewYNg/status/1770897666702233815