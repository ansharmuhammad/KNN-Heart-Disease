# KNN Heart Disease

Case based reasoning untuk deteksi kemungkinan penyakit jantung menggunakan algoritmas KNN

## Data

data yang dipakai merupakan data penyakit jantung dari Cleveland Clinic Foundation. [sumber](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)

Sample data :

| Indeks | age  | sex | cp  | trestbps | chol  | fbs | restecg | thalach | exang | oldpeak | slope | ca  | thal | target |
|--------|------|-----|-----|----------|-------|-----|---------|---------|-------|---------|-------|-----|------|--------|
| 0      | 63.0 | 1.0 | 1.0 | 145.0    | 233.0 | 1.0 | 2.0     | 150.0   | 0.0   | 2.3     | 3.0   | 0.0 | 6.0  | 0      |
| 1      | 67.0 | 1.0 | 4.0 | 160.0    | 286.0 | 0.0 | 2.0     | 108.0   | 1.0   | 1.5     | 2.0   | 3.0 | 3.0  | 1      |
| 2      | 67.0 | 1.0 | 4.0 | 120.0    | 229.0 | 0.0 | 2.0     | 129.0   | 1.0   | 2.6     | 2.0   | 2.0 | 7.0  | 1      |

keterangan fitur :

- age — age in years
- sex — (1 = male; 0 = female)
- cp — chest pain type
- trestbps — resting blood pressure (in mm Hg on admission to the hospital)
- chol — serum cholestoral in mg/dl
- fbs — (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
- restecg — resting electrocardiographic results
- thalach — maximum heart rate achieved
- exang — exercise induced angina (1 = yes; 0 = no)
- oldpeak — ST depression induced by exercise relative to rest
- slope — the slope of the peak exercise ST segment
- ca — number of major vessels (0–3) colored by flourosopy
- thal — 3 = normal; 6 = fixed defect; 7 = reversable defect
- target — have disease or not (1=yes, 0=no)

## Metode yang digunakan

### K-Nearest Neighbour

Algoritma k-Nearest Neighbor adalah algoritma supervised
learning dimana hasil dari instance yang baru diklasifikasikan berdasarkan mayoritas dari kategori k-tetangga terdekat.
pada kasus ini nilai K yang digunakan adalah 5

![KNN](https://machine-learning-course.readthedocs.io/en/latest/_images/knn.png)

### Minkowski Distance

Distance yang digunakan pada algoritma KNN dalam kasus ini adalah Minkowski Distance

![minkowski](https://www.oreilly.com/library/view/hands-on-unsupervised-learning/9781789348279/assets/07f5f198-bcf4-4f91-811d-a5bc867600af.png)

### KD-Tree

KD-Tree digunakan untuk indexing kasus. sehingga dapat mempercepat hasil pencarian kasus

![kd-tree](https://www.researchgate.net/profile/Oliver_Guenther/publication/2334587/figure/fig9/AS:349387994746891@1460311998030/Adaptive-k-d-tree.png)


### Aplikasi

berikut tampilan aplikasi :

![app](https://user-images.githubusercontent.com/39853838/73133012-7c4c6280-4055-11ea-8575-839723a1d7c0.png)
