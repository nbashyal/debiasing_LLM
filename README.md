This project aims to explore ways to measure and mitigate bias in GPT-2 language models. The project uses GPT-2 model and several techniques for measuring bias such as Regard score from Huggingface and WEAT score for embeddings. The project also runs Big-Bench tasks to evaluate the performance of the model.

The main focus of the project is to implement different debiasing techniques to mitigate the bias present in the model. Two techniques have been identified for this purpose:

Fine-tuning GPT-2 with transformer architecture changes: This technique involves freezing one or more layers of the GPT-2 model during the fine-tuning process. This will allow the model to learn from the dataset without the influence of the frozen layers, which can help reduce the bias in the output.

Identifying updates during feed forward layer and de-weighting bias tokens during updates: This technique involves identifying updates during the feed forward layer of the model and de-weighting bias tokens during these updates. This will help reduce the impact of biased tokens on the final output of the model.

This project will be updated with the results of the experiments conducted using these debiasing techniques. The project code is available on GitHub and contributions from the community are welcome.
