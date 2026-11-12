# Mustafa Sarı | Bilgisayar Mühendisliği ve Yapay Zeka 

Yapay zeka alanında, özellikle bilgisayarlı görü üzerine projeler geliştiren bilgisayar mühendisliği öğrencisiyim.

---

## Dataguess | Endüstriyel Yapay Zeka

Dataguess'te yapay zeka mühendisliği stajımı yapıyorum ve üretim hatları için görüntü işleme modelleri geliştiriyorum. Veri gizliliği nedeniyle çalışmalarımın yalnızca bazı kısımlarını paylaşıyorum.

### Pres hattında hata tespiti
Sıcak pres hattından çıkan metal parçalardaki hataların tespiti için geliştirilen bir model.

<p align="center">
  <img src="images/dataguess/press_etiket.jpg" width="400">
  <img src="images/dataguess/press_hat.jpg" width="400">
</p>

**Model:** YOLOv11 Nano · 1024×1024

<p align="center">
  <img src="images/dataguess/press_egitim_sonuclari.jpg" width="800">
</p>
<p align="center">
  <img src="images/dataguess/press_confusion_matrix.jpg" width="400">
</p>

**Precision** 0.97 · **Recall** 0.97 · **mAP50** 0.98 · **mAP50-95** 0.72

### Kamera ile cam panel ölçümü
Cam panelin en ve boyunu, pişirme bölgelerinin konum ve çaplarını ölçüp teknik resimle karşılaştıran ve OK/NOK sonucu veren bir ölçüm sistemi.

<p align="center">
  <img src="images/dataguess/cam_panel_olcum.jpg" width="800">
</p>

**Yöntem:** Distorsiyon ve perspektif düzeltmesi · Parçanın kendisiyle kalibrasyon · Alt-piksel kenar tespiti · Daire uydurma

**Sonuç:** ±0.02 mm tekrarlanabilirlik · Ölçüm başına ~5 sn

**Teknolojiler:** Python · OpenCV · NumPy · DepthAI

### Diğer örnek çalışmalar
Farklı üretim alanlarında yer aldığım POC ve saha çalışmalarından örnekler.

<p align="center">
  <img src="images/dataguess/poc_plastik_parca.jpg" width="260">
  <img src="images/dataguess/saha_etiket.jpg" width="260">
  <img src="images/dataguess/poc_elektronik_kart.jpg" width="260">
</p>

---

## Öne Çıkan Projeler

### 1. Mutabık: Fiş OCR ve Mutabakat Sistemi
Fiş fotoğrafını OCR ile okuyup sonucu Matrah + KDV = Toplam kuralıyla doğrulayan sistem; tutmayan fişleri nedeniyle birlikte "şüpheli" işaretliyor.
* **Özellikler:** OpenCV ile ön işleme, PaddleOCR ile okuma, ödeme çapraz kontrolü, harcama paneli ve telefondan çekim için mobil PWA.
* **Teknolojiler:** Python, FastAPI, PaddleOCR, OpenCV, SQLite, Streamlit, Docker
* [Kaynak Kodları](https://github.com/Mustafa037/mutabik)

### 2. Dermatoskopik Görüntülerle Deri Kanseri Tespiti
ISIC 2018 veri seti üzerinde derin öğrenme mimarileri (YOLOv8, EfficientNet, ResNet, MobileNet) ile lezyon sınıflandırması.
* **Sonuç:** YOLOv8-Cls ile **%81.15 Doğruluk**, EfficientNet-B0 ile Melanom için **%74.26 Recall** başarısı.
* **Teknolojiler:** PyTorch, YOLOv8, Scikit-Learn
* [Kaynak Kodları & Rapor](https://github.com/Mustafa037/skin-cancer-classification-deep-learning)

### 3. Diyabet Risk Tahmini & Canlı Web Sistemi
Pima Indians Diabetes veri seti üzerinde klinik öznitelik mühendisliği uygulanarak geliştirilen canlı çıkarım uygulaması.
* **Özellikler:** Eksik veri iyileştirmesi, Glukoz/İnsülin oranı, BMI/yaş segmentasyonu ve Random Forest sınıflandırması.
* **Teknolojiler:** Python, Scikit-Learn, Streamlit, Pandas
* [Kaynak Kodları](https://github.com/Mustafa037/Diabetes-risk-prediction-app-ML)
* [Canlı Demo](https://diabetes-risk-prediction-app-ml-tkfrjp7u4vewzjcj9cjkfz.streamlit.app/)

### 4. Otomatik Araç Plaka Tanıma Sistemi
YOLOv8 tabanlı iki aşamalı bir bilgisayarlı görü hattı: önce araç görselinde plaka bölgesi tespit edilip kırpılıyor, ardından kırpılan plakadaki karakterler ayrı bir model ile tespit edilip konumlarına göre soldan sağa dizilerek plaka metni oluşturuluyor.
* **Özellikler:** Plaka tespiti ve kırpma, karakter bazlı nesne tespiti ile okuma (klasik OCR yerine özel eğitilmiş model), tek görselde birden fazla plaka desteği, tespit kutularıyla görselleştirilmiş sonuçlar.
* **Teknolojiler:** Python, YOLOv8 (Ultralytics), OpenCV, Streamlit, NumPy, Pillow
* [Kaynak Kodları](https://github.com/Mustafa037/number-plate-recognition-app)
* [Canlı Demo](https://number-plate-recognition-app-6sv7vxpkfkpk6w3pkt692l.streamlit.app/)

### 5. Machine Learning Cookbook
Veri keşfi (EDA), regresyon, SVM, Naive Bayes ve hiperparametre optimizasyonu çalışmalarımı içeren pratik öğrenme günlüğü.
* **Teknolojiler:** Scikit-Learn, Pandas, Seaborn
* [Notebook Havuzu](https://github.com/Mustafa037/machine-learning-exercises)

---
