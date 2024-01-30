# TinyStories: How Small Can Language Models Be and Still Speak Coherent English?

This week's paper is [*TinyStories: How Small Can Language Models Be and Still Speak Coherent English?*](https://arxiv.org/abs/2305.07759)

TinyStories is an interesting paper for two reasons. First it's one of, if not the first, paper to use fully synthetic data for pretraining a language model. Second, it and similar datasets allow for us to practice pretraining language models in a reasonable amount of time on consumer hardware.

Small Pretraining Datasets:
* TinyStories: [Base](https://huggingface.co/datasets/roneneldan/TinyStories), [Instruct](https://huggingface.co/datasets/roneneldan/TinyStoriesInstruct), [Instruct-Standardized](https://huggingface.co/datasets/HydraLM/TinyStoriesInstruct-standardized)
* Tiny-Datasets: [TextBooks](https://huggingface.co/datasets/nampdn-ai/tiny-textbooks), [Code](https://huggingface.co/datasets/nampdn-ai/tiny-codes), [Web](https://huggingface.co/datasets/nampdn-ai/tiny-webtext), [Lessons](https://huggingface.co/datasets/nampdn-ai/tiny-lessons), [Multi-lingual](https://huggingface.co/datasets/nampdn-ai/tiny-bridgedict) 
* Clean Code: [Code](https://huggingface.co/datasets/vikp/clean_code), [Notebooks](https://huggingface.co/datasets/vikp/clean_notebooks), [PyPi](https://huggingface.co/datasets/vikp/pypi_clean)
* [Simple Wikipedia](https://simple.wikipedia.org/wiki/Main_Page): would need to be created from scratch from a wiki dump
* [MiniPile](https://huggingface.co/datasets/JeanKaddour/minipile): a small subset of The Pile

Training Time:

A 3-4GB dataset will take somewhere between 1-6 hours per epoch on a 25m-120m model at 256 sequence length with a high end consumer card. See [this table](http://benjaminwarner.dev/2023/08/16/flash-attention-compile.html#results) for an idea of what that translates too with larger context lengths and model sizes.