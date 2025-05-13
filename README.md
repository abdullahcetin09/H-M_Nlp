# H-M_Nlp
# H&M Hurdaya Çıkarılan Ürünler: Malzeme Açıklamaları Analizi ve Kümeleme

Bu proje, Kaggle'daki H&M Hurdaya Çıkarılan Ürünler veri setini kullanarak ürün malzeme açıklamaları üzerine odaklanan bir veri bilimi çalışmasıdır. NLP ve makine öğrenmesi teknikleriyle hurdaya çıkarılan ürünlerdeki malzeme kombinasyonlarını anlamak, benzer malzemelere sahip ürünleri gruplamak ve desenleri keşfetmek hedeflenmiştir.

## Proje Amacı

* Malzeme açıklamalarını analiz etmek.

* Metin işleme ile malzeme tanımlarını temizlemek.

* Benzer malzeme açıklamalarını kümelemek.

* Malzeme desenlerini keşfetmek.

* Bulguları görselleştirmek.

## Veri Seti

Çalışma, Kaggle H&M Hurdaya Çıkarılan Ürünler veri setinin `materials` sütununu kullanır.

## Metodoloji

Proje adımları:

1. **Veri Yükleme:** Veri setini yükleme ve temel yapısını anlama.

2. **Keşifçi Veri Analizi (EDA):** Eksik değerleri, dağılımları ve trendleri görselleştirme.

3. **Veri Temizleme:** Malzeme metinlerini ön işleme (küçük harf, noktalama, sayılar, stop-words).

4. **Özellik Mühendisliği:** Metinleri TF-IDF ile sayısal vektörlere dönüştürme ve kelime sıklıklarını görselleştirme.

5. **Modelleme ve Analiz:** KMeans ile kümeleme, Kosinüs benzerliği ile benzerlik arama, PCA ile boyut indirgeme ve görselleştirme.

6. **Yorumlama:** Analiz sonuçlarından çıkarımlar yapma.

## Ana Bulgular (Örnek)

* Veri setinin eksik değer durumu belirlendi.

* En sık hurdaya çıkan ürün tipleri ve renkler tespit edildi (varsa).

* Malzeme açıklamalarında yaygın kelimeler (cotton, polyester vb.) görüldü.

* KMeans ile benzer malzemeler gruplandı (doğal lifler, sentetik karışımlar vb.).

* PCA görselleştirmesi kümelerin ayrışmasını gösterdi.

* Kurulum ve Çalıştırma

Projeyi çalıştırmak için:

1. Depoyu klonlayın: `git clone <depo_adresiniz>`

2. Gerekli kütüphaneleri yükleyin: `pip install -r requirements.txt`

3. NLTK verilerini indirin: `python -m nltk.downloader punkt stopwords` (Spacy/Gensim için ek indirmeler gerekebilir)

4. Kaggle'dan veri setini indirin ve dosya yolunu güncelleyin.

5. `H&M.ipynb` dosyasını çalıştırın.
