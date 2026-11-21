---
layout: about
title: about
permalink: /
subtitle:
profile:
  align: right
  image: profile_pic.jpg
  image_circular: true # crops the image to make it circular

news: true # includes a list of news items
selected_papers: true # includes a list of papers marked as “selected={true}”
social: true # includes social icons at the bottom of the page
---
I am a final-year Data Science undergraduate at the Indian Institute of Information Technology Nagpur, advised by [Prof. Jitendra Tembhurne](https://code7wormer.github.io/profilepage/). I am currently a visiting student at the Singapore University of Technology and Design under [Prof. Ezekiel Soremekun](https://ezekiel-soremekun.github.io/). At Nanyang Technological University, I work on hallucination mitigation strategies in medical LLMs under [Prof. Erik Cambria](https://www.sentic.net/erikcambria/).

**Interests:** AI Safety · Mechanistic Interpretability · Representation Learning · AI Security · Trustworthy AI

I started in computer vision, trying to understand what happens when a model sees many examples of some classes and very few of others. The familiar result was that it favored the common classes. I explored ways to adjust its decisions and training so that rare classes would not be overlooked, but I kept coming back to a deeper question: what had the model learned about those classes in its feature space?

That question led me to neural collapse and the geometry of learned representations. Late in training, features can gather around class means while classifier weights align with those means. Under imbalance, rare classes can still sit too close to visually similar neighbors. We used the angles between normalized classifier prototypes to measure this semantic crowdedness and brought that signal into logit adjustment alongside class frequency. Seeing how much could be learned from the shape of a feature space made me want to look inside other models, too.

I then had the chance to work on LLM safety. With code language models, I began investigating how jailbreak prompts affect embeddings and hidden activations, and whether those internal changes can help us understand and defend against them. In medical LLMs, I am now exploring strategies to mitigate hallucinations, where a fluent answer can still be unsupported or misleading. The thread through all of this work is my interest in using a model's internal behavior to understand its failures and make its outputs more dependable.
