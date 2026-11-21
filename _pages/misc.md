---
layout: page
permalink: /misc/
title: misc
nav: true
nav_order: 2
---

#### experience

- **Visiting Student**, Singapore University of Technology and Design · Singapore (July 2026 – present)<br>
  Working with Prof. Ezekiel Soremekun on jailbreaks in code LLMs, studying embeddings and internal activations to understand and defend against them.
- **Research Intern**, Nanyang Technological University · Singapore (May 2026 – present)<br>
  Working with Prof. Erik Cambria on hallucination mitigation strategies in medical LLMs.
- **Research Contributor**, Nvtha AI · Singapore (August 2026 – present)<br>
  Contributing to hallucination detection research using representation-based signals, evaluation, and failure analysis for LLM workflows.
- **Undergraduate Researcher**, Indian Institute of Information Technology Nagpur · India (September 2025 – May 2026)<br>
  Worked with Prof. Jitendra Tembhurne on logit adjustment methods to handle imbalanced datasets.
- **Research Intern**, Indian Institute of Technology Hyderabad · India (May 2025 – July 2025)<br>
  Worked with Prof. Sidhardh on a U-Net model to predict strain maps from experimental images and automate crack-tip localization.

My full CV is [here](/assets/pdf/cv.pdf).

<br>

#### projects

- [Neural network from scratch in C++](https://github.com/brainardphilemon/neuralnetwork-in-cpp): A configurable feedforward network built with the C++ standard library. It trains with ReLU activations, backpropagation, and gradient descent for regression on housing data.
- [Sparse strain field prediction with U-Net](https://github.com/brainardphilemon/sparse-strainfield-generation): A U-Net predicts three strain components from microscopic speckle images. A masked loss lets it learn from the small fraction of pixels with valid measurements.
- [A backdoor defense for language models](https://github.com/brainardphilemon/A-Backdoor-Defense-for-LLMs): An extension of ONION that studies leave-one-out embedding shifts and early-layer signals to identify textual backdoor triggers.

<br>

#### some writings

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) ({{ post.date | date: "%b %Y" }})
{% endfor %}
