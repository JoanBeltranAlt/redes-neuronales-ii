# Redes Neuronales II

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![PyTorch](https://img.shields.io/badge/PyTorch-red)
![Colab](https://img.shields.io/badge/Google%20Colab-ready-yellow)

Segunda práctica de la serie de Deep Learning: profundiza en **backpropagation**, **funciones de activación** (Sigmoide y ReLU), **clasificación binaria** y **clasificación multiclase** sobre el dataset **MNIST**, implementadas desde cero con NumPy y replicadas con **TensorFlow + Keras** y **PyTorch**. No se usan redes convolucionales.

Continúa la entrega anterior: [redes-neuronales-basicas](https://github.com/JoanBeltranAlt/redes-neuronales-basicas) (perceptrón, red de una capa y MLP vainilla).

**Repositorio:** https://github.com/JoanBeltranAlt/redes-neuronales-ii
**Entorno:** Google Colab

[![Abrir Notebook 1 en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JoanBeltranAlt/redes-neuronales-ii/blob/main/01_Backprop_Activaciones_Clasificacion_Binaria.ipynb)
[![Abrir Notebook 2 en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JoanBeltranAlt/redes-neuronales-ii/blob/main/02_MNIST_Multiclase_TensorFlow_PyTorch.ipynb)

---

## Objetivo de la práctica

Profundizar en los fundamentos de Deep Learning trabajados en la entrega anterior, incorporando:

- El algoritmo de **backpropagation** aplicado con distintas funciones de activación (Sigmoide, ReLU).
- **Clasificación binaria** sobre un dataset no linealmente separable (dos semilunas entrelazadas).
- **Clasificación multiclase** sobre datos reales (dígitos manuscritos MNIST).
- El uso de frameworks especializados de Deep Learning: **TensorFlow + Keras** y **PyTorch**.

## Estructura del repositorio

```
redes-neuronales-ii/
├── 01_Backprop_Activaciones_Clasificacion_Binaria.ipynb
├── 02_MNIST_Multiclase_TensorFlow_PyTorch.ipynb
├── Redes_Neuronales_II_Documento_Tecnico.pdf
└── README.md
```

## Contenido

### Notebook 1 — Backpropagation, activaciones y clasificación binaria

| Sección | Descripción |
|---|---|
| 1 | Funciones de activación Sigmoide y ReLU, y sus derivadas |
| 2 | Dataset sintético de dos semilunas (no linealmente separable), generado con NumPy |
| 3 | MLP "vainilla" desde cero con backpropagation, comparando Sigmoide vs. ReLU en la capa oculta |
| 4 | La misma arquitectura implementada con TensorFlow + Keras |
| 5 | La misma arquitectura implementada con PyTorch |
| 6-7 | Comparación de resultados y conclusiones |

### Notebook 2 — Clasificación multiclase con MNIST

| Sección | Descripción |
|---|---|
| 0-1 | Carga y preprocesamiento del dataset MNIST (70,000 imágenes de dígitos 0-9) |
| 2 | Red densa multiclase (784→128→64→10, softmax) con TensorFlow + Keras |
| 3 | La misma arquitectura con PyTorch (CrossEntropyLoss) |
| 4-5 | Comparación de resultados, evidencias de ejecución y conclusiones |

Ninguno de los dos notebooks utiliza capas convolucionales (CNN), conforme al alcance definido para esta actividad.

## Modelos y técnicas implementadas

- **Perceptrón, red de una capa y red multicapa**: base heredada de la entrega anterior, ahora extendida con ReLU y clasificación binaria sobre datos no lineales.
- **Backpropagation**: implementado manualmente con NumPy (regla de la cadena, gradientes por capa) y de forma automática (autograd) en Keras y PyTorch.
- **Funciones de activación**: Sigmoide, ReLU y Softmax (para la capa de salida multiclase).
- **Clasificación binaria**: MLP con salida sigmoide + pérdida binary cross-entropy, sobre un dataset de dos semilunas.
- **Clasificación multiclase**: red densa con salida softmax + pérdida (sparse) categorical cross-entropy, sobre MNIST.

## Cómo ejecutarlo

1. Entrar a [Google Colab](https://colab.research.google.com/) o hacer clic en los badges de arriba.
2. Si se abre manualmente: `Archivo → Abrir notebook → GitHub`, pegar la URL de este repositorio y seleccionar el notebook deseado.
3. Ejecutar todas las celdas en orden (`Entorno de ejecución → Ejecutar todas`).
4. TensorFlow y PyTorch ya vienen preinstalados en Google Colab; no se requiere instalación adicional. MNIST se descarga automáticamente al ejecutar las celdas correspondientes.

## Requisitos cumplidos

- [x] Desarrollo individual en Google Colab.
- [x] Backpropagation implementado y explicado.
- [x] Funciones de activación Sigmoide y ReLU aplicadas y comparadas.
- [x] Clasificación binaria (MLP desde cero + Keras + PyTorch).
- [x] Clasificación multiclase con TensorFlow + Keras (MNIST, sin CNN).
- [x] Clasificación multiclase con PyTorch (MNIST, sin CNN).
- [x] Resultados y evidencias de ejecución incluidos en los notebooks.
- [x] Código fuente funcional, comentado y documentado.
- [x] Notebooks ejecutados de extremo a extremo sin errores.
- [x] Publicado en repositorio GitHub con enlace funcional.
- [x] Documento técnico en PDF con código, explicaciones, resultados y enlace al repositorio.

## Autor

**Estudiante:** Joan Schneider Beltrán Delgado
**Correo institucional:** jsbeltran@ucundinamarca.edu.co
**Asignatura:** Deep Learning – Conceptos
**Institución:** Universidad de Cundinamarca – Posgrados
