# Danish ULMFiT

Inductive transfer learning has greatly impacted computer vision, but existing approaches in NLP still require task-specific modifications and training from scratch.

This repository contains the weights for the embedding layer of a UMLFiT language model that can be used as the first step in fine-tuning any Natural Language Processing task.

The weights were trained on 90% of all text in the Danish Wikipedia as per 3. July 2018. The remaining 10% was used for validation.

We achieve a perplexity of 30.9 on the validation data.

### Paper

See Universal Language Model Fine-tuning for Text Classification, Jeremy Howard, Sebastian Ruder, https://arxiv.org/abs/1801.06146

### File descriptions

- dawt.h5  (Danish WikiText) contains the weights in 'Hierarchical Data Format'

- itos.pkl (Integers to Strings) contains the vocabulary mapping from ids (0 - 30000) to strings

### Sponsor

This work was sponsored by Danish chatbot company BotXO
http://www.botxo.co/
