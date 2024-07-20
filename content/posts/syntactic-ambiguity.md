+++
title = 'ChatGPT vs Claude: Ambiguity Resolution (Part I)'
date = 2024-05-28T12:12:38-04:00
draft = true
sectionPagesMenu = 'main'
+++
![Ambiguous images](/ambiguous-img.jpeg)

### *"One morning I shot an elephant in my pajamas." - Groucho Marx*

Syntactic ambiguities occur when a sentence can have multiple meanings. For example, consider the sentence from the famous Groucho Marx joke above. This sentence is ambiguous because it's unclear whether the elephant was in pajamas or Groucho Marx was in pajamas while shooting the elephant. If you're curious which interpretation Groucho Marx meant, here is the full quote: *"One morning I shot an elephant in my pajamas. How he got into my pajamas I’ll never know."*

It's easy enough for a human being to understand the two interpretations, and thanks to common sense or when given more context, it's possible to disambiguate the phrase. On the other hand, chatbots and even the latest large language models (LLMs) struggle with these types ambiguous inputs. Here are two reasons: (1) LLMs aren't trained to handle very ambiguous inputs well; (2) the ambiguity level can vary depending on the LLMs' knowledge, making it difficult to investigate. 

I'm currently working on an experiment where I look at *temporary syntactic ambiguities* which occur when the beginning of a sentence can have multiple meanings. I investigate how LLMs generate sentence completions after being fed ambiguous partial sentences. 

I was initially inspired by [this paper](https://arxiv.org/abs/2109.07848) where the researchers look at whether langauge models show uncertainty when processing ambiguous sentences and how this uncertainty changes with context clues. They generate multiple sentence completions from the LMs (GPT-2 and an LSTM), analyze them, and measure the probability the LMs assign to different interpretations. The findings suggest that LMs can keep track of multiple possible analyses at once, and while they often pick the correct interpretation when given clues, they still make mistakes, which means there is room for improvement.