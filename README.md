# 🚚 Dashboard de Capacidad Logística y Flota Vehicular — Perú (MTC)

## 📖 Contexto y Problema de Negocio
En la gestión de la cadena de suministro, la infraestructura vial y la capacidad de la flota son factores relevantes para analizar la conectividad y la oferta potencial de transporte. Este proyecto presenta un diagnóstico descriptivo del transporte terrestre de carga y de la infraestructura vial del Perú, utilizando datos públicos del Ministerio de Transportes y Comunicaciones (MTC).

El objetivo es proporcionar contexto analítico para la planificación logística, el análisis regional de la oferta de transporte y la formulación de preguntas para futuras evaluaciones de rutas y proveedores logísticos.

## 📊 KPIs Clave Medidos
* **Flota autorizada:** 373,240 vehículos de carga registrados a nivel nacional.
* **Composición y combustible:** Los camiones representan el 56% de la flota y el diésel corresponde al 75.5% del combustible registrado.
* **Antigüedad de la flota:** Promedio de 13.4 años. Entre los registros con año de fabricación válido, el 47.8% tiene menos de 10 años y el 28.8% supera los 15 años.
* **Sistema Nacional de Carreteras:** Análisis de más de 177,780 km distribuidos entre las redes nacional, departamental y vecinal.

## 🛠️ Herramientas utilizadas
* **Microsoft Power BI:** Modelado de datos, creación de medidas DAX y visualización interactiva. Proyecto guardado en formato avanzado `.pbip` para un control de versiones estructurado.
* **Procesamiento de Datos:** Limpieza y transformación de bases de datos gubernamentales complejas (Excel/Power Query).

## 📚 Fuentes de datos
Power BI carga cuatro archivos oficiales mediante enlaces web definidos en el modelo:

| Datos | Archivo utilizado | Publicación oficial |
| :--- | :--- | :--- |
| Empresas autorizadas | XLSX | Servicios de carga — MTC |
| Parque vehicular por departamento | XLSX | Parque automotor — MTC |
| Red vial por departamento | XLSX | Infraestructura vial — MTC |
| Detalle de flota de carga 2025 | CSV | Datos Abiertos — MTC |

## 🔁 Cómo reproducir el proyecto
Abre el archivo `.pbip` en Power BI Desktop y actualiza los datos con conexión a internet. Si el MTC modifica alguna URL de descarga, habrá que actualizar el parámetro correspondiente en Power Query.

> **Nota metodológica:** La serie departamental muestra 373,240 vehículos autorizados, mientras que el detalle de flota contiene 373,237 placas únicas. Son dos formas distintas de contar y no deben confundirse.

## ⚠️ Alcance y limitaciones
El análisis es descriptivo y se basa en registros administrativos y datos públicos del MTC. Los resultados muestran la distribución registrada de la flota y las características de la infraestructura vial, pero no representan necesariamente la disponibilidad operativa en tiempo real.

El dashboard no mide directamente tiempos de entrega, costos logísticos, utilización de capacidad, nivel de servicio, accidentabilidad, mantenimiento ni desempeño individual de los transportistas. Por ello, sus hallazgos deben utilizarse como contexto para el análisis logístico y como punto de partida para investigaciones posteriores.

## 📸 Vista Previa del Dashboard
*<img width="1920" height="1080" alt="Captura de pantalla (215)" src="https://github.com/user-attachments/assets/a543d069-09ae-47de-8105-ca861a780ab0" />
<img width="1920" height="1080" alt="Captura de pantalla (214)" src="https://github.com/user-attachments/assets/f656e268-1322-4b84-87b9-5137739d3988" />
<img width="1920" height="1080" alt="Captura de pantalla (213)" src="https://github.com/user-attachments/assets/aa3dd4a4-b159-47dc-bd40-00323b4d69d0" />*

## 💡 Principales Hallazgos (Insights)
* **Extrema Centralización:** Lima concentra abrumadoramente la capacidad logística (288,229 vehículos autorizados). Esto describe dónde están registrados, no dónde circulan en cada momento.
* **Reto Logístico en Última Milla:** El 68.6% de la red vial nacional es de carácter vecinal, pero apenas el 3.5% de sus kilómetros figura como pavimentado. Esto impacta directamente incrementando el *lead time* y los costos de mantenimiento vehicular en rutas remotas.
* **Antigüedad de la flota:** Entre las placas con año de fabricación válido, el 28.8% corresponde a vehículos de más de 15 años, siendo un factor de riesgo (averías, ineficiencia) indispensable a evaluar durante las licitaciones y homologaciones de transporte.

---
**Autor:** Katherine Palomino | Especialista en Supply Chain Management y Compras Estratégicas.
