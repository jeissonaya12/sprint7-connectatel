# Análisis de Comportamiento de Usuarios - ConnectaTel

## 🎯 Objetivo del Proyecto
Analizar y segmentar el comportamiento de los clientes de una empresa de telecomunicaciones para identificar patrones de consumo (llamadas y mensajes) y determinar qué grupos demográficos representan el mayor valor comercial para la compañía.

## 📁 Datasets Utilizados
Los datos están distribuidos en tres archivos CSV ubicados en la carpeta `datasets/`:
* `plans.csv`: Información sobre las tarifas y condiciones de los planes.
* `users_latam.csv`: Perfiles demográficos de los clientes (edad, ciudad, fecha de registro).
* `usage.csv`: Registros de consumo mensual (cantidad de llamadas, minutos y mensajes).

## 🛠️ Etapas del Análisis Realizadas
1. **Exploración Inicial:** Carga de datos y revisión de estructuras.
2. **Limpieza de Datos:** Tratamiento de valores nulos (ej. 11.7% en ciudad), corrección de datos centinela (edades en -999) y filtrado de fechas ilógicas de registro.
3. **Fusión de Datos:** Consolidación de los tres datasets en un único perfil de usuario (`user_profile`).
4. **Análisis de Outliers:** Identificación de valores atípicos en consumos mediante el método de Rango Intercuartílico (IQR) y boxplots.
5. **Segmentación de Clientes:** Clasificación de usuarios por nivel de uso ('Bajo', 'Medio', 'Alto') y por grupo de edad ('Joven', 'Adulto', 'Adulto Mayor').
6. **Visualización y Conclusiones:** Gráficos de distribución (Seaborn) y recomendaciones comerciales basadas en la rentabilidad de los segmentos.

## 🚀 Cómo Ejecutar el Notebook y Guía de Reproducción
Para revisar o ejecutar este proyecto, sigue estos pasos:

1. **Entorno recomendado:** Google Colab o Jupyter Notebook local.
2. **Estructura de carpetas:** Asegúrate de que los tres archivos CSV estén guardados dentro de una carpeta llamada `datasets/` ubicada en el mismo nivel/directorio que el notebook.
3. **Ejecución:** Abre el archivo `notebooks/S7_Version_Estudiante_Project_ConnectaTel.ipynb`.
4. Ejecuta las celdas de código en orden secuencial (de arriba a abajo) para cargar las librerías (`pandas`, `numpy`, `seaborn`, `matplotlib`), procesar los datos y generar los gráficos correctamente.
