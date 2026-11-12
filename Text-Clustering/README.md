# Text Clustering

Notebook praktik untuk materi Text Clustering, mata kuliah Text Analytics.

## Isi

`text_clustering.ipynb` mengikuti urutan slide dan modul:

1. Data: AG News (sampel 2.000 berita, 4 topik)
2. Ukuran kemiripan dan jarak: cosine, Jaccard, Euclidean
3. Representasi sparse: TF-IDF
4. Reduksi dimensi: Truncated SVD (LSA), t-SNE untuk visualisasi
5. K-Means, metode elbow, dan analisis silhouette
6. Hierarchical clustering dan dendrogram
7. DBSCAN dan HDBSCAN
8. Evaluasi internal dan eksternal, contoh metrik yang menyesatkan, kestabilan
9. Interpretasi cluster dengan c-TF-IDF dan dokumen representatif
10. Data berbahasa Indonesia (SmSA, IndoNLU)

Pipeline berbasis sentence embeddings tidak dicakup.

## Cara menjalankan

```bash
pip install -r requirements.txt
jupyter notebook text_clustering.ipynb
```

Notebook juga dapat dibuka langsung di Google Colab. HDBSCAN memerlukan scikit-learn versi 1.3 atau lebih baru.

## Data

Data diunduh otomatis saat notebook dijalankan dan disimpan di folder `data/` (tidak ikut disimpan di repositori):

- AG News (berkas uji): https://github.com/mhjabreel/CharCnn_Keras
- SmSA: https://github.com/IndoNLP/indonlu

Keluaran yang tersimpan di notebook dihasilkan dengan scikit-learn 1.9.1. Angka dapat sedikit berbeda pada versi lain.
