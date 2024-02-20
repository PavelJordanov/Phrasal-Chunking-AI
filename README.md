# Robust Phrasal Chunking with Adversarial Training

## Project Description

This project aims to enhance the robustness of natural language processing (NLP) models in the sub-task of phrasal chunking, which involves identifying and categorizing non-recursive syntactic groups of words in sentences. Leveraging the CoNLL 2000 shared task dataset, our model is particularly focused on generalizing well to noisy, real-world data, which may contain various types of input noise such as typographical errors or misspellings.

### Background

Phrasal chunking, a crucial step in understanding the structure of sentences, divides text into syntactically correlated chunks of words. Despite its success in syntactic parsing, the precision of NLP models dramatically decreases when encountered with noisy input, limiting their use in various real-world applications.

### Challenge

The project tackles the challenge of improving phrasal chunking accuracy in the presence of misspellings and other synthetic noise by using adversarial training. By simulating a set of noisy patterns, such as common spelling mistakes, during the training phase, our NLP model will be attuned to a more raw and original format of user input.

### The Data

The data for this model originates from the CoNLL 2000 shared task, enhanced with simulated noisy samples for the rigors of this specific project. A part-of-speech (POS) and chunk tagging are utilized to transform the extant clean sentences into formats affording the network the chance to predict precise phrasal bits.

### Architectural Adjustments

The optimization of this project was executed by applying dual optimizers with distinct learning rates: a more aggressive learning rate for the adjustment of the model’s classificatory branch, and a more methodical one for the multi-stage pre-trained encoder network. 

### Innovative Upgrade

1. **Adversarial Training**: Our project framework magnifies the strategy of misspelling simulation to prompt deep resilience of the NLP text in phrasal chunking. Mimicking a world with habitual or abrupt typing snags, this data modulation engrains the solutioning dexterity for a differentiated and differential world of typos.

2. **Tweaking at the Solver Level**: Realizing a slope in the learning curve by partitioning the learning rates between the pre-trained encoder layers and the succeeding classification head, we funneled in a hybrid technique to 'fine-coarse' learning schema.
