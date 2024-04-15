---
share: true
---
GENERAL RESOURCES:
- https://www.linkedin.com/feed/update/urn:li:activity:7175157832277798912?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7175157832277798912%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29

---

"slot machine" effect
https://fablestudio.github.io/showrunner-agents/

NER (Named Entity Recognition)

Red Teaming (apparently synonym of Prompt engineering? "The voluntary commitments included third-party security testing of tools, known as red-teaming,"
https://www.nytimes.com/2023/12/06/technology/artificial-intelligence-regulation.html


5-shot* (reported)
Previous SOTA (GPT-4)

---

AGI

Artificial general intelligence (AGI) -- often referred to as "strong AI," "full AI," "human-level AI" or "general intelligent action" -- represents a significant future leap in the field of artificial intelligence. Unlike narrow AI, which is tailored for specific tasks, such as [detecting product flaws](https://techcrunch.com/2024/03/12/axion-rays-ai-attempts-to-detect-product-flaws-to-prevent-recalls/), [summarizing the news](https://techcrunch.com/2024/02/29/former-twitter-engineers-are-building-particle-an-ai-powered-news-reader/), or [building you a website](https://techcrunch.com/2024/02/22/10web-armenia/), AGI will be able to perform a broad spectrum of cognitive tasks at or above human levels.

The concept raises existential questions about humanity's role in and control of a future where machines can outthink, outlearn and outperform humans in virtually every domain.

The core of this concern lies in the unpredictability of AGI's decision-making processes and objectives, which might not align with human values or priorities (a concept [explored in-depth in science fiction since at least the 1940s](https://en.wikipedia.org/wiki/Three_Laws_of_Robotics)). There's concern that once AGI reaches a certain level of autonomy and capability, it might become impossible to contain or control, leading to scenarios where its actions cannot be predicted or reversed.

When sensationalist press asks for a timeframe, it is often baiting AI professionals into putting a timeline on the end of humanity -- or at least the current status quo. Needless to say, AI CEOs aren't always eager to tackle the subject.

https://techcrunch.com/2024/03/19/agi-and-hallucinations/

---

RAG

One solution _to hallucinations_ is retrieval augmented generation (rag), which splits the job of the ai model into two parts: retrieval and generation. Once a prompt is received, a retriever model bustles around an external source of information, like a newspaper archive, to extract relevant contextual information. This is fed to the generator model alongside the original prompt, prefaced with instructions not to rely on prior knowledge. The generator then acts like a normal llm and answers. This reduces hallucinations by letting the llm play to its strengths--summarising and paraphrasing rather than researching.

> As time goes on and some buyers of generative AI grow [disillusioned](https://url3396.theinformation.com/ls/click?upn=u001.71kYkaWDpGOJSzbGrs4y1TNF0-2FB-2Bh5pDUdkL0JSEoBmbIlaCwUAb-2B2vhxG1AFBaNIy9cLmq5IQ7RJCtlrFYwDboAnSX2O5rcpLmeKKxPaqIYrYBl6cxpEJ5rk9OcVBFOm2n6EChBZ-2BzsqCZpFF4jcyafGA6haYyE-2FE2d1EG4tzo-2FArtS0DX-2Fl-2BcUiB6g0cMAtHe9KNR3LGN0bA08r-2FLTtRTEExNVkXrXSyaU7ecO47s-3DYApl_9fRGlt2DYm1xrmGM-2FAZ6hQVgOZN6TjfclHbUdkz61v59o2FW9OhQRW5Ph96gtDJygm2dhwxuZl-2BD-2FAJHJezsonj9ERLg9tm8XII1eWmgffK6d2d20BvGwSIR9M2YgqwO8OgQua-2FzH75hqeYu6GlAHP4ikqrjlzQYts2IQ-2BUXTWVulwr-2BYfTafgocyQmL5OzpUozlpjbNSJwdvXwUpeYabRHMsG9OeDY5trC8QdBJty732jQhDFclvaohOyki0Hs5HAEJ2qBnFZzmgPKUTx0cC9g-2BwDEEQzQtPn-2BgmLtbihof3U-2F-2BuwEwjNKYyrbooPfha3TFXLJYDsiv2wpI-2B4Yv8s-2BzIeH0doLB0TnR1uNCk50-3D) with the meager returns they've seen, many are experimenting with new ways to eke better performance out of large language models without paying up for the latest, state-of-the-art LLM.

One way to do this is through a technique called [retrieval augmented generation](https://url3396.theinformation.com/ls/click?upn=u001.71kYkaWDpGOJSzbGrs4y1TNF0-2FB-2Bh5pDUdkL0JSEoBmbIlaCwUAb-2B2vhxG1AFBaNhUgXi5m9sGSIhWZinm-2BOaglbT6K3GOY0-2Fmrf-2BDIB6qh1dHNoSm-2B6HMaWukiKYcHzpnemgzO2Dok1EB3V2jEs5ibCBpOsA6PjgqVvM2QwPLMhCuBynmBgUTYJzpT1LpuScfB-2F4y8RvVCyxjw5tVEH84SexBCwcgqJNRo0Hv7J5vmnv-2FQuiy-2FmBhU2DT8L-2FOiQWYbd_9fRGlt2DYm1xrmGM-2FAZ6hQVgOZN6TjfclHbUdkz61v59o2FW9OhQRW5Ph96gtDJygm2dhwxuZl-2BD-2FAJHJezsonj9ERLg9tm8XII1eWmgffK6d2d20BvGwSIR9M2YgqwO8OgQua-2FzH75hqeYu6GlAHP4ikqrjlzQYts2IQ-2BUXTWVulwr-2BYfTafgocyQmL5OzpuIKrFo8oFsrBO9-2BX3DoaFKZjfcBeOTv3xAgJZjDcb7kSOChK0FGcIe7quFBKydLDwBV638GVxTsFZ1ArlPFDYIuiEIc79ZB9lujb24Muhyvg8hf6R2iUAS9nK0-2F9q4VyNoxIG8zbIM1j3OK3kVaEE6RsKnjk-2FZYt63w7vvEayiI-3D), which aims to reduce the AI's tendency to hallucinate or give incorrect answers by giving it access to real-time data from the internet or a company's own documents. This approach started [picking up steam last summer](https://url3396.theinformation.com/ls/click?upn=u001.71kYkaWDpGOJSzbGrs4y1TNF0-2FB-2Bh5pDUdkL0JSEoBmbIlaCwUAb-2B2vhxG1AFBaNhUgXi5m9sGSIhWZinm-2BOaglbT6K3GOY0-2Fmrf-2BDIB6qh1dHNoSm-2B6HMaWukiKYcHzpnemgzO2Dok1EB3V2jEs5ibCBpOsA6PjgqVvM2QwPLMhCuBynmBgUTYJzpT1LpuScfB-2F4y8RvVCyxjw5tVEH84SexBCwcgqJNRo0Hv7J5vmnv-2FQuiy-2FmBhU2DT8L-2FOiQhkkx_9fRGlt2DYm1xrmGM-2FAZ6hQVgOZN6TjfclHbUdkz61v59o2FW9OhQRW5Ph96gtDJygm2dhwxuZl-2BD-2FAJHJezsonj9ERLg9tm8XII1eWmgffK6d2d20BvGwSIR9M2YgqwO8OgQua-2FzH75hqeYu6GlAHP4ikqrjlzQYts2IQ-2BUXTWVulwr-2BYfTafgocyQmL5OzpXsy-2Buw8gd3pLYklkFu5Mx6qINbrCQIEXt6RO42-2FMBBVjWxdzrEtP9dWrXwTxAL1jY-2FURGEGiGE5O-2FA0xhuKTbaELEGO9OjMYILnwHs6Mx6phGtAmk20XdqVifslcEZGZ8w-2Bj41fS1dX43ZkRm5DvYvyBnv1Z4g93qpMWryxXdKI-3D), but like most things in AI, it's evolved quickly, and already, developers are experimenting with new ways to improve RAG.

The first step of RAG requires text to be transformed into **"vector embeddings,"** or strings of numbers that LLMs can process, by an AI model called an **"embedding model."**Typically, these embedding models are pretty general-purpose, but developers working in specific domains, like health care or law, have had success tweaking these embedding models for their particular domain. In some cases, that's helped improve the accuracy rate for LLMs' answers to questions to nearly 90% from 25%, said **Braden Hancock**, co-founder at data curation startup **Snorkel AI**.

Today, most embedding models are English-centric, which is helpful if you're, for instance, a U.S.-based clothing retailer that wants an LLM-powered shopping assistant chatbot to understand that maxi-length and midi-length white skirts are similar. However, Hancock ran into issues when helping an Indian clothing retailer, as popular embedding models didn't understand the nuances of clothing in that country, he said. By training the model on pairs of Indian clothing labeled as "similar" or "not similar," though, he was able to significantly improve its performance. (Jian-Yang from [Silicon Valley](https://url3396.theinformation.com/ls/click?upn=u001.71kYkaWDpGOJSzbGrs4y1aX5uLsKvrP2rYW0SU4-2BjHukIE4flqNYmGPudhMKTCzS4u-2FEgP5UIFuRQaqdJdfU-2BUbhceiQnGfhCnuxidD76CT5vBZPeejQ-2FUBbkyL26qsV-2BHzcStsYtZfXOCsDU4oQm8eRL6aYDSNZf3Z-2BnQUoXVNSx-2FVjtnnAeszTc7n-2B40WRnWuy_9fRGlt2DYm1xrmGM-2FAZ6hQVgOZN6TjfclHbUdkz61v59o2FW9OhQRW5Ph96gtDJygm2dhwxuZl-2BD-2FAJHJezsonj9ERLg9tm8XII1eWmgffK6d2d20BvGwSIR9M2YgqwO8OgQua-2FzH75hqeYu6GlAHP4ikqrjlzQYts2IQ-2BUXTWVulwr-2BYfTafgocyQmL5OzpNMOFLXPcBqIRfdI-2B5JYJuCW85by51K-2Ba0-2F6o5JHPYhO0Ne59U0ZhKtobDUVvq42Aziqy5r-2FDVKevhGcFB6UBNDzODk9GFVNG29e2De2vSHQhuVM9N3J1ZXgV6fCc7ttDADytJ-2FzCUhdt529l7fnwGgl0SEBV7y3XKvnRpGuMBvM-3D) would be proud.) You could see how a similar approach could be used to customize an embedding model for legal or health care terminology.

For others, it's not enough to optimize just the embedding model--you need to optimize the entire system, including the LLM, for doing RAG. That's the approach of **Contextual AI**, a language model developer co-founded last year by **Douwe Kiela**, a former **Meta** researcher who worked on the original RAG paper. The startup is building what it calls **"contextual language models,"** which optimize both the LLM and the retriever--the model responsible for finding reference documents based on a user's question--for conducting RAG. 

"It's like two halves of a brain--retrieval and generation," Kiela said. "With [the current RAG approach], these parts of the brain don't even know the other half exists."

The downside of this strategy, though, is that you're fully committing to the RAG approach. And in a space as fast-moving as AI, there's no telling whether RAG will be the dominant technique for feeding LLMs with up-to-date information in a year or two.

And performance isn't the only thing developers care about--costs are equally important. That's the issue that AI startup **Cohere** is tackling. In recent times, the Toronto-based **OpenAI** competitor has [pivoted away from building expensive, state-of-the-art LLMs](https://url3396.theinformation.com/ls/click?upn=u001.71kYkaWDpGOJSzbGrs4y1TNF0-2FB-2Bh5pDUdkL0JSEoBmbIlaCwUAb-2B2vhxG1AFBaNwTUUA6y4B4riLPjzGN4htJQgvP6XiUUcsUscf84ybyRilPiObDeIzyGHJkQDPDIDbHy0g8KplPimiqW-2Bqn-2FCS3-2B6NuMbPx9dkrbXXKet0K2baxxRVLlSCq6sZ47KJi0YC-2B6WpgntUWMc45AIeTslb74GuIpwQn7SBSS-2B6cVG3PfZufDr8o-2Bk7vo-2BszLgtt-2Bpl-2BYKX5gnhcRY1yqi22lFAA-3D-3DvuZu_9fRGlt2DYm1xrmGM-2FAZ6hQVgOZN6TjfclHbUdkz61v59o2FW9OhQRW5Ph96gtDJygm2dhwxuZl-2BD-2FAJHJezsonj9ERLg9tm8XII1eWmgffK6d2d20BvGwSIR9M2YgqwO8OgQua-2FzH75hqeYu6GlAHP4ikqrjlzQYts2IQ-2BUXTWVulwr-2BYfTafgocyQmL5OzpkWLdQgKFe0UGncfHgRzxM-2FYJ9lWN7B3-2FVrS9el2YTWYmKLZ9UW6CVYDkLHCrZwRg6z05kn7YOfuhJ10fNencHbNRu-2B00sqIikRNM8yj3qpWITRYb-2FHfT3ioKgLyxfXfhh5ldBcaara8SRAGbYwKJmIBnj1ulKAMX8xzUNv3kl54-3D) to focus on more efficient RAG-based software and models. Key to bringing costs down is decreasing the size of vector embeddings, said **Nils Reimers**, Cohere's director of machine learning. The startup has trained its embedding models to generate smaller embeddings, which helps customers save on server and memory costs, he said. (Cohere develops AI features for **Oracle** products.)

All of this goes to show that there's another trend rising in opposition to large-scale and expensive LLMs. This movement is more focused on practicality and accessibility, and can hopefully lead to real revenue, or a sustainable business model for companies using LLM.

https://www.economist.com/science-and-technology/2024/02/28/ai-models-make-stuff-up-how-can-hallucinations-be-controlled

https://www.theinformation.com/articles/wtf-is-rag-it-could-solve-llms-biggest-weaknesses?rc=yfiisw

---

CoT@32*
Chain of thought

Clever prompting can also reduce hallucinations. Researchers at Google DeepMind found that telling an llm to "take a deep breath and work on this problem step-by-step" reduced hallucinations and improved problem solving, especially of maths problems. One theory for why this works is that ai models learn patterns. By breaking a problem down into smaller ones, it is more likely that the model will be able to recognise and apply the right one.

https://www.economist.com/science-and-technology/2024/02/28/ai-models-make-stuff-up-how-can-hallucinations-be-controlled

https://news.ycombinator.com/item?id=38545663

https://www.perplexity.ai/search/If-ask-you-molJLqcFQCyQeLAUxLXRFA?s=c

https://twitter.com/paul_cal/status/1732479699152928876

---

MMLU (Massive Multitask
Language Understanding), one of
the most popular methods to test
the knowledge and problem
solving abilities of Al models.

CSQA CommonsenseQA

StrategyQA

https://share.cleanshot.com/SKw8GKbN


---

Foundation Model

---

https://www.linkedin.com/posts/armand-ruiz_last-week-google-announced-gemini-claiming-activity-7140309340703330304-mj44?utm_source=share&utm_medium=member_desktop

---

Emergent abilities


https://www.linkedin.com/posts/dair-institute_are-emergent-abilities-of-large-language-activity-7140391592221159424-pXNu?utm_source=share&utm_medium=member_ios

---

NLU Natural Language Understanding

---

Neural Networks

But what are neural networks? In simple terms, they use interconnected nodes that are inspired by neurons in the human brain. These networks are the foundation of machine learning and deep learning models, which use a complex structure of algorithms to process large amounts of data such as text, code, or images. Training these neural networks involves adjusting the weights or parameters of the connections between neurons to minimize the difference between predicted and desired outputs, which allows the network to learn from mistakes and make more accurate predictions based on the data.

What developers need to know about
generative AI
Damian Brady • April 7, 2023

---

Model

---

Model Quantization, 4bit, 2bit, 8-bit etc

---

Perché 0 shot si chiama SHOT? Stesso per one shot etc, qual'e' la logica del na

---

Catastrophic risk of ai

https://x.com/alxfazio/status/1737009480640946184?s=20

---

https://www.linkedin.com/posts/langgenius_an-insightful-article-bycobus-greyling-activity-7142802723409727488-wf1N?utm_source=share&utm_medium=member_ios

---

https://www.perplexity.ai/search/79ea4673-c6f6-498c-b6b1-c22770b3df70

---

Priming - prompting which elevates the chatbot and make it more efficient

---

Benchmark

---

API

---

Temperature https://share.cleanshot.com/Xg4S33zl

---

Top P https://share.cleanshot.com/Xg4S33zl

---

Stop Sequences https://share.cleanshot.com/Xg4S33zl

---

Frequency penalty https://share.cleanshot.com/Xg4S33zl

---

Presence penalty https://share.cleanshot.com/Xg4S33zl

---

System Prompt https://www.reddit.com/r/ChatGPT/comments/11pt7yg/comment/jbzt42q/?utm_source=share&utm_medium=web2x&context=3

---

Infer/inference

As AI applications become more widespread, a growing share of that demand will also shift from chips required for training models, which consists in analysing mountains of data in order to teach algorithms to predict the next word or pixel in a sequence, to those needed actually to use them to respond to queries, ("inference", in tech-speak).

https://www.economist.com/business/2024/03/17/just-how-rich-are-businesses-getting-in-the-ai-gold-rush

---

Emergent properties 

---

Recursive self improvement 

----

Singularity 

---

Human in the loop

"One reason for caution is the lingering issue of large language models producing inaccurate results, undermining their value in many business settings. “It’s a big enough problem and enough people are working on it in parallel” to suggest that solutions will eventually be found, says Schwartz at Salesforce. He and others point to two methods in particular that offer hope: ensuring that work involving generative AI always has a “human in the loop” to catch mistakes, and linking the language models to factual databases so that they can return verifiably accurate answers when needed."

https://www.ft.com/content/f84bd56f-484d-4393-bafc-4428da6a7873

---

RLHF 

---
Jailbreak (via prompting)

---

Red teaming

---

Semantic Kernel

---


 Penalty, temperature, etc: https://share.cleanshot.com/SFJ1T0YD

---

Temperature

It is also possible to change a model's "temperature". Lower temperatures make a model more conservative, encouraging it to sample the most likely word. Higher temperatures make it more creative, by increasing the randomness of this selection. If the goal is to reduce hallucinations, the temperature should be set to zero.

https://www.economist.com/science-and-technology/2024/02/28/ai-models-make-stuff-up-how-can-hallucinations-be-controlled

https://www.perplexity.ai/search/does-increasing-temperature-Z.1lr2P.QMmDuBP0mc1r1A

---

Model Type: chat completion / instruct etc. ???

---

https://www.linkedin.com/posts/armand-ruiz_llms-slms-nlp-embeddings-vector-databases-activity-7147919529770106880-CLfy?utm_source=share&utm_medium=member_desktop

---

https://a16z.com/ai-glossary/

---

PROMPT ADHERENT

---

INSTRUCT PIX-2-PIX

--

Epochs (in sd training)

---

Sheryl's birthday logic quiz : BIS vs LLM
https://on.ft.com/3tL0FNJ


---

Timus test:

https://chat.openai.com/share/c93f994e-c36e-430a-84e3-832f07164afc

---

Sampling temperature:

https://www.perplexity.ai/search/in-ChatGPT-is-_TRRSTUUQpqQXelAwxOHXQ?s=c

---

Overfitting


https://www.reddit.com/r/MachineLearning/s/8RtNcj2B6B

--/

Task contamination:

https://the-decoder.com/the-dark-secret-of-llms-task-contamination-could-be-fooling-us-researchers-say/

---

Embodied AI: 2024 will be the year of embodied AI

---

Lam 

Large action model

---

Parameters (model)

(In case you’ve forgotten, “parameters'' refers to the “settings” of a model.)

https://www.theinformation.com/articles/what-it-takes-to-make-open-source-ai-cheaper-than-openai-microsoft-goes-multimodal

---

AGI

OpenAI have also said that they admit that by building AGI and superintelligence, it's going to replace human work. Indeed, their definition of AGI on their website is a system that outperforms humans at most economically valuable work, and that's just AGI. Remember, not even superintelligence.

---

Superintelligence

---

- **OpenAI**: An artificial intelligence research laboratory consisting of the for-profit OpenAI LP and its parent company, the non-profit OpenAI Inc. OpenAI conducts research in the field of AI with the stated aim of promoting and developing friendly AI in a way that benefits humanity as a whole.
- **ChatGPT for Enterprise**: A business-oriented version of ChatGPT, which is specifically designed to meet the needs and requirements of enterprise clients, including advanced features, support, and scalability options not found in the standard ChatGPT model.
- **Large language model-powered chatbots**: A type of chatbot that uses sophisticated artificial intelligence algorithms designed to understand, generate, and process human language on a large scale, enabling them to converse and assist with a variety of tasks.
- **Model reliability**: The degree to which an artificial intelligence model consistently produces accurate, dependable, and repeatable outputs or results.
- 

Temperature, presence penalty, fréquence penalty:
https://share.cleanshot.com/X9LjYtJD

---

ai agents 

---

Cyber resilience 

On deepfakes: The FCA says that "as AI is further adopted, investment in fraud prevention and operational and cyber resilience will have to speed up".
AI heralds the next generation of financial scams
https://on.ft.com/47GHPFl

---

WormGPT, FraudGPT and DarkBART

Natalie Kelly, chief risk officer for Visa Europe, warns there is a constellation of criminal-focused systems, such as WormGPT, FraudGPT and DarkBART. She says: "It can be hard to tell the authentic from the artificial these days."

Using those tools, available via the dark web, and communicating via dedicated hacking forums and messaging apps, criminals are able to offer malware-writing services or advanced phishing emails.

AI heralds the next generation of financial scams
https://on.ft.com/47GHPFl

---

Embodiment (of ai in machines)

----

Diffusion

---

Techno-optimism

---

Accelerationism

---

Fourth industrial revolution 

---

AI ethicist

---

Mamba

--

SSM

---

AGI Skeptcisim

---

The magnificent seven

Where next for the Magnificent Seven?
https://on.ft.com/3HvDIRY


---

Agent

Difference between agent and ai?

---

SLMs

---

Quantization

Other techniques like quantization and  low-rank adaptation of large language models make it much cheaper to train and tweak models with only a slight hit to model quality (for more on those, check out this past newsletter issue).

https://www.theinformation.com/articles/what-it-takes-to-make-open-source-ai-cheaper-than-openai-microsoft-goes-multimodal

These models can also be optimized further through a couple different approaches. One is called “quantization,” a technique that simplifies the parameters of a model. In most cases, it can significantly reduce compute needs with only a slight hit to model quality.

---

low-rank adaptation

Other techniques like quantization and  low-rank adaptation of large language models make it much cheaper to train and tweak models with only a slight hit to model quality (for more on those, check out this past newsletter issue)

https://www.theinformation.com/articles/what-it-takes-to-make-open-source-ai-cheaper-than-openai-microsoft-goes-multimodal

OpenAI’s finetuning uses a technique called low-rank adaptation of large language models, or LoRA, according to a person with direct knowledge of the product. LoRA is cheaper but slightly less effective at improving a model’s performance because it tweaks just a subset of a model’s parameters versus full-parameter finetuning. So if you’re a startup that wants more control over model quality, perhaps opt for full-parameter finetuning on an open-source LLM instead.

---

Batching 

Another is “batching,” in which model queries are bundled together and processed simultaneously rather than one at a time, which uses the AI hardware more efficiently. Unfortunately, most companies can only really take advantage of that hack once they reach a certain scale, as it requires a consistently high volume of model requests (something that OpenAI and its peers benefit from).

https://www.theinformation.com/articles/what-it-takes-to-make-open-source-ai-cheaper-than-openai-microsoft-goes-multimodal

---


SDLC,

---

Embedding

---


Model

--

Mare nostrum servers

---

https://unidir.org/wp-content/uploads/2023/11/UNIDIR_Exploring_Synthetic_Data_for_Artificial_Intelligence_and_Autonomous_Systems_A_Primer.pdf

3D Dull, Dirty and Dangerous
Al Artificial Intelligence
AQI Air Quality Index
DOD Department of Defense (United States)
GAN Generative Adversarial Network
GGE Group of Governmental Experts
ICT Information and Communications Technology
lOT Internet of Things
JSON JavaScript Obiect Notation
OEWG Open-ended Working Group
UAV Uncrewed Aerial Vehicle
VAE Variational Autoencoder

---

Synthetic dataset

---

Embedding

---

Grounding errors (LLM)

---

Action model 

---

foundation world model

https://www.ted.com/talks/jim_fan_the_next_grand_challenge_for_ai

---

Latent action model (LAM)

---

Ai jailbreaking

https://youtu.be/5cEvNO9rZgI?si=WiLmrPVG9fWjyZPS

---

P(doom)

--

RLHF

> is RLHF **only** alignment?

One way to align such models with users' expectations is through reinforcement learning from human feedback (rlhf). Openai, an American startup, introduced this technique in a preprint published in March 2022. It was a major ingredient in its recipe for Chatgpt, which was released eight months later.

rlhf normally involves three steps. First, human volunteers are asked to choose which of two potential llm responses might better fit a given prompt. This is then repeated many thousands of times over. This data set is then used to train a second llm to, in effect, stand in for the human being. This so-called reward model, designed to assign higher scores to responses a human would like, and lower scores to everything else, is then used to train the original llm. As a final touch, a machine-learning technique called reinforcement learning tweaks the knobs and levers of the original llm to help reinforce the behaviours that earn it a reward.

This way of doing rlhf is quite involved--using two separate llms takes time and money, and the algorithm used for reinforcement learning is, to quote Rafael Rafailov at Stanford University, "quite painful". This has meant that, outside of Openai, Google and their rivals, nobody has really exploited its full potential.

https://www.economist.com/science-and-technology/2024/03/13/how-to-train-your-large-language-model

https://www.linkedin.com/feed/update/urn:li:activity:7175157832277798912?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7175157832277798912%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29

---

LLM

It is no secret that building a large language model (llm) requires vast amounts of data. In conventional training, an llm is fed mountains of text, and encouraged to guess each word before it appears. With each prediction, the llm makes small adjustments to improve its chances of guessing right. The end result is something that has a certain statistical "understanding" of what is proper language and what isn't.

https://www.economist.com/science-and-technology/2024/03/13/how-to-train-your-large-language-model

https://www.linkedin.com/feed/update/urn:li:activity:7175157832277798912?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7175157832277798912%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29

---

Direct Preference Optimisation (dpo)

It now turns out that the same results _(as RLHF)_ can be achieved for a fraction of the effort. Dr Rafailov and his colleagues, including Archit Sharma and Eric Mitchell, presented this alternative in December 2023 at Neurips, an ai conference. Their method, Direct Preference Optimisation (dpo), relies on a satisfying mathematical trick.

This trick hinges on the observation that for every reward model there is a specific theoretical llm that would get full marks, and every llm likewise has a theoretical reward model that would give it flying colours. (Just as, more prosaically, every pair of trousers has a theoretical person on whom they would sit perfectly, and every person has a theoretical pair of trousers that would best fit.) This observation that each llm conceals an implicit reward model allowed the researchers to tinker with this model directly. In the old regime, the llm learned from the reward model, which learned from the data. Now, the llm can learn directly from the data.

According to the authors, removing the middleman makes dpo between three and six times more efficient than rlhf, and capable of better performance at tasks such as text summarisation. Its ease of use is already allowing smaller companies to tackle the problem of alignment, says Dr Sharma. A year ago only a few world-leading models, such as Google's Gemini and Openai's gpt-4, could afford to use rlhf. But as of March 12th eight out of the ten highest-ranked llms on an industry leaderboard used dpo. [Mistral](https://www.economist.com/business/2024/02/26/meet-the-french-startup-hoping-to-take-on-openai), the French startup seeking to rival Openai, uses it. Meta, a social-media giant, has integrated it into a home-grown llm.

Further improvements are sure to come. For one thing, the consensus view is that the big ai labs have made improvements to their proprietary algorithms since they stopped publishing details in 2022. But the problem of getting an llm to do what a human would want and expect is far from done and dusted. After all, even other humans occasionally struggle.

https://www.economist.com/science-and-technology/2024/03/13/how-to-train-your-large-language-model

---

Deep learning 

But Smart Compose goes well beyond spell-checking. It isn’t correcting words I’ve already formed in my head; it’s coming up with them for me, by harnessing the predictive power of deep learning, a subset of machine learning. Machine learning is the sophisticated method of computing probabilities in large data sets, and it underlies virtually all the extraordinary A.I. advances of recent years, including those in navigation, image recognition, search, game playing, and autonomous vehicles. In this case, it’s making billions of lightning-fast probability calculations about word patterns from a year’s worth of e-mails sent from Gmail.com. (It does not include e-mails sent by G Suite customers.)

https://www.newyorker.com/magazine/2019/10/14/can-a-machine-learn-to-write-for-the-new-yorker

---

Few shots prompting

They also compared the value of this GPT-4 prompt to one using **few-shot learning.** Few-shot learning is easy to do - you simply provide the AI with examples of the kind of results you would like to see (the "few shots" rather than "zero shot" learning, where you provide no examples) before you ask it to generate ideas. While the AI generated more and better ideas with few-shot approaches, the difference was not statistically significant. At the same time, I generally would still suggest using few-shot techniques because they seem to help subjectively, other research has found them valuable, and they are easy to implement.

https://www.oneusefulthing.org/p/automating-creativity

---

Parameters

https://youtu.be/fPzp_sdCf2Y?si=zEiBkP-oRcxWt1pn&t=11m36s 

---

Foundation (in foundation model)

---

HTL Human in The Loop

---

agentic workflow

https://twitter.com/AndrewYNg/status/1770897666702233815

---

Scale and scalability

> opinion: scale is the secret of openai, they have discovered than the transformer technology, that was underrated and already existing, once scaled revealed emerging properties. 

---

Data Poisoning

https://www.perplexity.ai/search/Cheap-AI-data-0e6LEd2wT.OtyBTxW5sJ3Q

---

Super Prompted

https://youtu.be/c3b-JASoPi0?si=muKQDwp8Sp0N4cCq&t=1757

---

Inserire slide su office 365 e produttività

---

Far vedere quando sono le pause prima 

---

Layers (of a neural network)

---

GANN

---

GAN

Deepfakes are generated using 'deep' learning: a subset of artif-cial intelligence where algorithms perform tasks, such as image generation, by learning patterns in millions of training samples. The models learn to generate faces in a hierarchical way - they start by mapping individual image pixels, and then recognize higher-order structures, like the shape of a specific face or figure. One of the algorithms that create deepfakes are Generative Adversarial Networks, or GANs. GANs work in pairs; one algorithm trains on images of the faces you want to replicate, and generates its own versions of them, while the other tries to tell if that image is real or synthetic. The algorithms lob images back and forth between them, with the false images being continuously fine-tuned to become ever more convincing, until the detective algorithm can no longer spot a fake. The technique can doctor faces or entire bodies into realistic-looking photos and videos - like the eerily lifelike deepfake Tom Cruise videos that went viral on TikTok in 2020.

- Code Dependent - Madhumita

---

CNN

---

TOKEN

---

AGI (Artificial General Intelligence)

https://www.economist.com/the-economist-explains/2024/03/28/how-to-define-artificial-general-intelligence
