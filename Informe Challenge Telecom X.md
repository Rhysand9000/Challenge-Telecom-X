
# Informe de Análisis de Evasión de Clientes (Churn) - Telecom X

## Introducción

Este informe tiene como objetivo analizar el fenómeno de la evasión de clientes (churn) en una empresa de telecomunicaciones ficticia llamada **Telecom X**. El propósito es identificar patrones y factores asociados a la cancelación del servicio por parte de los clientes, proporcionando insights que puedan guiar acciones estratégicas para reducir dicha evasión.

---

## Limpieza y Tratamiento de Datos

Se realizaron los siguientes pasos para asegurar la calidad de los datos:

- **Importación de Datos:** Se cargaron los datos desde un archivo JSON alojado en un repositorio de GitHub.
- **Transformación:** Se desanidaron columnas con estructuras de diccionario para obtener un DataFrame plano y manipulable.
- **Verificación de inconsistencias:** Se revisaron valores nulos, duplicados, tipos de datos y valores únicos por categoría.
- **Corrección de inconsistencias:** Se transformaron campos no numéricos, se aseguraron formatos válidos y se creó una nueva columna `Cuentas_Diarias`, dividiendo el total facturado entre 30 días.

---

## Análisis Exploratorio de Datos

Se calcularon métricas estadísticas como la media, mediana y desviación estándar para las variables numéricas, y se exploró la distribución de los datos categóricos y numéricos en función del churn.

### Evasión Global

- Se identificó el porcentaje general de clientes que cancelaron el servicio frente a los que permanecieron.

### Evasión por Variables Categóricas

Se analizaron las tasas de cancelación en función de:

- **Género**
- **Tipo de Contrato**
- **Método de Pago**

Esto permitió detectar patrones de evasión en ciertos segmentos de clientes.

### Evasión por Variables Numéricas

Se evaluaron variables como:

- **Cargos Totales**
- **Tiempo de Contrato (tenure)**

con el objetivo de ver si existen diferencias significativas entre quienes cancelaron y quienes no.

---

## Conclusiones e Insights

- Los clientes con contratos **mes a mes** presentan mayores tasas de cancelación que los que tienen contratos anuales.
- Aquellos con cargos mensuales más bajos o que han estado menos tiempo en la empresa tienen mayor propensión a cancelar.
- El método de pago también muestra relación con la evasión, especialmente entre quienes no usan tarjeta bancaria.

---

## Recomendaciones

- **Incentivar contratos a largo plazo**, como descuentos por contratos anuales.
- **Mejorar los servicios de atención y retención** en los primeros meses de relación con el cliente.
- **Segmentar campañas de fidelización** basadas en el perfil de clientes con mayor probabilidad de evasión.

---

## Análisis Extra: Correlación entre Variables (Opcional)

Se exploraron correlaciones entre:

- **Cuentas_Diarias y churn:** Clientes que pagan más por día tienden a cancelar más.
- **Cantidad de servicios contratados y churn:** A mayor cantidad de servicios, menor probabilidad de evasión.

Estas relaciones pueden alimentar modelos predictivos para anticipar la cancelación de clientes.

---
