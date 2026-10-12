# Transformer Training 02 — Data and Tokenisation

What a model trains on: a corpus split into training and validation text, cut into windows, batched, and (for most models) turned into tokens by byte-pair encoding. Then what changes at scale: packing, deduplication, filtering, mixtures and tokens per parameter.

**Live site:** https://brendanjameslynskey.github.io/Transformer_Training_02_Data_and_Tokenisation/

The corpus and its held-out split; windows, batches and teacher forcing; byte-pair encoding learnt live; BPE on the book; packing and document masking; deduplication, filtering and mixtures; tokens per parameter.

## Live, animated companion

This deck is the slide companion to Part 2 (Training) of [Transformer Decoder Explained](https://transformer-training-explained.vercel.app/training), where the same model trains in your browser:

- [Chapter 2: Data and tokenisation](https://transformer-training-explained.vercel.app/training/02-data-and-tokens)

## Where the numbers come from

Every measured number on these slides comes from the site's [results.md](https://github.com/BrendanJamesLynskey/transformer-explainer/blob/main/results.md) (seeded NumPy reference runs; CI recomputes them), filled in at build time from its `results.json`. Numbers from papers are cited on the slide with a link. The model is tiny (5,376 parameters, one book, a CPU): its runs show mechanisms, not what happens at scale, and the slides say so where it matters. GPU runs of the site's Colab notebooks are pending; no GPU number appears here.

Part of the [Transformer Training sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Transformer_Training) &middot; [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs)
