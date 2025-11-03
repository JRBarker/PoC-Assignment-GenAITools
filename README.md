# PoC-Assignment-GenAITools

How to run:

- Install Python (Created using Python 3.13.3, but other similar version should also work)
- Clone this repo
- Open a terminal in this project's directory
- Run `pip install -r requirements.txt`
- Create `.soonerai.env` in the repo's directory
- Add your API key to `.soonerai.env` (API keys can be created at https://ai.sooners.us) and SAVE
- Run `cifar10_classify.py`

For this example trial featuring different prompts, each prompt was run once. The 'silly'
prompt warning of nuclear obliteration appeared to perform better than the default prompt, but without multiple runs it's difficult to say that this is significant. Multiple runs with different seeds must be done to establish if this prompt does anything or if this variance is due to noise.

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