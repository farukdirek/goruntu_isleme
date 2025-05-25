# YOLO ile Nesne Tespiti — Görüntü İşleme Projesi

Bu projede, YOLO algoritması kullanılarak nesne tespiti gerçekleştirilmiştir. Eğitim ve test işlemleri kendi özel veri setimiz ile Google Colab ortamında yapılmıştır.

## Proje İçeriği

Bu repoda aşağıdaki dosyalar ve açıklamaları yer almaktadır:

- `goruntu_isleme.ipynb`: Model eğitimi ve testinin adım adım gerçekleştirildiği Jupyter defteri.
- Kendi veri setinizin eğitime uygun şekilde hazırlanması ve Colab üzerinde kullanılması için gerekli yönergeler.

## Kurulum ve Kullanım

### 1. Bu Reponun Kopyalanması

```bash
git clone https://github.com/farukdirek/goruntu_isleme.git
```
### 2. Google Colab ile Açma

goruntu_isleme.ipynb dosyasını Google Colab üzerinde açın.

Tercihen A100 GPU kullanarak daha hızlı eğitim ve test gerçekleştirebilirsiniz.

Gerekli kütüphaneler kod içinde otomatik olarak kurulmaktadır.

### 3. Veri Seti
Kendi veri setinizi Google Drive’a yükleyin.

Notebook içinde belirtilen data.yaml, images, ve labels yollarını kendi Drive dosya yapınıza göre güncelleyin.

Dosya yollarının doğru verildiğinden emin olun!

### 4. Eğitimi Başlatmak
Notebook içinde adım adım açıklamalar mevcuttur. Sırasıyla:

Gerekli kütüphaneler yüklenir.

Drive bağlantısı yapılır.

YOLO modeli eğitilir ve test edilir.

Model çıktıları görselleştirilir.

## Model
Kullanılan model: YOLOv12

Eğitim süreci boyunca mAP, precision ve recall gibi metriklerle model başarımı değerlendirilmektedir.

Eğitim sonunda model .pt formatında kaydedilir.

## Notebook Colab üzerinde çalıştığı için tek ihtiyacınız bir Google hesabı. Yerel çalıştırmak isterseniz:

Python 3.10+

PyTorch

Ultralytics

OpenCV

kütüphanelerini kurmalısınız.

## Uyarılar
Veri seti boyutuna göre eğitim süresi değişebilir.

Dosya yollarını kendi Google Drive yapınıza göre düzenlemeyi unutmayın.

Colab oturumları belirli bir süreden sonra sona erebilir; modeli ara sıra kaydedin.
