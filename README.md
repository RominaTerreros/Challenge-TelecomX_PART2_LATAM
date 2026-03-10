# 📊 Telecom X – Predicción de Cancelación (Churn)

## 📌 Descripción del Proyecto

La cancelación de clientes (*customer churn*) es uno de los principales desafíos para las empresas de telecomunicaciones, ya que impacta directamente en los ingresos y la estabilidad del negocio.

En este proyecto se desarrolla un análisis de datos y un modelo de **Machine Learning** para **predecir qué clientes tienen mayor probabilidad de cancelar el servicio** en Telecom X.

A través de técnicas de **análisis exploratorio de datos, preprocesamiento y modelado predictivo**, se identifican los factores que influyen en la cancelación de clientes y se generan **insights de negocio que pueden ayudar a mejorar las estrategias de retención**.

---

# 🎯 Objetivos

El objetivo principal del proyecto es:

* Analizar el comportamiento de los clientes de Telecom X.
* Identificar **patrones asociados a la cancelación del servicio (churn)**.
* Construir modelos de **Machine Learning** para predecir qué clientes tienen mayor riesgo de abandono.
* Extraer **insights de negocio** que ayuden a mejorar las estrategias de fidelización.

---

# 🛠️ Tecnologías Utilizadas

El proyecto fue desarrollado utilizando herramientas del ecosistema de **Data Science en Python**:

* **Python**
* **Pandas** – Manipulación de datos
* **NumPy** – Operaciones numéricas
* **Matplotlib / Seaborn** – Visualización de datos
* **Scikit-learn** – Modelos de Machine Learning
* **Google Colab / Jupyter Notebook**

---

# 📂 Estructura del Proyecto

El flujo de trabajo del análisis sigue las siguientes etapas:

1️⃣ **Carga y exploración de datos**

* Análisis inicial del dataset
* Identificación de variables
* Revisión de valores faltantes

2️⃣ **Preprocesamiento de datos**

* Limpieza de datos
* Codificación de variables categóricas
* Eliminación de columnas redundantes
* Preparación de variables predictoras

3️⃣ **División del dataset**

El dataset se dividió en:

* **80% entrenamiento**
* **20% prueba**

```
Train set: 5625 registros  
Test set: 1407 registros
```

4️⃣ **Normalización de variables**

Para modelos sensibles a la escala de los datos (como **Logistic Regression**) se aplicó:

* **StandardScaler**

Esto permite que las variables tengan **media 0 y desviación estándar 1**, evitando que variables con mayor magnitud dominen el modelo.

---

# 🤖 Modelos de Machine Learning

Se entrenaron dos modelos para la predicción de churn:

## 1️⃣ Logistic Regression

Modelo lineal utilizado comúnmente para **problemas de clasificación binaria**.

Resultados obtenidos:

| Métrica   | Valor |
| --------- | ----- |
| Accuracy  | 0.796 |
| Precision | 0.637 |
| Recall    | 0.540 |
| F1 Score  | 0.585 |

---

## 2️⃣ Random Forest

Modelo basado en **ensamble de árboles de decisión**, capaz de capturar relaciones no lineales.

Resultados obtenidos:

| Métrica   | Valor |
| --------- | ----- |
| Accuracy  | 0.781 |
| Precision | 0.620 |
| Recall    | 0.455 |
| F1 Score  | 0.525 |

---

# 📊 Importancia de Variables

El modelo **Random Forest** permitió identificar las variables más relevantes para la predicción de churn.

Top variables:

| Variable                       | Importancia |
| ------------------------------ | ----------- |
| Charges.Total                  | 0.191       |
| tenure                         | 0.178       |
| Charges.Monthly                | 0.162       |
| PaymentMethod_Electronic check | 0.041       |
| InternetService_Fiber optic    | 0.037       |

Estas variables indican que **el costo del servicio y la duración de la relación con el cliente son factores clave en la cancelación**.

---

# 🔎 Principales Hallazgos

### Clientes con mayor riesgo de cancelación

Los clientes con mayor probabilidad de churn presentan características como:

* Bajo **tiempo de permanencia (tenure)**
* **Facturas mensuales elevadas**
* Uso de **Electronic Check** como método de pago
* Contratos de corto plazo
* Ciertos tipos de servicio de internet

---

### Variables que más influyen en el churn

Las variables con mayor impacto en el modelo fueron:

* **Charges.Total**
* **tenure**
* **Charges.Monthly**

Estas variables reflejan principalmente **el costo del servicio y la duración de la relación con el cliente**.

---

# 💡 Insights de Negocio

A partir del análisis se identifican posibles estrategias para reducir el churn:

* Implementar **programas de fidelización en los primeros meses del cliente**.
* Ofrecer **planes más flexibles o promociones personalizadas**.
* Incentivar **contratos de largo plazo**.
* Promover **métodos de pago automáticos**.

Estas estrategias pueden ayudar a **reducir la tasa de cancelación y mejorar la retención de clientes**.

---

# 📈 Conclusión

El análisis demuestra que el uso de **Machine Learning y análisis de datos** permite identificar patrones de comportamiento asociados al abandono de clientes.

Entre los modelos evaluados, **Logistic Regression mostró un mejor desempeño general**, con un **Accuracy de 0.796 y un F1 Score de 0.585**, superando ligeramente al modelo Random Forest.

Además, el análisis de importancia de variables permitió identificar factores clave en la cancelación de clientes, como:

* el **costo del servicio**
* el **tiempo de permanencia**
* el **método de pago**

Estos hallazgos pueden ayudar a Telecom X a implementar **estrategias de retención basadas en datos**, reduciendo el churn y mejorando la estabilidad del negocio.

---

# 👩‍💻 Autora

**Rommina Terreros Cotera**

