# 🎧 Clasificador de Géneros Musicales con Deep Learning

Este proyecto utiliza redes neuronales convolucionales (CNN) y una arquitectura preentrenada (MobileNetV2) para clasificar géneros musicales a partir de espectrogramas Mel generados desde archivos .wav.

## 🎯 Objetivo
Predecir el género musical de una canción a partir de su representación visual (espectrograma), trabajando con 10 géneros distintos.

## 📦 Dataset
Usamos el GTZAN Genre Collection, que contiene 1000 archivos .wav de 30 segundos cada uno, distribuidos en 10 géneros:

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

## 🧠 Modelos utilizados
- **CNN personalizada:** 5 bloques convolucionales con capas de normalización y dropout.
- **MobileNetV2:** arquitectura preentrenada, adaptada al dataset con fine-tuning.

| Modelo            | Precisión en test |
|-------------------|-------------------|
| CNN personalizada | 0.81              |
| MobileNetV2       | 0.46              |

> **Nota:** MobileNetV2 mostró menor precisión posiblemente porque es una arquitectura más compleja y preentrenada para imágenes naturales, no para espectrogramas. El dataset pequeño y la posible necesidad de ajustar hiperparámetros o técnicas de regularización influyeron en su desempeño inferior.

## 📈 Resultados
- Matriz de confusión
- Curvas de entrenamiento (Loss y Accuracy)

## 🛠️ Cómo usar
Cloná este repositorio:
```bash
git clone https://github.com/Daiegmz92/music-genre-classifier.git
cd music-genre-classifier
