# Credit-Risk_Model   
## (Link dataset :https://www.kaggle.com/datasets/husainsb/lendingclub-issued-loans )
## Introduction
Credit Risk Model adalah sebuah model untuk memprediksi pinjaman mana yang akan mengalami gagal bayar.

## Pengenalan Dataset, Target variable, dan Missing Value
1. pengenalan Dataset
*  Data terdiri dari 759338 rows dan 75 kolom
  
2. Target variabel
*  Dikarenakan project ini untuk mengetahui bad loan & good loan, maka perlu dibuat feature baru, yaitu target variable yang merepresentasikan bad loan (sebagai 1) dan good loan (sebagai 0). 
*  Jika loan_statusnya 'Charged Off', 'Default', 'Late (31-120 days)', 'Late (16-30 days)' akan dianggap sebagai bad_loan atau 1 dan nilai selain itu akan dianggap good loan atau 0
  
3. Missing Values
   Banyak terdapat missing value, sehingga metode yang digunakan adalah dengan menghapus kolom yang memiliki missing value diatas 50%

 ## Data Splitting
 1. Training dataset untuk melatih model
 2. Testing dataset untuk menguji seberapa baik kinerja model yang sudah dilatih atau evaluasi

 ## Feature Engineering
 1. memilih fitur yang relevan untuk dijadikan objek variabel prediktor dan target
 2. melakukan transformasi dari datetime ke numerik

## Modelling 1
1. menggunakan Logistic regression dengan nilai score accuracy 0.9167961650907367 serta nilai confution matrix dengan nilai di gambar berikut ![image](https://github.com/user-attachments/assets/1d7da55d-b85f-43aa-828b-fb7b749a96f6)

## Modelling 2 
1. Threshold
   Nilai batas yang digunakan untuk menentukan kelas dalam model klasifikasi. Misalnya, dalam model klasifikasi biner, jika probabilitas prediksi lebih besar dari threshold (misalnya 0.5), maka model memprediksi kelas positif; jika tidak, kelas negatif.
2. Confusion Matrix
   Matriks yang digunakan untuk mengevaluasi kinerja model klasifikasi dengan membandingkan prediksi dan label sebenarnya. Komponen: True Positive (TP), True Negative (TN), False Positive (FP), dan False Negative (FN).
3. ROC AUC (Receiver Operating Characteristic - Area Under Curve)
   ROC adalah grafik yang menunjukkan hubungan antara True Positive Rate (TPR/Recall) dan False Positive Rate (FPR). AUC adalah area di bawah kurva ROC.
Kegunaan: Mengukur kemampuan model untuk membedakan antara kelas-kelas. Nilai AUC mendekati 1 menunjukkan model yang baik, sedangkan nilai mendekati 0.5 menunjukkan model yang buruk.
4. Model Interpretation
  Proses memahami bagaimana model membuat keputusan atau prediksi.
Contoh: Menggunakan teknik seperti SHAP, LIME, atau visualisasi untuk mengetahui fitur mana yang paling berpengaruh terhadap prediksi model.
Kegunaan: Penting untuk kepercayaan, transparansi, dan validasi model, terutama dalam aplikasi sensitif seperti kesehatan atau keuangan.

## Evaluasi 
* True Positive (TP): 9323 — Jumlah kasus kelas 1 yang diprediksi dengan benar.
* True Negative (TN): 116323 — Jumlah kasus kelas 0 yang diprediksi dengan benar.
* False Positive (FP): 24252 — Kasus kelas 0 yang salah diprediksi sebagai kelas 1.
* False Negative (FN): 1970 — Kasus kelas 1 yang salah diprediksi sebagai kelas 0.

## Ringkasan:
* Akurasi: 82.7%
* Presisi: 27.8%
* Recall: 82.5%
* Specificity: 82.7%
* F1-Score: 41.6%






