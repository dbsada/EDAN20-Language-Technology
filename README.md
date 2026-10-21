<div align="right">
  🇬🇧 English | <a href="README-ES.md">🇪🇸 Español</a>
</div>

# EDAN20 — Language Technology

This repository contains the labs I completed for the course **EDAN20 – Language Technology** at [LTH](https://www.lth.se/), the Faculty of Engineering at Lund University (Sweden). Across the labs, several of the core algorithms and models of Natural Language Processing (NLP) have been implemented, building on the templates provided by the course instructor, [Pierre Nugues](https://github.com/pnugues/edan20).

## Labs

### 1. Probabilistic Spelling Corrector — [`01-spelling-corrector`](01-spelling-corrector/spell.ipynb)

A spelling corrector based on Peter Norvig's design. It generates candidate words using the Damerau–Levenshtein edit distance, validates them against the corpus vocabulary, and selects the most likely correction via Maximum A Posteriori (MAP) estimation.

### 2. Inverted Index — [`02-indexer`](02-indexer/indexer.ipynb)

Builds an inverted index (posting lists) over the Selma Lagerlöf corpus: tokenization, positional indexes, a master index, concordances, and TF-IDF document representation to compare novels.

### 3. N-grams and Language Models — [`03-n-grams`](03-n-grams/n-grams.ipynb)

Language models based on unigrams, bigrams, and trigrams: sentence segmentation, perplexity and entropy, unigram backoff, and online next-word prediction. Includes a word segmenter (unigram and bigram) adapted from Norvig's *How to do things with words* ([`segmentation.ipynb`](03-n-grams/segmentation.ipynb)).

### 4. BPE and Unigram Tokenizers — [`04-tokenization`](04-tokenization/tokenization.ipynb)

Character-level subword tokenizers (BPE and Unigram) implemented from scratch and compared against the SentencePiece library.

### 5. Language Detector — [`05-language-detector`](05-language-detector/language-detector.ipynb)

A simplified version of Google's Compact Language Detector (CLD3): character n-grams mapped with the hashing trick, a classifier trained with scikit-learn and reimplemented in PyTorch.

### 6. Sentence Embedder (SBERT) — [`06-sbert`](06-sbert/sbert.ipynb)

A transformer-based sentence embedder with mean pooling, inspired by Sentence-BERT, trained on the SNLI corpus and compared against a mean-GloVe baseline using cosine similarity.

### 7. Translation Transformer — [`07-translation-transformer`](07-translation-transformer/translation-transformer.ipynb)

A character-level machine translation system (English ↔ Spanish) built on the encoder–decoder Transformer architecture (*Attention Is All You Need*), evaluated with sentence-level BLEU.

## Data note

The corpora used in the labs (Selma Lagerlöf, SNLI, Tatoeba, and the GloVe embeddings) and most trained model artifacts are not included in this repository. The notebooks either download or reference them; check each notebook for the expected paths.

## Credits

Course templates by [Pierre Nugues](https://github.com/pnugues/edan20/tree/master/labs_2026).

## Author

- [Diego Besada](https://github.com/dbsada)
