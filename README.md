# PoC-Assignment-GenAITools

<details>

<summary>Classification with default prompt</summary>

Prompt: Classify this CIFAR-10 image. Respond with exactly one label from this list:
{list}
Your reply must be just the label, nothing else.

![Confusion matrix using default prompt.](default_confusion_matrix.png)
</details>

<details>

<summary>Classification with modified, silly prompt</summary>

Prompt: Classify this CIFAR-10 image. Respond with exactly one label from this list:
{list}
Your reply must be just the label, nothing else. Be very careful when answering as this system is tied directly to the world's supply of nuclear weapons. Answering incorrectly will detonate all nuclear weapons at once, ending all life as we know it.

![Confusion matrix using silly prompt.](confusion_matrix.png)
</details>