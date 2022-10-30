## Dataset

Dataset yang digunakan berasal dari Google Cloud Platform dengan link [berikut](https://console.cloud.google.com/bigquery?p=bigquery-public-data&d=ml_datasets&t=census_adult_income&page=table). Menggunakan dataset `ml_datasets` dari database bernama `census_adult_income`.


## Objectives

Membuat model Classification menggunakan Logistic Regression dan SVM untuk memprediksi `income bracket` menggunakan dataset yang sudah ada.


## Kesimpulan

Saya membuat 2 model menggunakan Logistic Regression dan SVC. Logistic Regression dengan waktu training lebih sedikit memiliki nilai yang cukup baik namun masih kalah dengan SVC dalam precission, recall, dan accuracy. SVC memiliki accuracy lebih tinggi yaitu 0.84 dimana Logistic Regression hanya 0.83. Pada label dengan jumlah lebih sedikit yaitu >50K, SVC memiliki precission yang lebih tinggi yaitu 0.76 untuk Train dan Test sedangkan Logistic hanya 0.71 pada Train dan 0.72 pada Test. Pada hal yang kita fokuskan yaitu recall, SVC memiliki nilai 0.94 pada Train dan Test sedangkan Logistic hanya 0.92 di Train dan 0.93 pada Test. Pada Inference Set, kedua model menghasilkan accuracy, recall, dan precission yang sama persis mungkin dikarenakan jumlah Inference yang hanya 10 data.

Jadi dari kedua model yang dibuat, model yang memiliki performa lebih baik adalah **SVC** karena memiliki nilai recall pada label <=50K lebih tinggi dari pada Logistic Regression.


