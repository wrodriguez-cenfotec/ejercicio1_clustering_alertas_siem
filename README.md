# Práctica: Agrupamiento de alertas de un SIEM con K-means
Libreta de práctica para los estudiantes del curso CIB-209, Temas Especiales en Seguridad de Datos y Sistemas
## Aviso sobre los datos
Las 600 alertas del archivo alertas_siem.csv son sintéticas, generadas para este ejercicio con el script generar_datos.py. No corresponden a alertas reales de ningún SIEM ni de ninguna organización. La columna perfil_real existe solo para calificar el resultado al final del ejercicio, en un caso real esa columna no existiría y el analista tendría que validar los grupos con otros medios.
## Cómo ejecutar en Binder
1. Abrir el repositorio en Binder con el botón de abajo:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/wrodriguez-cenfotec/ejercicio1_clustering_alertas_siem/HEAD?urlpath=%2Fdoc%2Ftree%2Fejercicio1_clustering_alertas_siem.ipynb)
2. La primera carga tarda unos minutos mientras se construye el entorno. Tener paciencia.
3. Ejecutar las celdas en orden, de arriba hacia abajo.
4. La sesión de Binder es temporal. Antes de cerrar, descargar la libreta o guardar capturas de los resultados.
## Qué hace la libreta
- Carga y explora las 600 alertas simuladas del SIEM.
- Escala las variables y aplica el método del codo y el coeficiente de silueta para elegir el número de grupos.
- Entrena K-means y agrupa las alertas en familias.
- Interpreta cada grupo comparando sus variables promedio y valida el resultado contra el perfil real conocido.
- Visualiza los grupos en un gráfico de dispersión.
- scikit-learn, agrupamiento. https://scikit-learn.org/stable/modules/clustering.html
- scikit-learn, KMeans. https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
- scikit-learn, coeficiente de silueta. https://scikit-learn.org/stable/modules/clustering.html#silhouette-coefficient
- Binder. https://mybinder.org/
