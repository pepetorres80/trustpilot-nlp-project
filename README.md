# 📊 Análisis de reseñas con NLP — Airtime Rewards

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

---

## 🧠 Conclusión

El análisis revela que Airtime Rewards presenta problemas estructurales en su sistema de recompensas, afectando directamente a la experiencia del cliente.

La mejora del sistema de cashback es clave para aumentar la satisfacción y competitividad en el mercado.

---

## 👨‍💻 Autor

Torres — Proyecto de Machine Learning / NLP
