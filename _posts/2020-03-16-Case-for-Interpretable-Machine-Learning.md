---
toc: true
layout: post
description: Why should you care about the black box?
categories: [Interpretable Machine Learning], [Natural Language Processing]
title: A Case for Interpretable Machine Learning
---

From video recommendation, autonomous vehicles to predictive medicine, machine learning(ML) systems are ubiquitous in decision making process. ML systems are often labeled as black-box models, since their complexity makes it challenging for human evaluation or understanding. Recently, Geoffrey Hinton, one of the founders of deep learning, tweeted the following:

{% twitter https://twitter.com/geoffreyhinton/status/1230592238490615816?s=20 %}

This post spurred large discussions about interpretable ML systems and whether explanation for their outputs are necessary. In this scenario, I believe that the scalability and cost will nudge the user’s decision, but that’s a huge topic appropriate for a future post of its own. As pointed out in many interpretability papers[^1] ML systems for performance does not address important criteria such as nondiscrimination, safety, or right to explanation by end-users or legal systems. Ignoring any of these criteria could lead to alarming consequences, but unlike measures of performance, these criteria are usually difficult to quantify. For example, HR system may discriminate applications based on many confounders that may not be obvious to the recruiter. To address such cases, ML researchers are developing methods to measure interpretability; or the ability to explain ML systems in understandable terms to human.

One of the most widely used method for interpretable machine learning is the attention mechanism. The attention mechanism has dramatically improved the performance in many domains such as natural language processing, but it also provides insights for interpretability. The main idea is this: each time the model generates an output, it only refers small part of the input that is most relevant to the output. By quantifying the level of input relevance, users can evaluate which part the data the model is most attentive to. For a more in-depth explanation, check out these great posts [Attention? Attention!](https://lilianweng.github.io/lil-log/2018/06/24/attention-attention.html) by Lilian Weng and [The Annotated Transformer](https://nlp.seas.harvard.edu/2018/04/03/attention.html). Note that the transformers are a variant of attention model that revolutionized natural language processing in recent years.

In the following weeks, I will present some interesting papers that show strengths and limitations of attention mechanism. Please stay tuned.

### Acknowledgments
[^1]:References terminologies from 'Towards A Rigorous Science of Interpretable Machine Learning' by Finale Doshi-Velez and Been Kim.