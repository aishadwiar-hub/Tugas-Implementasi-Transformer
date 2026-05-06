# Pemahaman dan Implementasi Transformer untuk Text dan Vision

**Penulis:** Aisha Dwi Anindita Radianto (256150100111003)  
**Institusi:** Program Magister Ilmu Komputer, Fakultas Ilmu Komputer (FILKOM), Universitas Brawijaya

## 📌 Deskripsi Proyek

1. **Text Classification (Transformer vs LSTM vs TextCNN)**
   - **Dataset:** AG News (4 Kelas).
   - **Tugas:** Membangun *Text Transformer* dari awal (*from scratch*) dengan modul *Embedding*, *Positional Encoding*, dan *Self-Attention*, lalu membandingkan performanya dengan arsitektur sekuensial konvensional (Bidirectional LSTM) dan jaringan konvolusi 1D (TextCNN).
   - **Hasil:** Transformer mengungguli model lainnya dari segi akurasi akhir (88.41%) berkat mekanisme atensi global. Namun, TextCNN (87.58%) terbukti menjadi arsitektur komputasi yang paling efisien dan dieksekusi paling cepat. LSTM (85.75%) justru memakan waktu terlama akibat proses komputasi yang berjalan sekuensial.

2. **Image Classification (Vision Transformer vs Simple CNN vs ResNet)**
   - **Dataset:** CIFAR-10 (Resolusi 32x32 piksel, RGB).
   - **Tugas:** Membangun *Vision Transformer* (ViT) dengan mekanisme *Patch Splitting* (eksperimen 4x4 dan 8x8), lalu membandingkannya dengan dua arsitektur *baseline* berbasis konvolusi: Simple CNN dan ResNet.
   - **Hasil:** Jaringan konvolusi Simple CNN (74.47%) dan ResNet (72.30%) menang telak atas ViT (55.45%). Ketiadaan *inductive bias* spasial pada ViT menyebabkannya mengalami *underfitting* parah di dataset berskala kecil. Sebaliknya, ResNet mendemonstrasikan stabilitas dan efisiensi memori yang sangat luar biasa meskipun hanya berbekal ~78 ribu parameter.

3. **Object Detection (Eksplorasi GitHub Non-Klasifikasi)**
   - **Model:** YOLOv8 Nano dari Ultralytics.
   - **Tugas:** Eksplorasi arsitektur produksi untuk lokalisasi dan deteksi objek.
   - **Modifikasi:** Mengubah *Confidence Threshold* inferensi dari `0.25` (bawaan) menjadi `0.85` untuk mengeliminasi prediksi dengan tingkat keyakinan rendah.

Link Drive (Laporan): https://drive.google.com/drive/folders/1mq-mcwmWFHtUbQsSdRstZAPIwOetjhpU?usp=sharing
