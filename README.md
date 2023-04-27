This project aims to explore ways to measure and mitigate bias in GPT-2 language models. The project uses GPT-2 model and several techniques for measuring bias such as Regard score from Huggingface and WEAT score for embeddings. The project also runs Big-Bench tasks to evaluate the performance of the model.

The main focus of the project is to implement different debiasing techniques to mitigate the bias present in the model. Two techniques have been identified for this purpose:

Fine-tuning GPT-2 with transformer architecture changes: This technique involves freezing one or more layers of the GPT-2 model during the fine-tuning process. This will allow the model to learn from the dataset without the influence of the frozen layers, which can help reduce the bias in the output.

We will investigate the use of masking techniques to identify and modify the updates during the feedforward layers of the GPT-2 model. Specifically, we will de-weight the contribution of bias tokens during these updates to reduce their impact on the model's predictions.
To achieve this, we will first identify the tokens that are associated with biased language using existing bias measurement techniques. Then, we will use a masking technique to zero out the gradients for these tokens during the feedforward layers. This approach will effectively reduce the contribution of the biased tokens to the model's predictions.By de-weighting the impact of the biased tokens in this way, we expect to mitigate the effects of bias in the GPT-2 model and improve its overall performance.

This project will be updated with the results of the experiments conducted using these debiasing techniques. The project code is available on GitHub and contributions from the community are welcome.
