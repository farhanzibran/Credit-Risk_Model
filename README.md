# Credit-Risk_Model
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

