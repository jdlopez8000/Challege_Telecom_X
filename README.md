# 📊 Telecom X - Análisis de Evasión de Clientes (Churn Analysis)

Análisis de ciencia de datos realizado para identificar patrones y factores clave asociados a la **evasión de clientes (churn)** en la empresa **Telecom X**.

---

## 🚀 Objetivo del Proyecto

El objetivo de este proyecto es explorar, limpiar y analizar un conjunto de datos de clientes de Telecom X para identificar patrones que expliquen por qué ciertos clientes deciden cancelar sus servicios. Este análisis servirá como base para futuras estrategias de retención y desarrollo de modelos predictivos.

---

## 🛠️ Tecnologías y Librerías Utilizadas

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Requests

---

## 📦 Instalación

Instala las dependencias necesarias ejecutando:

```bash
pip install pandas numpy matplotlib seaborn requests plotly

```

## 🧪 Fases del Análisis

### 1. 🔍 Extracción de Datos
- Se cargaron los datos desde una API pública en formato JSON:  
  [`TelecomX_Data.json`](https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/main/TelecomX_Data.json)
- Se transformaron estructuras anidadas en un DataFrame plano.

### 2. 🧹 Limpieza y Transformación
- Se manejaron valores nulos, vacíos y duplicados.
- Se estandarizaron columnas categóricas (e.g., `Yes/No` a `1/0`).
- Se crearon nuevas variables como `Cuentas_Diarias`.
- Conversión de datos numéricos a formato adecuado (`TotalCharges`, `tenure`, etc.).

### 3. 📈 Análisis Exploratorio (EDA)
- Distribución de la variable objetivo `Churn`.
- Análisis por variables categóricas y numéricas.
- Visualizaciones de distribución y boxplots por grupo de churn.
- Matriz de correlación para variables numéricas.
- Segmentación por grupos de tiempo (`tenure`) y facturación mensual (`MonthlyCharges`).

---

## 📊 Principales Hallazgos

- **Tasa de evasión general:** ~26.5%

### Tiempo promedio de contrato:
- Clientes que se van: ~17 meses  
- Clientes que permanecen: ~33 meses

### Facturación mensual promedio:
- Clientes que se van: ~$74.42  
- Clientes que permanecen: ~$61.27

---

## 🧠 Insights Destacados

- Clientes con **contratos más cortos** tienden a cancelar más.
- Aquellos con **mayores cargos mensuales** presentan mayor churn.
- Algunos **métodos de pago** y tipos de contrato se asocian con tasas altas de cancelación.
- Variables **demográficas** también pueden influir en la retención.

---

## 📌 Recomendaciones Estratégicas

- 🎯 Enfocar retención en nuevos clientes con menos de 12 meses.
- 💰 Ajustar precios para clientes de alto valor.
- 📋 Promover contratos de mayor duración con beneficios.
- 🔄 Mejorar experiencia de usuario en métodos de pago.
- 👥 Segmentar campañas según perfil demográfico.
- 📞 Implementar sistema de alertas tempranas basado en patrones identificados.


