# Veri Analizi Raporu

## Genel Bakış

Bu depo, bir veri kümesi üzerinde gerçekleştirilen keşifsel veri analizi (EDA) çalışmasını içermektedir. Analiz, verilerden içgörüler çıkarmayı, desenleri belirlemeyi ve uygulanabilir sonuçlar elde etmeyi amaçlamaktadır.

## Veri Kümesi

Bu veri kümesi aşağıdaki özelliklerden oluşmaktadır:

- **product_id** - Ürün Kimliği
- **product_name** - Ürünün Adı
- **category** - Ürünün Kategorisi
- **discounted_price** - Ürünün İndirimli Fiyatı
- **actual_price** - Ürünün Gerçek Fiyatı
- **discount_percentage** - Ürünün İndirim Yüzdesi
- **rating** - Ürünün Puanı
- **rating_count** - Amazon'da oylayan kişi sayısı
- **about_product** - Ürünün Açıklaması
- **user_id** - Ürüne yorum yapan kullanıcının kimliği
- **user_name** - Ürüne yorum yapan kullanıcının adı
- **review_id** - Kullanıcı yorumu kimliği
- **review_title** - Kısa yorum
- **review_content** - Uzun yorum
- **img_link** - Ürünün Görsel Bağlantısı
- **product_link** - Ürünün Resmi Web Sitesi Bağlantısı

## Kullanım

1. Depoyu klonlayın:
   ```bash
   git clone https://github.com/ErenalpYilmaz/veri_seti_incelemelerim.git
   ```
2. Bağımlılıkları yükleyin:
   ```bash
   pip install -r requirements.txt
   ```
3. Jupyter Notebook'u çalıştırın:
   ```bash
   jupyter notebook analyse.ipynb
   ```

## Bağımlılıklar

Bu analiz aşağıdaki kütüphaneler kullanılarak gerçekleştirilmiştir:

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn

(Gerekli diğer kütüphaneleri ekleyin.)

## Kod Örnekleri

Örneğin, veri kümesini yüklemek için aşağıdaki kod kullanılabilir:

```python
import pandas as pd

data = pd.read_csv("veri.csv")
print(data.head())
```

Bir histogram oluşturmak için:

```python
import matplotlib.pyplot as plt

data['rating'].hist()
plt.xlabel('Değer')
plt.ylabel('Frekans')
plt.title('Ürün Puanı Histogramı')
plt.show()
```

## Yazar

#### Erenalp Yılmaz @ErenalpYilmaz

## Lisans

Bu proje MIT Lisansı altında lisanslanmıştır - ayrıntılar için LICENSE dosyasına bakın.
