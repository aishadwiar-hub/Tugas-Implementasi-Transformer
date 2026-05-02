# Pemahaman dan Implementasi Transformer untuk Text dan Vision

**Penulis:** Aisha Dwi Anindita Radianto (256150100111003)  
**Institusi:** Program Magister Ilmu Komputer, Fakultas Ilmu Komputer (FILKOM), Universitas Brawijaya

## 📌 Deskripsi Proyek

1. **Text Classification (Transformer vs LSTM)**
   - **Dataset:** AG News (4 Kelas).
   - **Tugas:** Membangun *Text Transformer* dengan modul *Embedding, Positional Encoding*, dan *Self-Attention*, lalu membandingkannya dengan Bidirectional LSTM.
   - **Hasil:** Transformer mengungguli LSTM baik dari segi akurasi (88.72%) maupun kecepatan komputasi berkat mekanisme paralelisasi *attention*.

2. **Image Classification (Vision Transformer vs Simple CNN)**
   - **Dataset:** CIFAR-10 (Resolusi 32x32).
   - **Tugas:** Membangun *Vision Transformer* (ViT) dengan mekanisme *Patch Splitting* (4x4 dan 8x8), lalu membandingkannya dengan CNN sederhana.
   - **Hasil:** CNN (74.19%) mengungguli ViT (56.85%) pada dataset beresolusi kecil karena CNN memiliki *inductive bias* (lokalitas dan invariansi translasi) yang tidak dimiliki oleh ViT tanpa tahap *pre-training* skala masif.

3. **Object Detection (Eksplorasi GitHub Non-Klasifikasi)**
   - **Model:** YOLOv8 Nano dari Ultralytics.
   - **Tugas:** Eksplorasi arsitektur produksi untuk lokalisasi dan deteksi objek.
   - **Modifikasi:** Mengubah *Confidence Threshold* inferensi dari `0.25` (bawaan) menjadi `0.85` untuk mengeliminasi prediksi dengan tingkat keyakinan rendah.

Link Drive (Laporan): https://drive.google.com/drive/folders/1mq-mcwmWFHtUbQsSdRstZAPIwOetjhpU?usp=sharing
