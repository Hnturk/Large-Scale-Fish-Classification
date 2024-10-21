# Büyük Ölçekli Balık Sınıflandırma - Yapay Sinir Ağı (ANN)

Bu proje, 9 farklı balık türüne ait görüntülerden oluşan bir veri seti kullanarak balık türlerini sınıflandırmayı amaçlamaktadır. Projede, bir Yapay Sinir Ağı (ANN) modeli oluşturulmuş ve TensorFlow kullanılarak eğitilmiştir.

## Veri Seti

Veri seti, her bir balık türü için 1000 adet artırılmış görüntü içermektedir. Balık türleri şunlardır:
- Çipura (Gilt Head Bream)
- Mercan (Red Sea Bream)
- Levrek (Sea Bass)
- Barbun (Red Mullet)
- İstavrit (Horse Mackerel)
- Karadeniz Hamsisi (Black Sea Sprat)
- Tekir (Striped Red Mullet)
- Alabalık (Trout)
- Karides (Shrimp)

## Veri İşleme

- **Kütüphaneler**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `OpenCV`, `TensorFlow` gibi kütüphaneler veri işleme ve görselleştirme için kullanılmıştır.
- **Görüntülerin Okunması**: Görüntüler, dosya yollarından okunarak işlenmiştir.
- **Etiket Dönüştürme**: Sınıf etiketleri, modelin işleyebilmesi için **One-Hot Encoding** yöntemi ile dönüştürülmüştür.

## Model

- **Yapay Sinir Ağı (ANN)**: Model, birden fazla gizli katman ve dropout katmanları içeren bir **Sequential** modeldir.
- **Aktivasyon Fonksiyonları**: Gizli katmanlarda `ReLU`, çıktı katmanında `softmax` kullanılmıştır.
- **Optimizasyon**: Model, `Adam` optimizasyon algoritması ile eğitilmiştir.

## Sonuçlar

Eğitim ve test sürecinde modelin doğruluk ve kayıp değerleri izlenmiş, ve güncel olarak şu sonuçlara ulaşılmıştır.
- Test Kaybı: 0.27224
- Test Doğruluğu: 91.67%

Kaggle Notebook Linki: https://www.kaggle.com/code/mehmethantrk/large-scale-fish-classification-ann
