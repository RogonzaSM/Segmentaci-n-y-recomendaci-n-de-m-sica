# 🎵 Segmentación y recomendación de música
Este es un proyecto de análisis de datos que utiliza la base de datos **Chinook** para aplicar **SQL, Python y Machine Learning** en la segmentación de clientes, predicción de ingresos y recomendación musical.

---

## 📌 Planteamiento del problema
Se quiere llegar a entender mejor cómo es que el entender a los clientes del mercado musical puede optimizar las ventas mediante recomendaciones de música que les pueda gustar.

---

## 🎯 Objetivos
- **General:** Desarrollar un proyecto de análisis y machine learning que combine SQL y Python para generar insights y modelos predictivos.
- **Específicos:**
  - Extraer y limpiar datos con SQL.
  - Analizar patrones de compra y segmentar clientes.
  - Construir un modelo de recomendación musical.
  - Predecir ingresos futuros por cliente.
  - Presentar resultados en dashboards y conclusiones claras.

---

## 🧩 Hipótesis
1. Los clientes pueden agruparse en segmentos con patrones de compra similares.  
2. Un sistema de recomendación basado en géneros y compras pasadas aumentaría la probabilidad de ventas futuras.  
3. Los ingresos futuros de un cliente pueden predecirse con base en su historial de compras, país y género favorito.  

---

## 📊 Metodología
1. **SQL:** Extracción de datos desde la base Chinook.  
2. **Python (pandas, matplotlib, seaborn):** Limpieza y análisis exploratorio.  
3. **Machine Learning (scikit-learn):**  
   - Clustering (K-Means) para segmentación.  
   - Recomendador basado en similitud.  
   - Modelos de regresión para predicción de ingresos.  
4. **Visualización:** Dashboards interactivos con Streamlit.  

---

## 📂 Estructura de notebooks
- `01_exploracion_chinook.ipynb` → Conexión y consultas básicas.  
- `02_clustering_clientes.ipynb` → Segmentación con K-Means.  
- `03_prediccion_ingresos.ipynb` → Regresión para predecir gasto.  
- `04_recomendador_musica.ipynb` → Sistema de recomendación y visualización.  

---

## 📓 Resultados por notebook

### 🔹 01 — Exploración de Chinook
- Los países con mayores ventas son **EE. UU. (523.06)**, **Canadá (303.96)**, **Francia (195.10)**, **Brasil (190.10)** y **Alemania (156.48)**.  
- El gráfico de barras muestra una clara concentración de ventas en Norteamérica y Europa occidental.  
**Interpretación:** se identificaron los mercados más rentables, lo que sirvió como base para los análisis posteriores de segmentación y predicción.  

---

### 🔹 02 — Clustering de clientes
- La mayoría de los clientes presentan un comportamiento muy similar: alrededor de **38 compras** y un gasto total entre **325–500 unidades**.  
- El modelo agrupó los clientes en **3 clusters**, aunque los datos muestran poca variabilidad, lo que sugiere una base homogénea.  
- Los países con clientes más activos incluyen **Alemania, Noruega, Bélgica, Canadá y EE. UU.**  
**Interpretación:** el clustering evidenció que la base Chinook contiene clientes con patrones casi idénticos, lo que abre la puerta a incorporar variables adicionales (género musical, frecuencia temporal) para mejorar la segmentación.  

---

### 🔹 03 — Predicción de ingresos
- **MSE:** 2.76 × 10⁻¹⁰  
- **R²:** 0.9999999999999228  
- El modelo logra una **predicción prácticamente perfecta** del gasto total, con valores reales y predichos alineados sobre la línea ideal.  
**Interpretación:** las variables de compra explican casi completamente el gasto del cliente. Aunque el resultado es casi perfecto, esto también refleja que el dataset tiene una estructura determinística, lo que invita a explorar modelos más complejos o variables externas para obtener predicciones más realistas.  

---

### 🔹 04 — Recomendador de música
- **Preferencias globales por género:** los géneros más comprados son **Rock, Latin y Metal**, seguidos por **Alternative & Punk** y **Jazz**.  
- **Promedio de canciones por cliente y género:** **Rock y Latin** tienen el mayor compromiso promedio por cliente.  
- **Preferencias individuales:** para un cliente específico, se grafican sus géneros más consumidos.  
- **Sistema de recomendación:** sugiere géneros a un cliente basándose en los gustos de clientes similares (ejemplo: para el cliente 1, se recomiendan **Rock, Latin y Jazz**).  
**Interpretación:** el análisis combina una visión **macro** (tendencias globales de géneros) con una visión **micro** (recomendaciones personalizadas), mostrando cómo los datos pueden usarse para segmentar, predecir y recomendar.  

---

## 🚀 Conclusión
El proyecto demuestra un flujo completo de **Data Science aplicado a SQL y Machine Learning**:  
1. Extracción y análisis con SQL.  
2. Exploración y visualización con Python.  
3. Segmentación con clustering.  
4. Predicción con regresión.  
5. Recomendación personalizada.  

Esto evidencia la capacidad de manejar todo el ciclo de un proyecto de datos, desde la base hasta la aplicación práctica.  

---

## 🚀 Tecnologías utilizadas
- Python (pandas, matplotlib, scikit-learn, SQLAlchemy)  
- MySQL (Workbench + base Chinook)  
- Jupyter Notebook (Anaconda)  
- GitHub (portafolio)  

---

## 📌 Cómo usar
1. Clonar este repositorio.  
2. Importar la base **Chinook** en MySQL.  
3. Abrir los notebooks en Jupyter.  
4. Ejecutar cada notebook en orden para reproducir el flujo completo.  

---

## ✨ Autor
**Roberto González Espinosa de los Monteros**  
Clinical Logistic Specialist | Data Scientist en formación
