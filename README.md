# WhatsApp Kullanıcı Yorumları Üzerine Duygu Analizi (NLP Projesi)

Bu proje, WhatsApp uygulamasına ait Google Play Store kullanıcı yorumları üzerinde metin madenciliği ve duygu analizi gerçekleştirmektedir. Yorum metinleri temizlenmiş, TF-IDF yöntemiyle sayısal forma dönüştürülmüş ve Naive Bayes algoritması ile sınıflandırma yapılmıştır.

## Proje Hedefi

Kullanıcı yorumlarını pozitif ve negatif olarak sınıflandırmak ve bu sayede WhatsApp uygulaması hakkında kullanıcı memnuniyetine dair içgörüler sunmak.

## Kullanılan Veri Seti

- Kaynak: [Kaggle - WhatsApp Messenger Reviews Dataset](https://www.kaggle.com/datasets/ravibits/whatsapp-app-reviews-from-google-play-store)
- Boyut: ~94.000 yorum
- Sütunlar: App, Review, Translated_Review, Sentiment, Rating, Review Date

## Kullanılan Teknolojiler

- Python
- Pandas
- Scikit-learn
- Seaborn
- Matplotlib
- WordCloud

## Metin Ön İşleme

- Küçük harfe çevirme
- Noktalama temizliği
- Stopword (gereksiz kelimeler) temizliği
- Gereksiz karakterlerin kaldırılması

## Özellik Çıkarımı

- TF-IDF vektörleştirme (maksimum 5000 kelime)

## Sınıflandırma

- Algoritma: Multinomial Naive Bayes
- Eğitim/Test ayrımı: %80 - %20
- Değerlendirme Metrikleri:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

## Görseller

### Kullanıcı Puan Dağılımı
![kullanici-puan-dagilimi](https://github.com/user-attachments/assets/6e95120e-a202-4600-82e9-44d904e984e2)


### Yorum Duygu Dağılımı
![yorum-duygu-dagilimi](https://github.com/user-attachments/assets/f8607f1d-1995-4f5b-a350-013c6589e6d2)


### Confusion Matrix (Binary)
![confusion-matix](https://github.com/user-attachments/assets/7a3d6ab9-7843-447f-83d1-f7af6abc7d26)


### Kelime Bulutu
![kelime-bulutu](https://github.com/user-attachments/assets/641c51b2-2152-45ee-8c8b-56f4faee0738)


### Yorum Uzunluğu Dağılımı
![yorum-uzunlugu-dagilimi](https://github.com/user-attachments/assets/89230e36-4339-4b4a-8240-f0096f44e05a)


## Sonuçlar

- Naive Bayes modeli ile yapılan sınıflandırma yüksek doğruluk oranı göstermiştir.
- Confusion Matrix, modelin pozitif ve negatif sınıfları ayırt etmede başarılı olduğunu göstermektedir.
- WordCloud görselleştirmesi ile yorumlarda en sık geçen kelimeler belirlenmiştir.

## İşletme Açısından Yorum

Bu analiz, WhatsApp gibi mobil uygulamalar için kullanıcı geri bildirimlerinden faydalanarak müşteri memnuniyetini değerlendirme fırsatı sunmaktadır. Özellikle negatif yorumlarda sık tekrarlanan sorunlar tespit edilerek ürün iyileştirme ve kullanıcı deneyimi geliştirme süreçleri desteklenebilir. Ayrıca pazarlama stratejilerinde kullanılabilecek önemli kullanıcı içgörüleri sağlanabilir.

## Lisans

Bu proje yalnızca eğitim amacıyla hazırlanmıştır. Kullanılan veri seti [Kaggle](https://www.kaggle.com/datasets/ravibits/whatsapp-app-reviews-from-google-play-store) platformundan edinilmiştir.
