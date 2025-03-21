<<<<<<< HEAD
# Insect-Detection-Using-CNN
=======
Deskripsi
Proyek ini adalah model klasifikasi gambar menggunakan TensorFlow dan Keras. Model telah dikonversi ke tiga format: SavedModel, TFJS, dan TF-Lite agar bisa digunakan di berbagai platform.

📂 Struktur Folder
submission
├───tfjs_model
|   ├───group1-shard1of1.bin
|   └───model.json
├───tflite
|   ├───model.tflite
|   └───label.txt
├───saved_model
|   ├───saved_model.pb
|   └───variables
├───notebook.ipynb
├───README.md
└───requirements.txt

🛠Instalasi
1.Clone Repository (jika ada)
git clone <repository-url>
cd submission

2.Install Dependencies
pip install -r requirements.txt

Cara Menjalankan

1.Menjalankan Notebook
Buka notebook.ipynb di Jupyter Notebook atau Google Colab, lalu jalankan sel satu per satu.

2.Menggunakan Model TF-Lite
Untuk inference menggunakan model TensorFlow Lite, gunakan kode berikut:

import tensorflow.lite as tflite

interpreter = tflite.Interpreter(model_path="tflite/model.tflite")
interpreter.allocate_tensors()

3.Menggunakan Model TFJS
Model TFJS bisa digunakan di browser dengan TensorFlow.js. Copy file di tfjs_model/ ke server dan load model dengan:

const model = await tf.loadLayersModel('tfjs_model/model.json');
>>>>>>> 8e66703 (First commit - add initial project files)
