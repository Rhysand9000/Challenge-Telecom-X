# 📊 Telecom X – Análisis de Evasión de Clientes (Churn Analysis)

Este proyecto forma parte del desafío **Telecom X**, cuyo objetivo es analizar los factores que influyen en la **cancelación del servicio por parte de los clientes (churn)** y proponer estrategias basadas en datos para mejorar la **retención**.

---

## 📌 Objetivos

- Identificar patrones de comportamiento de los clientes que se dan de baja.
- Comprender la relación entre variables demográficas, de consumo y de contrato con la evasión.
- Proponer recomendaciones estratégicas basadas en los hallazgos.
- Servir como base para futuros modelos predictivos de churn.

---

## 🛠️ Herramientas y Librerías Utilizadas

- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn

---

## 📂 Estructura del Proyecto

telecom-x-churn-analysis/
│
├── data/             # Archivos de datos (JSON original)
├── notebooks/        # Notebooks con análisis y visualizaciones
├── reports/          # Imágenes exportadas, informes PDF
├── scripts/          # Funciones o procesos de limpieza reutilizables
├── README.md         # Este archivo
└── requirements.txt  # Librerías necesarias para reproducir el proyecto 


---

## 🧪 Etapas del Análisis

### 1. 📥 Extracción y Carga de Datos
- Los datos fueron importados desde un archivo JSON alojado en GitHub.
- Estructuras anidadas fueron aplanadas con `json_normalize`.

### 2. 🧹 Limpieza y Transformación
- Conversión de tipos (`Charges.Monthly`, `tenure`).
- Eliminación de duplicados y valores nulos.
- Conversión de variables `Yes/No` a `1/0` y a texto para gráficos.
- Traducción y estandarización de nombres de columnas.
- Cálculo de columna `Facturacion_Diaria`.

### 3. 📊 Análisis Exploratorio de Datos (EDA)
- Distribución general de evasión (churn).
- Gráficos de evasión por género, contrato y método de pago.
- Análisis de churn según variables numéricas como facturación total y tiempo de contrato.

### 4. 📈 Análisis de Correlación (Opcional)
- Matriz de correlación de variables numéricas.
- Relación entre cantidad de servicios contratados y churn.
- Correlación entre facturación diaria y evasión.

### 5. 📋 Informe Final
- Incluye introducción, limpieza, EDA, conclusiones, recomendaciones y análisis opcional de correlación.
- Generado dentro del mismo notebook.

---

## 💡 Principales Hallazgos

- Clientes con **contrato mensual** tienen una tasa de evasión significativamente mayor.
- Usuarios con **menos servicios contratados** tienden a cancelar más.
- La **facturación total y mensual** influye menos en la evasión que el tiempo de permanencia.
- Se detectan más cancelaciones durante los **primeros meses de servicio**.

---

## 🧠 Recomendaciones

- Promover contratos anuales con beneficios adicionales.
- Crear campañas de fidelización dirigidas a nuevos clientes.
- Monitorear usuarios con bajo uso de servicios para intervenir antes de que cancelen.
- Utilizar estos hallazgos para construir un modelo predictivo de churn.

---

## ✅ Requisitos

Instala las dependencias necesarias con:

```bash
pip install -r requirements.txt
