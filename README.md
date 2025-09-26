# Akbank Derin Öğrenme Bootcamp Projesi: Görüntü Sınıflandırma
### Intel Image Classification Veri Seti Üzerine CNN Mimarisi Uygulaması

Bu proje, Akbank Derin Öğrenme Bootcamp'i kapsamında derin öğrenme pratiklerini ve model geliştirme tekniklerini uygulamak amacıyla oluşturulmuştur. [cite_start]Proje, bir **Convolutional Neural Network (CNN)** mimarisi kullanarak görsel bir sınıflandırma problemini çözmeyi hedeflemektedir[cite: 2].

## 📌 Projenin Amacı

[cite_start]Bu çalışmanın ana amacı, **Intel Image Classification** veri setini kullanarak 6 farklı coğrafi ortamı (Binalar, Orman, Buzul, Dağ, Deniz, Sokak) yüksek doğrulukla sınıflandıran bir model oluşturmaktır[cite: 73]. [cite_start]Proje süreci, veri analizi, model eğitimi, performans değerlendirme ve yorumlama gibi derin öğrenmenin temel adımlarını içermektedir[cite: 3].

## 📂 Veri Seti Hakkında

Projede kullanılan veri seti Kaggle'dan temin edilmiştir. [cite_start]Veri seti, 6 farklı sınıfa ait yaklaşık **25,000 eğitim** ve **14,000 test** görüntüsü içermektedir[cite: 74].

**Veri Ön İşleme Adımları:**
* Görüntüler **150x150 piksel** boyutuna yeniden ölçeklendirilmiştir.
* [cite_start]Modelin genelleme yeteneğini artırmak için **Veri Çoğaltma (Data Augmentation)** teknikleri (Rotasyon, Yatayda Çevirme vb.) uygulanmıştır[cite: 21].

## 🛠 Kullanılan Yöntemler ve Model Mimarisi

* **Framework:** PyTorch
* **Optimizasyon:** Hiperparametre optimizasyonu sonucunda **Adam** optimizasyon algoritması ve optimize edilmiş **0.0001 Öğrenme Oranı (Learning Rate)** kullanılmıştır.
* **Model Mimarisi:** Proje yönergelerine uygun olarak, modelin karmaşık desenleri öğrenmesi için derin bir CNN mimarisi tasarlanmıştır. Modelin temel bileşenleri:
    * [cite_start]**Evrişimsel Katmanlar (Convolutional Layers)** [cite: 30]
    * [cite_start]**Havuzlama Katmanları (Pooling Layers)** [cite: 31]
    * [cite_start]**Dropout Katmanları** (0.5 ve 0.3 oranlarında) [cite: 32, 46]
    * [cite_start]**Tam Bağlantılı Katmanlar (Dense Layers)** [cite: 33]

## 📈 Elde Edilen Sonuçlar ve Değerlendirme

Modelin performansı, çeşitli metrikler ve görselleştirmelerle detaylı bir şekilde değerlendirilmiştir.

* **En İyi Doğrulama Doğruluğu:** %85.36
* [cite_start]**Değerlendirme Raporları:** Accuracy ve Loss grafikleri, Confusion Matrix ve Classification Report kullanılmıştır[cite: 37, 38].
* [cite_start]**Model Yorumlama:** Modelin hangi bölgelere odaklandığını göstermek için **Grad-CAM** görselleştirmeleri uygulanmıştır[cite: 39, 40].

### Önemli Not: Overfitting/Underfitting

[cite_start]Eğitim ve doğrulama grafikleri dikkatle incelenmiş, modelin **aşırı uyum (overfitting)** yapmaması için gerekli önlemler alınmıştır[cite: 53, 54].

---

### 🌐 Proje Bağlantısı

Bu projenin tüm teknik detaylarına, kodlarına ve çıktılara aşağıdaki Kaggle not defterinden ulaşabilirsiniz.

[Kaggle Notebook Linkiniz BURAYA Gelecek]
