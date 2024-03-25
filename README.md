# Speaker Classification

This project focuses on the classification of speakers in speech signals. The model has achieved a remarkable accuracy rate of **97.06%** on the task, ranking in the **top 6% out of 1000 teams**.

## Data Preprocessing

The original dataset utilized is [VoxCeleb](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/). Data preprocessing involved transforming it into vectors using mel-frequency cepstrum. Initially, the signal was converted into the frequency domain using Discrete Fourier Transform to obtain a spectrum. Subsequently, a filter bank, log transform, and Discrete Cosine Transform were applied to construct the vector. A window length of 128 was randomly chosen from the vectors. The processed dataset is stored [here](https://drive.google.com/file/d/1xOFUZZRlcURtqnXTg1FyftW4ztwUGQNi/view?usp=sharing).

## Model Training

The constructed model, based on [Conformer](https://arxiv.org/abs/2005.08100), undergoes rigorous training using the preprocessed dataset to optimize its parameters and achieve the desired predictive performance.

## Model Improvement Techniques

To enhance model performance, the following techniques were employed:

1. [Additive Margin Softmax](https://arxiv.org/abs/1801.05599)
2. Cosine learning rate scheduler

## Dataset

The preprocessed VoxCeleb dataset serves as the primary data source for this project, accessible [here](https://drive.google.com/file/d/1xOFUZZRlcURtqnXTg1FyftW4ztwUGQNi/view?usp=sharing).  

For detailed implementation and usage instructions, please refer to the provided [code](https://github.com/Dawson-ma/Speaker-Classification/blob/main/Speaker_classification.ipynb).
