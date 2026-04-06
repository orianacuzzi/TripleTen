# 📈 Análisis de Clientes – ConnectaTel

## 🧠 Objetivo del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los clientes de *ConnectaTel* mediante técnicas de análisis de datos para entender cómo se relacionan con el uso de servicios (llamadas y mensajes) y características demográficas como la edad. A partir de este análisis se busca identificar segmentos de clientes relevantes y derivar recomendaciones para mejorar la oferta de planes y la estrategia de negocio.

---

## 📊 Datasets Utilizados

Se emplean los siguientes conjuntos de datos:

- plans.csv: los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).
- users_latam.csv: información de clientes: edad, ciudad, fecha de registro, plan contratado.
- usage.csv: el detalle de uso real: llamadas (duración) y mensajes (longitud).
  
Cada dataset contiene atributos que se usan para segmentar, analizar patrones de comportamiento y visualizar tendencias.

---

## 🔍 Etapas del Análisis

El análisis se realizó siguiendo las siguientes etapas:

1. **Carga y exploración de datos**  
   - Lectura de archivos CSV y revisión de las columnas disponibles.
   - Identificación inicial de valores faltantes y sentinels.

2. **Limpieza de datos**  
   - Reemplazo de valores sentinel (como `-999` y “?”) por `NaN`.
   - Conversión de tipos y manejo de nulos.

3. **Segmentación de clientes**  
   - Definición de grupos de edad: *Joven*, *Adulto*, *Adulto Mayor*.
   - Clasificación de clientes según uso: *Bajo uso*, *Uso medio* y *Alto uso*.

4. **Visualización exploratoria**  
   - Gráficos `boxplot` para detectar posibles outliers.
   - `countplot` para analizar la distribución de segmentos de edad y uso.

5. **Interpretación y recomendaciones**  
   - Identificación de segmentos valiosos para negocio.
   - Generación de recomendaciones para optimizar planes y estrategias de retención.
