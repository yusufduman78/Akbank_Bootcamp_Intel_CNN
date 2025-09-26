# Akbank_Bootcamp_Intel_CNN

# Akbank Derin Öğrenme Bootcamp Projesi: Intel Görüntü Sınıflandırma

## Projenin Amacı
Bu proje, Intel Image Classification veri setini kullanarak 6 farklı coğrafi ortamı (Binalar, Orman, Buzul, Dağ, Deniz, Sokak) yüksek doğrulukla sınıflandıran derin bir Evrişimsel Sinir Ağı (CNN) modeli geliştirmeyi amaçlamaktadır. Proje, derin öğrenme pratiklerini, veri çoğaltmayı ve model yorumlama tekniklerini kapsamaktadır.

## Veri Seti Hakkında Bilgi
* **Veri Seti Adı:** Intel Image Classification
* **Sınıf Sayısı:** 6 (Multiclass Classification)
* **Boyut:** Yaklaşık 14.000 eğitim ve 3000 test görüntüsü.
* **Ön İşleme:** Görüntüler 150x150 boyutuna yeniden boyutlandırılmış ve eğitim seti için **Rotation** ve **Horizontal Flip** içeren **Veri Çoğaltma (Data Augmentation)** uygulanmıştır.

## Kullanılan Yöntemler
1.  **Framework:** PyTorch
2.  **Model Mimarisi:** Derin bir CNN yapısı kullanılmıştır. Model, 4 Evrişimsel Katman, 3 Havuzlama Katmanı, Dropout (0.5 ve 0.3 oranlarında) ve 3 Tam Bağlantılı Katman içermektedir.
3.  **Optimizasyon:** Hiperparametre optimizasyonu sonucunda **Adam** optimizasyon algoritması ve optimize edilmiş **$0.0001$ Öğrenme Oranı (Learning Rate)** kullanılmıştır.
4.  **Değerlendirme:** Accuracy, Loss grafikleri, Confusion Matrix ve modelin karar verme bölgelerini gösteren **Grad-CAM** görselleştirmesi ile değerlendirilmiştir.

## Elde Edilen Sonuçlar Özeti
* **En İyi Doğrulama Doğruluğu:** %85.36
* **Optimizasyon Kazanımı:** Öğrenme oranının $0.001$'den $0.0001$'e düşürülmesi, doğruluğu **%4.49** oranında artırmıştır.

---

### Kaggle Notebook Linki
[BURAYA KAGGLE NOTEBOOK'UNUZUN FİNAL LİNKİNİ EKLEYİN]
