
# Conclusión

El análisis realizado permitió detectar que el dataset original presentaba distintos problemas de calidad, entre ellos valores nulos, fechas y horas inválidas, formatos inconsistentes y valores atípicos. Por este motivo fue necesario realizar un proceso previo de limpieza y normalización antes de utilizar la información para el análisis de infracciones.

Luego del procesamiento, se observó que las infracciones se distribuyen de manera relativamente pareja entre los distintos turnos, aunque el turno tarde presentó la mayor cantidad. En cuanto a los muelles, MUELLE-B y MUELLE-D fueron los que registraron mayor cantidad de infracciones. Por otro lado, el tipo de carga más frecuente entre los registros infractores fue TRIGO, representando aproximadamente el 15.44% del total.

También se detectó que el 4.92% de las infracciones provenían de registros con fechas inválidas y el 48.77% contenían alguna hora inválida. Estos resultados muestran que incorporar los datos directamente al nuevo sistema sin realizar una limpieza previa podría generar análisis incorrectos, afectar el cálculo de tiempos de estadía y producir conclusiones poco confiables.

Como propuesta de mejora, sería conveniente implementar validaciones automáticas al momento de registrar los datos en el puerto. Por ejemplo, controlar que las fechas y horas tengan un formato válido, evitar campos obligatorios vacíos y validar automáticamente la velocidad registrada respecto del límite del muelle. Esto permitiría mejorar la calidad de los datos desde su origen y reducir la necesidad de correcciones posteriores.
