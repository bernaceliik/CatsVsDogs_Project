# CatsVsDogs_Project
# Cats vs Dogs Classification with CNN and Grad-CAM

## Projenin Amacı
Bu proje, kedi ve köpek resimlerini sınıflandırmak amacıyla Convolutional Neural Network (CNN) kullanmaktadır. 
Ayrıca Grad-CAM yöntemi ile modelin hangi bölgeleri dikkate alarak tahmin yaptığını görselleştiriyoruz.

## Veri Seti Hakkında
- Kullanılan veri seti: [Dogs vs Cats Redux](https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition) (Kaggle)
- Toplam resim sayısı: 25,000 (12,500 kedi, 12,500 köpek)
- Resimler eğitim ve doğrulama seti olarak ayrılmıştır.
- Veri seti Kaggle üzerinde mevcut olduğundan repoya eklenmesine gerek yoktur.

## Kullanılan Yöntemler
1. **CNN Modeli**:
   - 4 adet Conv2D + BatchNormalization + MaxPooling katmanı
   - Flatten → Dense → Dropout → Sigmoid çıktı
2. **Data Augmentation** ile eğitim verisinin artırılması
3. **EarlyStopping** ve **ReduceLROnPlateau** callback’leri
4. **Grad-CAM** ile modelin dikkat ettiği bölgelerin görselleştirilmesi

## Elde Edilen Sonuçlar
- Eğitim ve doğrulama accuracy grafikleri, loss grafikleri görselleştirildi.
- Confusion matrix ve classification report ile modelin performansı değerlendirildi.
- Örnek Grad-CAM görselleri ile modelin hangi bölgelere odaklandığı gözlemlendi.
- Model doğruluk oranı: ~%85 (Geliştirilmiş CNN + BatchNormalization ve daha fazla epoch ile)

## Kaggle Notebook
Projeyi Kaggle üzerinde çalıştırmak için notebook linki: [Cats vs Dogs CNN + Grad-CAM](https://www.kaggle.com/code/bernaelik/notebook00b9e2bc46/notebook)
