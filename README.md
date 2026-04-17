# 📊 NLP aplicado a reseñas de Trustpilot

Análisis de la experiencia del cliente en Airtime Rewards mediante técnicas de Machine Learning y Procesamiento de Lenguaje Natural.

---

## 🚀 Resultados clave

- 60% de reseñas negativas  
- Problema central en el sistema de recompensas  
- Diferencias estructurales frente a la competencia  

👉 Insight clave:

**El problema no está en el servicio, sino en el producto, y este patrón se mantiene consistente en todos los enfoques analíticos aplicados (LDA, grafos y BERTopic)**

# 📊 Análisis de reseñas con NLP — Airtime Rewards

![Python](https://img.shields.io/badge/Python-3.10-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-NLP-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 🧠 Descripción

Este proyecto analiza reseñas de clientes de Trustpilot utilizando técnicas de Procesamiento de Lenguaje Natural (NLP) con el objetivo de entender la experiencia del cliente, identificar problemas clave y comparar el posicionamiento de Airtime Rewards frente a sus competidores.

El enfoque se centra en transformar datos textuales en **insights de negocio accionables**.

---

## 🎯 Objetivos

* Analizar el sentimiento de los clientes
* Identificar los principales temas (topics) en las reseñas
* Relacionar temas con sentimiento
* Comparar Airtime Rewards con empresas del mismo sector
* Detectar áreas clave de mejora

---

## 📂 Dataset

Se utilizan dos fuentes de datos:

* **Trustpilot Reviews Dataset** (~123.000 reseñas)
* **Empresas con 100 reseñas** (subset proporcionado)

Variables principales:

* `review`: texto de la reseña
* `stars`: puntuación (1–5)
* `company`: nombre de la empresa
* `category`: sector

---

## ⚙️ Metodología

### 1. Selección de empresa

Se selecciona **Airtime Rewards** por su relevancia dentro del sector financiero y su potencial analítico.

---

### 2. Preprocesamiento de texto

* Conversión a minúsculas
* Eliminación de caracteres especiales
* Eliminación de stopwords
* Lematización

---

### 3. Análisis de sentimiento

Clasificación basada en la puntuación:

* Positivo → ≥ 4
* Negativo → < 4

---

### 4. Modelado de temas (Topic Modeling)

* Uso de LDA (Latent Dirichlet Allocation)
* Identificación de los principales temas en las reseñas

---

### 5. Relación topic–sentimiento

Análisis del sentimiento asociado a cada tema para detectar:

* Fortalezas
* Problemas estructurales

---

### 6. Análisis de competencia

* Selección de empresas del mismo sector
* Comparación basada en topics (no en sentimiento global debido al dataset balanceado)

---

### 7. Análisis mediante grafos

* Grafo de co-ocurrencia de palabras
* Grafo de similitud entre empresas

Permite identificar:

* Conceptos clave
* Relaciones entre temas
* Posicionamiento competitivo

---

### 8. Validación con BERTopic

* Aplicación de BERTopic (modelo basado en embeddings)
* Validación de los temas obtenidos con LDA
* Confirmación de consistencia en los patrones detectados

## 🔍 Resultados principales

* El **60% de las reseñas son negativas**
* El sistema de **recompensas (cashback)** es el eje central de la experiencia
* Los principales problemas se encuentran en:

  * Fallos en recompensas
  * Transacciones
  * Percepción de valor

👉 Insight clave:

**El problema no está en el servicio, sino en el producto**

---

## 🆚 Comparación con competencia

* Airtime Rewards presenta problemas en su propuesta de valor
* La competencia muestra problemas más operativos
* Mayor similitud con empresas centradas en transacciones

---

## ⚠️ Limitaciones

* Dataset limitado a 100 reseñas por empresa
* Distribución de estrellas balanceada
* Sentimiento basado en ratings (no en modelo NLP puro)
* Interpretación subjetiva de topics

---

## 📁 Estructura del proyecto

```bash
data/
notebooks/
src/
outputs/
presentation/
README.md
```

---

## 🚀 Tecnologías utilizadas

* Python
* Pandas
* Scikit-learn
* NLTK
* NetworkX
* Matplotlib
* BERTopic

---

## 🧠 Conclusión

El análisis revela que Airtime Rewards presenta problemas estructurales en su sistema de recompensas, afectando directamente a la experiencia del cliente.

Estos resultados han sido consistentes a través de diferentes enfoques analíticos, incluyendo modelado de temas (LDA), análisis de grafos y validación mediante BERTopic, lo que refuerza la solidez de las conclusiones obtenidas.

La mejora del sistema de cashback es clave para aumentar la satisfacción y competitividad en el mercado.


---

## 👨‍💻 Autor

Torres — Proyecto de Machine Learning / NLP
