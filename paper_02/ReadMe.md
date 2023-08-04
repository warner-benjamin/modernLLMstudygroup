# Finetuned Language Models Are Zero-Shot Learners

This week's paper is [*Finetuned Language Models Are Zero-Shot Learners*](https://arxiv.org/abs/2109.01652) on supervised fine-tuning.

Further Reading:
- [*Multitask Prompted Training Enables Zero-Shot Task Generalization*](https://arxiv.org/abs/2110.08207) 
- [Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2210.11416.pdf) 
- [The Flan Collection: Designing Data and Methods for Effective Instruction Tuning](https://arxiv.org/abs/2301.13688)

Code: 

https://github.com/google-research/FLAN

Metrics:

[ROUGE (metric)](https://en.wikipedia.org/wiki/ROUGE_(metric)) \
[What is the ROUGE metric (video from HF course)](https://www.youtube.com/watch?v=TMshhnrEXlg) \
[An intro to ROUGE, and how to use it to evaluate summaries](https://www.freecodecamp.org/news/what-is-rouge-and-how-it-works-for-evaluation-of-summaries-e059fb8ac840/) \
[Two minutes NLP — Learn the ROUGE metric by examples](https://medium.com/nlplanet/two-minutes-nlp-learn-the-rouge-metric-by-examples-f179cc285499)

Other Resources:

[HF NLP Course - Part 7: Summarization](https://huggingface.co/learn/nlp-course/en/chapter7/5?fw=pt#summarization) \
[Training summarization & translation models with fastai & blurr: W&B Study Group](https://www.youtube.com/watch?v=Jsz4E2iNXUA)

Notes:

* "These models have been fine-tuned on more that 1000 additional tasks covering also more languages" 
* Improves upon T5 with instruction finetuning with more tasks and including chain-of-thought data 
* Dataset = [samsum](https://huggingface.co/datasets/samsum) ("16k messenger-like conversations with summaries") 