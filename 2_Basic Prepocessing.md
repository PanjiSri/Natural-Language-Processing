# Basic Preprocessing

Ini merupakan lanjutan dari tokenization. Basic prepocessing adalah serangkaian langkah awal yang dilakukan untuk membersihkan dan mempersiapkan teks mentah untuk diolah lebih lanjut. Bagian ini dilakukan untuk menghilangkan noise atau gangguan pada teks, memperbaiki format, dan memperjelas struktur teks agar dapat diolah dengan baik melalui algoritma NLP.

Sebelum masuk ke jenis-jenisnya ada satu istilah yang perlu diketahui yaitu **vocabulary**. **vocabulary** adalah sekumpulan token unik di dalam corpus.

Lanjut, berikut adalah macam dari basic preprocessing

## 1.  Case Folding
Case Folding mengubah semua huruf kapital menjadi huruf kecil. Perhatikan kalimat berikut

```
Mr. Cook  went into the kitchen to cook dinner
```

Sebelum C.F. : **cook**, dinner, into, kitchen, Mr., the, to, went, **Cook**

Sesudah C.F. : **cook**, dinner, into, kitchen, **mr.**, the, to, went

Kelebihan: lebih efisien dari segi penyimpanan.

Kekurangan: Information loss atau banyak informasi yang hilang sehingga menjadi tidak akurat.

## 2. Stop Word Removal
Stop Word Removal menghapus kata-kata umum atau stopwords yang tidak memiliki  nilai penting dalam analisis seperti "the", "a", "is". Perhatikan kalimat berikut

"I saw **the** movie last night. I was **not** amused."

setelah dikenai stop word removal, kalimat tersebut akan berubah menjadi seperti ini

"I saw movie last night. I was amused."

Lihat, bahwa arti dari kalimat tersebut menjadi berbeda.

Kelebihan: Lebih efisien.

Kekurangan: Information loss.

## 3. Stemming
Mengubah kata-katanya menjadi bentuk dasar atau kata dasar dengan menghapus akhiran seperti "-ing" atau "-ed". Contoh:

{Banks, Bangking} -> Bank

Kelebihan:

1. Mengurangi ukuran vocabulary
2. Menggeneralisir model akan kata dasar yang sama bisa bersikap sama
3. Membantu mengolah kata yang mungkin ada diluar vocabulary

Kekurangan: 
1. Overstem
2. Understem
3. Menghasilkan hasil yang hurang bagus

## 4. Lemmatization
Mengubah kata-kata menjadi bentuk dasarnya atau lemma dengan memperhitungkan konteks dan menggunakan kamus atau aturan bahasa. Metode ini lebih canggih dibandingkan stemming. Contoh

{Did, Done, Doing} -> Do

Kelebihan:
Mirip seperti stemming tapi lebih akurat dan lebih dianjurkan

Kekurangan: cukup merugikan jika tenses diperhitungkan dan jika suatu kalimat itu ambigu.

## Hands On
https://colab.research.google.com/github/nitinpunjabi/nlp-demystified/blob/main/notebooks/nlpdemystified_preprocessing.ipynb

