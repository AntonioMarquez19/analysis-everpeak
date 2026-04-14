Análisis de Datos para ConnectaTel 📊

Objetivo del Proyecto
El propósito de este proyecto es actuar como Analista de Datos para ConnectaTel.
El análisis busca transformar datos brutos de consumo y perfiles de clientes en insights estratégicos que permitan a la dirección:
- Comprender la demografía de su base de usuarios.
- Identificar patrones de consumo (mensajes, datos y minutos).
- Segmentar a los clientes para personalizar la oferta comercial y reducir la tasa de deserción.

Datasets Utilizados
Para este análisis se utilizaron conjuntos de datos que integran la siguiente información:
-Usuarios: ID único, nombre, apellido, edad, ciudad y fecha de registro.
-Consumo: Registros detallados de la cantidad de mensajes enviados, megabytes utilizados y minutos consumidos mensualmente.
-Planes: Información sobre las tarifas y beneficios de los planes actuales, Básico y Premium.

Etapas del Análisis
El proyecto se desarrolló siguiendo un flujo de trabajo de ciencia de datos:

1.  Exploración y Limpieza de Datos:
    - Tratamiento de valores ausentes NaN en columnas como ciudad y fechas de cancelación.
    - Estandarización de formatos de fecha y tipos de datos numéricos.
    - Detección y manejo de registros inconsistentes.

2.  Ingeniería de Características:
    -Segmentación por Edad: Creación de categorías Joven, Adulto, Adulto Mayo, para entender el ciclo de vida del cliente.
    -Segmentación por Uso: Clasificación de usuarios según su nivel de actividad Bajo, Medio, Alto uso.

3.  Análisis Estadístico y Visualización:
    -Generación de histogramas y gráficas de barras para visualizar la distribución de los segmentos identificados.
    -Identificación de outliers.

4.  Conclusiones e Insights Ejecutivos:
    -Interpretación de los resultados para la toma de decisiones basada en datos.

Cómo ejecutar el Notebook

Requisitos previos
-Librerías de Python necesarias: `pandas`, `matplotlib`, `seaborn`.

Instrucciones
1.  Cargar el archivo: Sube el notebook `.ipynb` a tu entorno de preferencia Github.
2.  Subir los Datos: Asegúrate de cargar los archivos CSV correspondientes en el directorio de trabajo para que el código pueda leerlos.
3.  Ejecución: Ejecuta las celdas de forma secuencial para asegurar que las variables y funciones se definan correctamente.

Guía de Reproducción
Para replicar los hallazgos de este reporte:
1.  Aplica las funciones de segmentación `segmentar_edad` y `segmentar_uso` sobre el DataFrame de perfiles de usuario.
2.  Utiliza el método `.value_counts()` para verificar la consistencia de los grupos creados.
3.  Genera las visualizaciones utilizando `plt.show()` para confirmar que la distribución coincida con el análisis ejecutivo presentado.
