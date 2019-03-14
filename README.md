# Scandinavian ULMFiT

Inductive transfer learning has greatly impacted computer vision, but existing approaches in NLP still require task-specific modifications and training from scratch.

This repository contains the weights for the embedding layer of a UMLFiT language model that can be used as the first step in fine-tuning any Natural Language Processing task.

The weights were trained on 90% of all text in the corresponding language wikipedia as per 3. July 2018. The remaining 10% was used for validation.

# Supported Languages:

- Danish

Trained on 78,373,122 tokens, and validated on 7,837,310 tokens. We achieve a perplexity of 30.9.

- Norwegian

Trained on 80,284,231 tokens, and validated on 8,920,387 tokens. We achieve a perplexity of 26.31.

- Finnish

Trained on 68,775,370 tokens, and validated on 7,641,571 tokens. We achieve a perplexity of 27.66

Training even higher performance models is possible, but require more (costly) training time. If you need a model with higher performance, feel free to contact us.

### Paper

See Universal Language Model Fine-tuning for Text Classification, Jeremy Howard, Sebastian Ruder, https://arxiv.org/abs/1801.06146

### File descriptions

- enc.h5  Contains the weights in 'Hierarchical Data Format'

- enc.pth  Contains the weights in 'Pytorch model format'

- itos.pkl (Integers to Strings) contains the vocabulary mapping from ids (0 - 30000) to strings

### Sponsor

This work was sponsored by Danish chatbot company BotXO
http://www.botxo.co/

### Thanks 

Thanks to Tobias Lindberg from Damvad Analytics for converting the vectors to pth-format.
