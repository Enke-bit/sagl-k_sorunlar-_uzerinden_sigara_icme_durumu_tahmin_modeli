## Sigara içme durmu üzerinden sağlık probleri öğrenme ve bunuda tam tersine tahmin işlemi yapan mode.

# Kullanılan kütüpaneler

pip install pandas
pip install matplotlib
pip install scikit-learn
pip install tensorflow  # Keras, TensorFlow'un bir parçası olarak gelir

# Veri seti kaynak yeri

https://www.kaggle.com/datasets/jaceprater/smokers-health-data

## Model Özellikleri
Model Tipi: Sequential
Toplam Katman Sayısı: 3 (Giriş, Ara ve Çıkış katmanları)
Katmanlar ve Aktivasyon Fonksiyonları
Giriş Katmanı:

# Katman Türü: Dense (Tam Bağlantılı Katman)
Nöron Sayısı: 1000
Girdi Boyutu: input_dim=X_train.shape[1] (Girdi verisinin özellik sayısı)
Aktivasyon Fonksiyonu: ReLU (Rectified Linear Unit)
Ara Katman:

# Katman Türü: Dense (Tam Bağlantılı Katman)
Nöron Sayısı: 500
Aktivasyon Fonksiyonu: ReLU
Çıkış Katmanı:

# Katman Türü: Dense (Tam Bağlantılı Katman)
Nöron Sayısı: y.shape[1] (Çıkış sınıf sayısı)
Aktivasyon Fonksiyonu: Softmax
Derleme (Compile) Özellikleri
Optimizasyon Algoritması: Adam
Kayıp Fonksiyonu: Categorical Crossentropy
Değerlendirme Metrikleri: Accuracy (Doğruluk)
Model Özet Tablosu
Aşağıdaki kodu çalıştırarak model özet tablosunu görebilirsiniz:

model.summary()

Bu kod bloğu modelin özetini verecek ve katmanların detaylarını (katman türleri, çıkış şekilleri, parametre sayıları) listeleyecektir. Örneğin:


# Modelin eğitimi sonrasında elde edilen değerler şunlardır:

loss: 0.3123 - accuracy: 0.8923

# Katkıda Bulunma
Katkıda bulunmak isterseniz, lütfen bir issue açın veya bir pull request gönderin. Her türlü geri bildirim ve katkı değerlidir.

