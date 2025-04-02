# Detección de Fraude con Isolation Forest

## Introducción

El fraude financiero es un problema creciente que impacta tanto a empresas como a usuarios. La detección temprana de transacciones fraudulentas es clave para minimizar pérdidas y mejorar la seguridad. Este proyecto utiliza **Isolation Forest**, un algoritmo de detección de anomalías, para identificar patrones sospechosos en transacciones.

## Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un modelo de detección de fraude basado en **Isolation Forest**. Se entrenó un modelo con datos históricos, generando un puntaje de anomalía que permite identificar transacciones potencialmente fraudulentas.

## Datos Utilizados

Los datos empleados contienen información relevante sobre transacciones, incluyendo:

- **Monto de la transacción**
- **Frecuencia de transacciones**
- **Ubicación de la transacción**
- **Método de pago utilizado**

> ⚠️ *Dado que la matriz de features completa es confidencial, no se incluye en este repositorio.*

## Acerca de Isolation Forest

**Isolation Forest** es un algoritmo de detección de anomalías que construye múltiples árboles de aislamiento (Isolation Trees). Su principio clave es que las anomalías se aíslan más rápidamente debido a su rareza o baja densidad en el espacio de características. La profundidad promedio de aislamiento se usa para asignar un puntaje de anomalía, permitiendo identificar fraudes sin necesidad de datos etiquetados.

**¿Cuándo es recomendable estandarizar?** 
- Si hay variables con escalas muy diferentes (ej. "monto" en miles y "frecuencia de compras" en unidades pequeñas) ✅ 
- Si hay valores extremos muy grandes que podrían afectar la distribución de las divisiones ✅ 
