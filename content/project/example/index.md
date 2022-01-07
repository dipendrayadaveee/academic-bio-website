---
slides: example
url_pdf: ""
summary: ""
authors: []
url_video: ""
date: 2022-01-07T01:00:00.000Z
external_link: ""
url_slides: ""
title: Exploring Transfer Learning for Deep NLP systems for rarely annotated langauges
subtitle: The goal of this thesis work is to explore transfer learning for the
  task of Part-of-speech(POS) tagging between Hindi and Nepali languages which
  are part of the Indo-Aryan language family with very high similarity.
tags:
  - Deep Learning
links:
  - icon: linkedin
    icon_pack: fab
    name: Follow
    url: https://www.linkedin.com/in/dipendra-yadav-eee/
image:
  caption: ""
  focal_point: Smart
url_code: ""
---
Natural language processing has seen exponential growth since deep learning has
been used for various tasks. Deep learning has replaced the old rule-based methods by
providing better performance on almost all the tasks in NLP, as deep learning basically
looks into the hidden patterns and structures in the data which were sometimes not
detected and at other-times overlooked by the rule-based systems. 

The research and development in NLP have been however focused on some handful languages of the world
given their financial importance and a huge number of speakers. This has left out most
of the other languages unexplored. The other reason for the lack of research in these
languages is the unavailability of properly annotated and the required amount of datasets
which is very important for training deep learning neural networks. The situation looks
grim. 

When we look at the world language tree, thankfully we see that most of the
unexplored languages have other well-explored languages nearby which basically means
that both the languages are kind of similar. So if we could somehow adapt research
and development from one language to another, it could be really helpful for both the
languages. The goal of this thesis work is to explore transfer learning for the task of
Part-of-speech(POS) tagging between Hindi and Nepali languages which are part of the
Indo-Aryan language family with very high similarity. We have tried to explore the
possibility of jointly training a model for the task of POS tagging in both Hindi and
Nepali language and see if it helps in improving the performance of the model. We also
try to explore if multitask learning in the Hindi language can be helpful for the task of
POS tagging with auxiliary tasks of the gender tagging and singularity/plurality tagging.
The deep learning architecture used for this work is BLSTM-CNN-CRF. The model is
trained with monolingual word embeddings, vector mapped embeddings, and also with
jointly trained Hindi-Nepali word embeddings in different setups with varying dropout
from 0.25 to 0.5 and using ADAM and AdaDelta optimizers. These modes were used to
train the models of individual languages, multitask learning in the Hindi language, and
transfer learning for the task of POS tagging between Hindi and Nepali language. 

It has
been observed that the jointly trained Hindi-Nepali word embeddings seem to improve
the performance of all the models, better than monolingual word embeddings and vector
mapped word embeddings. The default setup derived from Reimers et. al. \[1] seems to
help the model in its task of POS tagging. It has also been observed that multitask
learning doesn’t seem to help in the task of POS tagging in the Hindi language, on the
contrary, it degrades the performance. And for jointly training a model for the task of
POS tagging between Hindi and Nepali language, it also doesn’t seem to help in the
performance of the model.