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

```text
telecom-x-churn-analysis/
│
├── data/             # Archivos de datos (JSON original)
├── notebooks/        # Notebooks con análisis y visualizaciones
├── reports/          # Imágenes exportadas, informes PDF
├── scripts/          # Funciones o procesos de limpieza reutilizables
├── README.md         # Este archivo
└── requirements.txt  # Librerías necesarias para reproducir el proyecto 
```

---

## 🧪 Etapas del Análisis

### 1. 📥 Extracción y Carga de Datos
- Los datos fueron importados desde un archivo JSON alojado en GitHub.
- Se normalizaron estructuras anidadas con `json_normalize`.

### 2. 🧹 Limpieza y Transformación
- Conversión de tipos (`Charges.Monthly`, `tenure`).
- Eliminación de duplicados y valores nulos.
- Conversión de variables `Yes/No` a `1/0` y a texto para visualización.
- Traducción y estandarización de nombres de columnas.
- Cálculo de columna `Facturacion_Diaria`.

### 3. 📊 Análisis Exploratorio de Datos (EDA)
- Distribución general de evasión.
- Gráficos de evasión por género, tipo de contrato y método de pago.
- Análisis de churn según variables numéricas como facturación total y duración del contrato.

### 4. 📈 Análisis de Correlación (Opcional)
- Matriz de correlación de variables numéricas.
- Relación entre la cuenta diaria y la evasión.
- Análisis de cómo la cantidad de servicios contratados afecta el churn.

### 5. 📋 Informe Final
- Resumen detallado dentro del mismo notebook con visualizaciones.
- Incluye conclusiones y recomendaciones estratégicas.

---

## 💡 Principales Hallazgos

- Los clientes con **contrato mensual** tienen mayor tasa de evasión.
- Usuarios con **menos servicios contratados** tienden a cancelar más.
- La **facturación total o mensual** influye menos que la **duración del contrato**.
- Mayor proporción de cancelaciones ocurre en los **primeros meses**.

---

## 🧠 Recomendaciones

- Ofrecer descuentos o beneficios por contratar servicios anuales.
- Lanzar campañas dirigidas a nuevos clientes con menor uso de servicios.
- Detectar perfiles con alto riesgo de cancelación de forma temprana.
- Aplicar los insights en modelos predictivos de churn.

---

## ✅ Requisitos

Instala las dependencias necesarias con:

```bash
pip install -r requirements.txt
```

---

## 🤝 Autor

Renzo Echevarria 
Desafío de Ciencia de Datos – Telecom X  
🔗 [Repositorio en GitHub](https://github.com/tu-usuario/telecom-x-churn-analysis)
