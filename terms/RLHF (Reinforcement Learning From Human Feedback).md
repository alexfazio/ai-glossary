---
share: true
---
RLHF is a method used to reduce bias in large language models. It works by allowing human testers to guide the AI model towards producing the type of text output they indicate they prefer. The use of the ratings given by human testers guides the improvement of AI models. [^3][^5]. 

ChatGPT was trained  using a RLHF. It is often said that RLHF is the secret ingredient of ChatGPT. The basic idea is to take a large language model with a tendency to spit out anything it wants—in this case, GPT-3.5—and tune it by teaching it what kinds of responses human users actually prefer. [^1]

OpenAI reduced the amount of misinformation and offensive text that GPT-3 produced by using reinforcement learning to train a version of the model on the preferences of human testers. [^2]

 [OpenAI](https://openai.com/research/instruction-following), [Google](https://www.deepmind.com/blog/building-safer-dialogue-agents), [Anthropic](https://www-files.anthropic.com/production/images/Model-Card-Claude-2.pdf), and other companies all use the technique. After a chatbot has processed massive amounts of text, human feedback helps fine-tune it. [^5]
  
RLHF allows the AI to learn from human preferences. To apply RLHF, companies hire large teams of contractors to look at the responses of their AI models and rate them as “good” or “bad”. By analysing enough responses, the model becomes attuned to those judgments, and filters its responses accordingly. This basic process works to refine an AI’s responses at a superficial level. But the method is primitive, according to [Dario Amodei](../Dario%20Amodei.md), who helped develop it while previously working at OpenAI. “It’s . . . not very accurate or targeted, you don’t know why you’re getting the responses you’re getting [and] there’s lots of noise in that process,” he said. [^6]

### Footnotes

[^1]: https://www.technologyreview.com/2023/03/03/1069311/inside-story-oral-history-how-chatgpt-built-openai/
[^2]: https://www.technologyreview.com/2023/02/08/1068068/chatgpt-is-everywhere-heres-where-it-came-from/
[^3]: https://www.technologyreview.com/2023/12/19/1084505/generative-ai-artificial-intelligence-bias-jobs-copyright-misinformation/
[^4]: https://www.technologyreview.com/2023/03/20/1070067/language-models-may-be-able-to-self-correct-biases-if-you-ask-them-to/
[^5]: https://www.theatlantic.com/technology/archive/2023/07/ai-chatbot-human-evaluator-feedback/674805/
[^6]: https://www.ft.com/content/f23e59a2-4cad-43a5-aed9-3aea6426d0f2