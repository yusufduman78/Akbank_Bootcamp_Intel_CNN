# Akbank Derin Öğrenme Bootcamp Projesi: Görüntü Sınıflandırma
### Intel Image Classification Veri Seti Üzerine CNN Mimarisi Uygulaması

Bu proje, Akbank Derin Öğrenme Bootcamp'i kapsamında derin öğrenme pratiklerini ve model geliştirme tekniklerini uygulamak amacıyla oluşturulmuştur. Proje, bir **Convolutional Neural Network (CNN)** mimarisi kullanarak görsel bir sınıflandırma problemini çözmeyi hedeflemektedir.

## 📌 Projenin Amacı

Bu çalışmanın ana amacı, **Intel Image Classification** veri setini kullanarak 6 farklı coğrafi ortamı (Binalar, Orman, Buzul, Dağ, Deniz, Sokak) yüksek doğrulukla sınıflandıran bir model oluşturmaktır. Proje süreci, veri analizi, model eğitimi, performans değerlendirme ve yorumlama gibi derin öğrenmenin temel adımlarını içermektedir.

## 📂 Veri Seti Hakkında

Projede kullanılan veri seti Kaggle'dan temin edilmiştir. Veri seti, 6 farklı sınıfa ait yaklaşık **25,000 eğitim** ve **14,000 test** görüntüsü içermektedir.

**Veri Ön İşleme Adımları:**
* Görüntüler **150x150 piksel** boyutuna yeniden ölçeklendirilmiştir.
* Modelin genelleme yeteneğini artırmak için **Veri Çoğaltma (Data Augmentation)** teknikleri (Rotasyon, Yatayda Çevirme vb.) uygulanmıştır.

## 🛠 Kullanılan Yöntemler ve Model Mimarisi

* **Framework:** PyTorch
* **Optimizasyon:** Hiperparametre optimizasyonu sonucunda **Adam** optimizasyon algoritması ve optimize edilmiş **0.0001 Öğrenme Oranı (Learning Rate)** kullanılmıştır.
* **Model Mimarisi:** Proje yönergelerine uygun olarak, modelin karmaşık desenleri öğrenmesi için derin bir CNN mimarisi tasarlanmıştır. Modelin temel bileşenleri:
    * **Evrişimsel Katmanlar (Convolutional Layers)** 
    * **Havuzlama Katmanları (Pooling Layers)** 
    * **Dropout Katmanları** (0.5 ve 0.3 oranlarında) 
    * **Tam Bağlantılı Katmanlar (Dense Layers)** 

## 📈 Elde Edilen Sonuçlar ve Değerlendirme

Modelin performansı, çeşitli metrikler ve görselleştirmelerle detaylı bir şekilde değerlendirilmiştir.

* **En İyi Doğrulama Doğruluğu:** %85.36
* **Değerlendirme Raporları:** Accuracy ve Loss grafikleri, Confusion Matrix ve Classification Report kullanılmıştır.
* **Model Yorumlama:** Modelin hangi bölgelere odaklandığını göstermek için **Grad-CAM** görselleştirmeleri uygulanmıştır.

### Önemli Not: Overfitting/Underfitting

Eğitim ve doğrulama grafikleri dikkatle incelenmiş, modelin **aşırı uyum (overfitting)** yapmaması için gerekli önlemler alınmıştır.

---

### 🌐 Proje Bağlantısı

Bu projenin tüm teknik detaylarına, kodlarına ve çıktılara aşağıdaki Kaggle not defterinden ulaşabilirsiniz.

[https://www.kaggle.com/code/smoke78/cnn-working]

Bu projenin tüm teknik detaylarına, kodlarına ve çıktılara aşağıdaki Kaggle not defterinden ulaşabilirsiniz.

[Kaggle Notebook Linkiniz BURAYA Gelecek]
