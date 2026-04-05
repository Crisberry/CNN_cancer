# Detección de Cáncer con Redes Neuronales Convolucionales

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/[TUUSUARIO/TUREPOSITORIO](https://github.com/Crisberry/CNN_cancer//blob/main/Taller_CNN_CristinaBerrio.ipynb)

## Descripción
Proyecto de clasificación de imágenes médicas para detectar presencia 
de cáncer usando arquitecturas CNN clásicas (LeNet-5 y AlexNet), 
desarrollado en Google Colab con GPU.

## Dataset
[Multi-Cancer Dataset — Kaggle](https://www.kaggle.com/datasets/obulisainaren/multi-cancer)
- 130.002 imágenes médicas de 8 tipos de cáncer
- Muestra utilizada: 2.000 imágenes por clase (4.000 total)
- Tamaño de imagen: 128x128 px

## Arquitecturas implementadas
- **LeNet-5** (LeCun, 1998) — arquitectura liviana, base histórica de las CNN
- **AlexNet** (Krizhevsky et al., 2012) — arquitectura profunda con Dropout y ReLU

## Resultados

| Modelo  | Accuracy | Sensibilidad | Especificidad | F. Negativos |
|---------|----------|--------------|---------------|--------------|
| LeNet-5 | 73.50%   | 71.5% 🏆     | 75.6%         | 118 🏆       |
| AlexNet | 75.50%   | 61.8%        | 90.2% 🏆      | 158          |

**Modelo recomendado según objetivo clínico:**
- **Detectar más cánceres reales** → LeNet-5 (mayor Sensibilidad)
- **Evitar falsas alarmas** → AlexNet (mayor Especificidad)

## 💾 Modelos preentrenados
Los modelos están disponibles en Google Drive público:
- [LeNet-5](https://drive.google.com/file/d/1Ry8v1uS6wDNxpS62NTFsYwNOjnK3i2RB/view?usp=drive_link)
- [AlexNet](https://drive.google.com/file/d/1I4c1twEhSZa9GFr5E5JnteXLH_2lyf3d/view?usp=drive_link)

## Cómo usar este proyecto

### Opción 1 — Solo lectura (recomendada)
Abre el cuaderno directamente en GitHub. Todas las salidas 
ya están guardadas — no necesitas ejecutar nada.

### Opción 2 — Ejecución sin re-entrenar
1. Activa GPU: *Entorno de ejecución → Cambiar tipo → GPU*
2. Ejecuta todas las celdas en orden
3. La Celda 5b descarga los modelos preentrenados automáticamente

### Opción 3 — Re-entrenamiento completo
Ejecuta todas las celdas incluyendo las de entrenamiento.  
Requiere ~30 minutos con GPU activada.

## Tecnologías
- Python 3
- TensorFlow / Keras
- Google Colab (GPU T4)
- KaggleHub

## 👤 Autor
**Tu Nombre Completo**  
Curso: Nombre del curso  
Fecha: Abril 2026
