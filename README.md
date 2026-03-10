# 📊 Análisis de Churn de Clientes - TelecomX

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo analizar la **evasión de clientes (Churn)** en una empresa de telecomunicaciones llamada **TelecomX**.  

El churn ocurre cuando un cliente **deja de utilizar los servicios de una empresa**, lo que representa una pérdida de ingresos y un desafío importante para las compañías del sector telecomunicaciones.

El propósito del análisis es **identificar patrones y factores asociados a la cancelación del servicio**, con el fin de generar **insights que permitan diseñar estrategias para mejorar la retención de clientes**.

---

## 🎯 Objetivos del Análisis

- Comprender la distribución de clientes que **permanecen y cancelan el servicio**.
- Analizar variables demográficas, contractuales y de consumo.
- Identificar **factores asociados al churn**.
- Proponer **recomendaciones estratégicas para reducir la evasión de clientes**.

---

## 🗂️ Dataset

El dataset contiene información sobre clientes de TelecomX, incluyendo:

- Información demográfica del cliente
- Servicios contratados
- Tipo de contrato
- Método de pago
- Facturación mensual y total
- Tiempo de permanencia del cliente
- Estado de churn (si el cliente canceló o no el servicio)

Variables importantes del dataset:

- `customerID`
- `Churn`
- `customer_gender`
- `customer_SeniorCitizen`
- `customer_Partner`
- `customer_Dependents`
- `customer_tenure`
- `phone_PhoneService`
- `internet_InternetService`
- `account_Contract`
- `account_PaymentMethod`
- `account_Charges_Monthly`
- `account_Charges_Total`

---

## ⚙️ Tecnologías Utilizadas

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 🧹 Limpieza y Tratamiento de Datos

Durante esta etapa se realizaron las siguientes tareas:

- Importación de datos desde un archivo **JSON**.
- Conversión del dataset a un **DataFrame de Pandas**.
- Normalización de columnas anidadas.
- Verificación de valores nulos.
- Corrección de tipos de datos.
- Conversión de variables categóricas a formato binario cuando fue necesario.
- Creación de una nueva variable:

**Cuentas_Diarias**

Esta variable se calculó a partir de la facturación mensual para estimar el gasto diario del cliente.

---

## 📊 Análisis Exploratorio de Datos (EDA)

Se realizaron diversos análisis exploratorios para comprender la relación entre las variables y el churn.

### Distribución del Churn

Se observó que:

- **26.5% de los clientes cancelaron el servicio**
- **73.5% permanecen en la empresa**

---

### Análisis por Variables Categóricas

Se exploró el churn según variables como:

- Género
- Tipo de contrato
- Método de pago
- Tipo de servicio de internet

Esto permitió identificar patrones importantes en el comportamiento de los clientes.

---

### Análisis por Variables Numéricas

Se analizaron variables como:

- Tiempo de permanencia (`tenure`)
- Facturación mensual
- Facturación total

Los gráficos permitieron observar diferencias entre clientes que cancelaron y los que permanecieron.

---

## 🔎 Conclusiones e Insights

### Tasa general de churn

El **26.5% de los clientes cancelaron el servicio**, lo que representa un nivel importante de evasión.

---

### Variables categóricas más relevantes

**Tipo de contrato (`account_Contract`)**

Los clientes con **contratos mensuales (Month-to-month)** presentan una tasa de churn significativamente mayor.

**Tipo de internet (`internet_InternetService`)**

Los clientes con **Fiber optic** presentan mayor probabilidad de cancelar el servicio.

**Método de pago (`account_PaymentMethod`)**

Los clientes que utilizan **electronic check** muestran una tasa de churn más alta.

---

### Variables numéricas

**Tiempo de permanencia (`tenure`)**

Los clientes con **poca antigüedad en la empresa** presentan mayor probabilidad de abandonar el servicio.

**Gasto total (`Charges_Total`)**

Los clientes con **menor gasto acumulado** tienden a cancelar más frecuentemente.

---

### Variables menos relevantes

Las siguientes variables no mostraron diferencias significativas en churn:

- Género
- Presencia de pareja
- Dependientes

---

## 💡 Recomendaciones Estratégicas

### Incentivar contratos a largo plazo

Promover contratos de **1 o 2 años** mediante descuentos o beneficios exclusivos para reducir la evasión asociada a contratos mensuales.

---

### Optimizar métodos de pago

Analizar a los clientes que utilizan **electronic check** y ofrecer alternativas como pagos automáticos o débito bancario.

---

### Mejorar la experiencia de clientes nuevos

Dado que los clientes nuevos tienen mayor churn, se recomienda implementar:

- Programas de bienvenida
- Atención temprana
- Soporte proactivo

---

### Atención especial a clientes con Fiber optic

Evaluar posibles problemas de calidad del servicio o expectativas del cliente en este segmento.

---

## 📌 Conclusión

El análisis permitió identificar **patrones clave en el comportamiento de los clientes**, especialmente en relación con:

- tipo de contrato
- antigüedad del cliente
- método de pago
- tipo de servicio de internet

Estos hallazgos pueden ayudar a **diseñar estrategias de retención más efectivas**, reduciendo la tasa de churn y mejorando la satisfacción del cliente.

---

## 📎 Autor

Proyecto realizado por Timoteo Flavio Taya Ramos como parte de un **análisis exploratorio de datos (EDA)** enfocado en comprender la evasión de clientes en el sector de telecomunicaciones.
