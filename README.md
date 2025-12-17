# BART Summarization Exploration

This mini-project explores abstractive summarization using a pretrained transformer model,
`facebook/bart-large-cnn`, applied to a real-world long-form science article from *The New York Times*. Check out the [model card](https://huggingface.co/facebook/bart-large-cnn) on Hugging Face.

The goal is not to optimize summarization quality, but to understand **where and why a strong pretrained model breaks** when applied outside its training distribution.

## What this notebook covers
- Running abstractive summarization using Hugging Face’s `pipeline` API
- Comparing summaries from short excerpts vs. full-length articles
- Diagnosing degradation due to context window limits and attention dilution
- Understanding why long-form text is challenging for BART
- Outlining next steps: chunking, using long-context models, and tuning generation parameters

## Notebook
- `bart_summarization_exploration.ipynb`

## Next steps
- Chunking text, and summarizing summaries
- Exploring long-context models ([LED](https://huggingface.co/docs/transformers/en/model_doc/led?usage=Pipeline) and [LongT5](https://huggingface.co/docs/transformers/en/model_doc/longt5))
- Tuning generation parameters for beter abstraction
