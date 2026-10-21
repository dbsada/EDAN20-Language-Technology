<div align="right">
  <a href="README.md">🇬🇧 English</a> | 🇪🇸 Español
</div>

# EDAN20 — Language Technology

Este repositorio recoge los laboratorios que he realizado para la asignatura **EDAN20 – Language Technology** en [LTH](https://www.lth.se/), la Facultad de Ingeniería de la Universidad de Lund (Suecia). A lo largo de los laboratorios se han implementado varios de los algoritmos y modelos fundamentales del Procesamiento del Lenguaje Natural (NLP), partiendo de las plantillas del profesor [Pierre Nugues](https://github.com/pnugues/edan20).

## Laboratorios

### 1. Corrector ortográfico probabilístico — [`01-spelling-corrector`](01-spelling-corrector/spell.ipynb)

Implementación de un corrector ortográfico basado en el diseño de Peter Norvig. Genera palabras candidatas mediante la distancia de edición de Damerau–Levenshtein, las valida contra el vocabulario del corpus y selecciona la corrección más probable con estimación MAP (máximo a posteriori).

### 2. Índice invertido — [`02-indexer`](02-indexer/indexer.ipynb)

Construcción de un índice invertido (posting lists) sobre el corpus de Selma Lagerlöf: tokenización, índices de posición, índice maestro, concordancias y representación de documentos con TF-IDF para comparar novelas.

### 3. N-gramas y modelos de lenguaje — [`03-n-grams`](03-n-grams/n-grams.ipynb)

Modelos de lenguaje con unigramas, bigramas y trigramas: segmentación de oraciones, perplejidad y entropía, backoff a unigramas y predicción en línea de la siguiente palabra. Incluye un segmentador de palabras (unigrama y bigrama) adaptado de Norvig ([`segmentation.ipynb`](03-n-grams/segmentation.ipynb)).

### 4. Tokenizadores BPE y Unigram — [`04-tokenization`](04-tokenization/tokenization.ipynb)

Tokenizadores de subpalabras a nivel de carácter (BPE y Unigram) implementados desde cero y comparados con la librería SentencePiece.

### 5. Detector de idiomas — [`05-language-detector`](05-language-detector/language-detector.ipynb)

Versión simplificada del Compact Language Detector (CLD3) de Google: n-gramas de caracteres mapeados con el hashing trick, un clasificador entrenado con scikit-learn y reimplementado en PyTorch.

### 6. Sentence embedder (SBERT) — [`06-sbert`](06-sbert/sbert.ipynb)

Codificador de oraciones basado en transformers con mean pooling, inspirado en Sentence-BERT, entrenado sobre el corpus SNLI y comparado con una línea base de medias de GloVe mediante similitud coseno.

### 7. Transformer de traducción — [`07-translation-transformer`](07-translation-transformer/translation-transformer.ipynb)

Sistema de traducción automática a nivel de carácter (inglés ↔ español) basado en la arquitectura encoder-decoder del Transformer (*Attention Is All You Need*), evaluado con BLEU a nivel de frase.

## Nota sobre los datos

Los corpus empleados en los laboratorios (Selma Lagerlöf, SNLI, Tatoeba y los embeddings GloVe) y la mayoría de los modelos entrenados no están incluidos en este repositorio. Los notebooks los descargan o referencian; consulta cada notebook para ver las rutas esperadas.

## Créditos

Plantillas de la asignatura de [Pierre Nugues](https://github.com/pnugues/edan20/tree/master/labs_2026).

## Autor

- [Diego Besada](https://github.com/dbsada)
