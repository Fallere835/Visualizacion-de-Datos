**PROYECTO DE VISUALIZACION DE DATOS: ANALISIS DE SATURACION HOSPITALARIA Y CONTAMINACION ATMOSFERICA**

**OBJETIVO DEL PROYECTO**
Este repositorio contiene el desarrollo de un Dashboard interactivo construido con la libreria Dash de Python. El objetivo principal es explorar y comunicar la relacion existente entre los niveles de contaminacion atmosferica por material particulado (PM 2.5), el aumento de las atenciones de urgencia por causas respiratorias y la ocupacion de camas criticas en la zona sur de Chile (Osorno, Chiguayante, Concepcion, Temuco y Valdivia).

**DESCRIPCION DE DIRECTORIOS**

_Atenciones_Respiratorias_
Contiene los conjuntos de datos en formato CSV con el registro de atenciones de urgencia por causas respiratorias entre los años 2020 y 2025. Los archivos han sido procesados para unificar los cambios de nomenclatura realizados por el Departamento de Estadisticas e Informacion de Salud (DEIS).

_Datos_PM_
Contiene los registros historicos de contaminacion PM 2.5 para las ciudades de Osorno, Chiguayante, Concepcion, Temuco y Valdivia. Estos datos permiten sincronizar temporalmente los peaks de contaminacion con la carga hospitalaria.

_Indicadores de Salud REM20_
Contiene el archivo Indicadores_REM20.csv, el cual detalla la disponibilidad, ocupacion y saturacion de camas criticas (UCI/UTI) por establecimiento de salud y area funcional.

**DESCRIPCION DE NOTEBOOKS DEL PROYECTO**

_Visualizacion.ipynb_
Es el componente central del repositorio. Contiene el proceso de extraccion, transformacion y carga de datos (ETL) y la implementacion del Dashboard. El panel incluye 7 visualizaciones clave: mapa de focos de contaminacion, composicion de causas, evolucion semanal de smog vs urgencias, impacto segun estado del aire, matriz de correlacion, histograma de saturacion y capacidad operativa de camas.

_Urgencias_Hospitalarias.ipynb_
Este notebook documenta el proceso inicial de preparacion, limpieza y filtrado de los datos brutos de atenciones de urgencia hospitalaria. Se encarga de procesar los registros originales y exportar los conjuntos de datos limpios y segmentados por año (desde el 2020 hasta el 2025) en formato CSV hacia el directorio Atenciones_Respiratorias. Estos archivos depurados son los que posteriormente alimentan el dashboard principal.
