# TensorFlow ile El Yazısı Rakam Tanıma (MNIST)

Bu proje, TensorFlow ve Keras kullanarak el yazısı rakamları tanıyan basit bir yapay sinir ağı modeli geliştirmek için yapılmıştır. MNIST veri seti üzerinden model eğitilip test edilmiştir.

## Projenin Amacı
Yapay zeka ve derin öğrenmeye giriş yapmak, TensorFlow kullanarak temel bir sinir ağı oluşturup eğitmek ve modelin doğruluğunu test etmek.

## Kullanılan Teknolojiler
- Python  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  

## Model Mimarisi
- Girdi: 28x28 piksellik el yazısı rakam görüntüleri (flatten edilmiş)  
- Gizli Katman: 128 nöron, ReLU aktivasyon  
- Çıkış Katmanı: 10 nöron, Softmax aktivasyon (0-9 rakamları için)

## Veri Hazırlama
- Görüntü değerleri 0-1 aralığına normalize edildi  
- Etiketler one-hot encoding formatına dönüştürüldü

## Eğitim Detayları
- Eğitim verisi: 60.000 örnek  
- Test verisi: 10.000 örnek  
- Epoch sayısı: 5  
- Modelin test doğruluğu yaklaşık %97

## Sonuçlar ve Görselleştirme
Model, test verisi üzerindeki rakamları yüksek doğrulukla tahmin etmektedir. matplotlib ile tahmin edilen rakamlar ve gerçek rakamlar görselleştirilmiştir.

## Kişisel Deneyim
Bu projeyi yaparak TensorFlow ile basit bir sinir ağı kurmayı ve eğitmeyi öğrendim. Görsel verilerle çalışma deneyimi kazandım ve derin öğrenmeye giriş yapmış oldum. Bu temelin üzerine daha karmaşık yapay zeka modelleri geliştirmeyi planlıyorum.

## Proje Dosyaları
- `mnist_model.py` — Modelin eğitim ve test kodları  
- `visualization.py` — Tahminlerin görselleştirilmesi için kullanılan kodlar  

## Nasıl Çalıştırılır?
1. Python ve gerekli kütüphaneler (TensorFlow, NumPy, Matplotlib) yüklü olmalı.  
2. `mnist_model.py` dosyasını çalıştırarak modeli eğitebilirsiniz.  
3. Eğitim tamamlandıktan sonra `visualization.py` ile tahminleri görselleştirebilirsiniz.


