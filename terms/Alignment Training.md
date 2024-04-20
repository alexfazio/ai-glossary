---
share: true
---
There are a few types of alignment training. The most relevant looks rather old-fashioned: Humans interact with the LLM and rate its responses good or bad, which coaxes it toward certain behaviors (such as being friendly or polite) and away from others (like profanity and abusive language). Tramèr told me that this seems to steer LLMs away from quoting their training data. He was part of a team that managed to break ChatGPT’s alignment training while studying its ability to memorize text, but he said that it works “remarkably well” in normal interactions. Nevertheless, he said, “alignment alone is not going to completely get rid of this problem.” [^1]

Another potential solution is [retrieval-augmented generation](https://www.theatlantic.com/technology/archive/2023/11/google-generative-ai-search-featured-results/675899/). RAG is a system for finding answers to questions in external sources, rather than within a language model. A RAG-enabled chatbot can respond to a question by retrieving relevant webpages, summarizing their contents, and providing links. Google Bard, for example, offers a list of “additional resources” at the end of its answers to some questions. RAG isn’t bulletproof, but it [reduces the chance](https://research.ibm.com/blog/retrieval-augmented-generation-RAG) of an LLM giving incorrect information (or “hallucinating”), and it has the added benefit of avoiding copyright infringement, because sources are cited. [^1]

### Footnotes

[^1]: https://www.theatlantic.com/technology/archive/2024/01/chatgpt-memorization-lawsuit/677099/