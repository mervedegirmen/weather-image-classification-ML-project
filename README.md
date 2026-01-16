# Weather Image Classification with Machine Learning and Deep Learning

## Project Description (English)
This project focuses on automatically classifying weather images into four categories: **sunny, cloudy, rainy, and snowy**. Due to variations in lighting, camera angle, and atmospheric conditions, weather image classification represents a challenging and meaningful real-world machine learning problem.

The project implements and compares **two different approaches**:
1. A **classical machine learning approach** using handcrafted image features and a tree-based model.
2. A **deep learning approach** using a Convolutional Neural Network (CNN) trained directly on images.

---

## Implemented Approaches

### 1. Classical Machine Learning Approach
- Images are read using **OpenCV**
- Feature extraction is performed using:
  - Color-based features
  - Histogram / texture-like representations
- Extracted features are converted into tabular format
- Labels are encoded using **LabelEncoder**
- A **tree-based classifier (XGBoost)** is trained on the extracted features

### 2. Deep Learning Approach (CNN)
- A custom **Convolutional Neural Network** is implemented using **PyTorch**
- Images are fed directly into the network without manual feature extraction
- The CNN model is trained and evaluated on the same classification task

---

## Evaluation Metrics
Both models are evaluated and compared using:
- Accuracy
- Precision
- Recall
- F1-score (macro)
- Confusion Matrix

Additionally, comparative plots are generated to visualize model performance.

---

## Dataset Structure
The dataset is expected to follow a folder-per-class structure:
data/
  sunny_weather/
  cloudy_weather/
  rainy_weather/
  snowy_weather/


Each class should contain approximately **150–300 images**.

> Note: The dataset is not included in this repository.

---

## Technologies Used
- **Language:** Python
- **Libraries:**
  - NumPy
  - Pandas
  - OpenCV
  - scikit-learn
  - XGBoost
  - PyTorch
  - Matplotlib
- **Environment:** Jupyter Notebook

---

## How to Run
1. Install required dependencies:
```bash
pip install -r requirements.txt

```
# Makine Öğrenmesi ve Derin Öğrenme ile Hava Durumu Görüntü Sınıflandırma

## Proje Açıklaması (Türkçe)
Bu proje, hava durumu görüntülerini **güneşli, bulutlu, yağmurlu ve karlı** olmak üzere dört sınıfa otomatik olarak ayırmayı amaçlamaktadır. Görüntülerdeki ışık değişimleri, çekim açıları ve atmosfer koşullarındaki farklılıklar nedeniyle bu problem, gerçek dünya için anlamlı ve zorlu bir makine öğrenmesi problemidir.

Projede **iki farklı yaklaşım** uygulanmış ve karşılaştırılmıştır:
1. El ile çıkarılan görüntü özelliklerine dayalı **klasik makine öğrenmesi yaklaşımı**
2. Görüntülerden doğrudan öğrenen **CNN tabanlı derin öğrenme yaklaşımı**

---

## Uygulanan Yöntemler

### 1. Klasik Makine Öğrenmesi Yaklaşımı
- Görüntüler **OpenCV** kullanılarak okunmuştur
- Görüntülerden aşağıdaki özellikler çıkarılmıştır:
  - Renk tabanlı özellikler
  - Histogram / doku benzeri temsiller
- Elde edilen özellikler tablo (tabular) formata dönüştürülmüştür
- Etiketler **LabelEncoder** ile sayısallaştırılmıştır
- Çıkarılan özellikler kullanılarak **XGBoost tabanlı ağaç sınıflandırıcı** eğitilmiştir

### 2. Derin Öğrenme Yaklaşımı (CNN)
- **PyTorch** kullanılarak özel bir Evrişimsel Sinir Ağı (CNN) modeli oluşturulmuştur
- Görüntüler modele doğrudan verilmiştir, manuel özellik çıkarımı yapılmamıştır
- CNN modeli aynı sınıflandırma problemi için eğitilmiş ve test edilmiştir

---

## Değerlendirme Metrikleri
Her iki model aşağıdaki metrikler kullanılarak değerlendirilmiş ve karşılaştırılmıştır:
- Accuracy (Doğruluk)
- Precision (Kesinlik)
- Recall (Duyarlılık)
- F1-score (macro)
- Confusion Matrix (Karışıklık Matrisi)

Ayrıca modellerin performanslarını karşılaştırmak amacıyla grafikler oluşturulmuştur.

---

## Veri Kümesi Yapısı
Veri kümesinin aşağıdaki klasör yapısına sahip olması beklenmektedir:
data/
  sunny_weather/
  cloudy_weather/
  rainy_weather/
  snowy_weather/

 
Her sınıf için yaklaşık **150–300 görüntü** bulunması önerilmektedir.

> Not: Veri kümesi bu GitHub deposunda paylaşılmamıştır.

---

## Kullanılan Teknolojiler
- **Dil:** Python
- **Kütüphaneler:**
  - NumPy
  - Pandas
  - OpenCV
  - scikit-learn
  - XGBoost
  - PyTorch
  - Matplotlib
- **Ortam:** Jupyter Notebook

---

## Çalıştırma
1. Gerekli kütüphaneleri yükleyin:
```bash
pip install -r requirements.txt
 


