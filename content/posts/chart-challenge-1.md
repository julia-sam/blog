+++
title = 'Comparing "Internet" Usage Across Languages'
date = 2024-08-28T21:01:16-04:00
draft = false
+++

![Retro Computer](./computer-old.jpeg)

Language can tell us a lot about societal trends, technological advances, and cultural shifts. Tools like [Google Ngrams](https://books.google.com/ngrams/) have provided a way to see these trends and explore the frequency of words and phrases across centuries of literature. 

Inspired by this, I wanted to explore something similar but across multiple languages and then be able to visualize it. I found an Ngrams API (based off of Google Ngrams) and created some charts across English, German, and Russian.

I started off by exploring some historical trends of the term "internet" across languages using charts which revealed some interesting insights.

{{< resizeimg src="./english.png" alt="eng" width="550" >}}

"Internet" usage started growing fast in the early 1990s in the English corpus, peaking around 2000. This aligns with the global expansion of internet access and its integration into everyday life. Interestingly, the usage began to decline after this peak, possibly reflecting the emergence of new technologies and terminologies.

{{< resizeimg src="./german.png" alt="ger" width="550" >}}

Similar to the English data, the German corpus shows a sharp increase in the usage of "Internet" starting in the 1990s.

{{< resizeimg src="./russian.png" alt="rus" width="550" >}}

Russian data has a unique pattern. Significant usage of the term "Интернет" (internet) only began after 2000, with a dramatic increase after 2010. This suggests a later but more intense adoption of the term in Russian.

{{< resizeimg src="./treemap.png" alt="treemap" width="750" >}}

To put it all together and compare all three languages, I created a treemap that shows the usage of "Internet" in 2019 across English, German, and Russian. With the historical context in mind, I chose to focus on the year 2019 because by this time, the term "Internet" had established itself across all three languages, making it an ideal year to analyze how each language's usage contributes to the whole.