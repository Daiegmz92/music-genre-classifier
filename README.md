# 🎧 Clasificador de Géneros Musicales con Deep Learning

Este proyecto utiliza redes neuronales convolucionales (CNN) y una arquitectura preentrenada (MobileNetV2) para clasificar géneros musicales a partir de espectrogramas Mel generados desde archivos `.wav`.

---

## 🎯 Objetivo

Predecir el género musical de una canción a partir de su representación visual (espectrograma), trabajando con 10 géneros distintos.

---

## 📦 Dataset

Usamos el [GTZAN Genre Collection](http://marsyas.info/downloads/datasets.html), que contiene 1000 archivos `.wav` de 30 segundos cada uno, distribuidos en 10 géneros:

- 🎸 Blues  
- 🎼 Classical  
- 🤠 Country  
- 🕺 Disco  
- 🎤 Hip-Hop  
- 🎷 Jazz  
- 🤘 Metal  
- 🎧 Pop  
- 🇯🇲 Reggae  
- 🎸 Rock  

---

## 🧠 Modelos utilizados

- **CNN personalizada**: 5 bloques convolucionales con capas de normalización y dropout.
- **MobileNetV2**: arquitectura preentrenada, adaptada al dataset con fine-tuning.

| Modelo             | Precisión en validación |
|--------------------|-------------------------|
| CNN personalizada  | 0.79                    |
| MobileNetV2        | 0.80                    |

---

## 📈 Resultados

### Matriz de confusión  
![Confusion Matrix](images/confusion_matrix.png)

### Curvas de entrenamiento  
![Loss Curve](images/loss_curve.png)  
![Accuracy Curve](images/accuracy_curve.png)

---

## 🛠️ Cómo usar

1. Cloná este repositorio:
```bash
git clone https://github.com/Daiegmz92/music-genre-classifier.git
cd music-genre-classifier

