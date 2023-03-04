# Tokenization

<p> Pre-processing teks adalah langkah pertama yang perlu disiapkan sebelum membuat model NLP.

## Teks Sebagai Data Tidak Terstruktur
Dalam dunia nlp, kita akan sering ketemu sama yang namanya teks, tweet, dan suara. Data-data tersebut bersifat tidak terstruktur. Mereka diberi nama **Corpus** atau **Unstructured Data**. Tugas kita adalah mengubah data-data tersebut menjadi lebih terstruktur.!

## Langkah Pertama dalam Pre-Processing
![Alt text](Picture-1.png)
Dokumen akan disegmentasi menjadi kalimat. Kemudian kalimat akan disegmentasi menjadi **Token**. Token biasanya adalah _kata_. Akan tetapi, _tanda baca_ dan _angka_ juga termasuk token.

## Tantangan dalam Tokenisasi
![Alt text](Picture-2.png)
![Alt text](Picture-3.png)
![Alt text](Picture-4.png)

## Hands On
https://colab.research.google.com/github/nitinpunjabi/nlp-demystified/blob/main/notebooks/nlpdemystified_preprocessing.ipynb