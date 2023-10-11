README

Realizar un análisis sobre el número de fallecidos y sobrevivientes generados por accidentes aéreos desde principios del siglo 19 es de suma importancia por varias razones, tales como: seguridad y mejora continua, evaluación de protocolos de emergencia, capacitación y entrenamiento, entre otros.

Estudiar los accidentes aéreos pasados proporciona información valiosa para mejorar la seguridad en la industria de la aviación. Analizar el número de fallecidos ayuda a identificar áreas de mejora y a implementar políticas y procedimientos que reduzcan los riesgos. Comprender las causas subyacentes de los accidentes puede llevar a la implementación de medidas preventivas y correctivas.

En cuanto a la diferenciación entre fallecidos de tripulación, pasajeros y sobrevivientes, esto es importante para comprender la distribución de los riesgos y para diseñar políticas y procedimientos que maximicen la seguridad de todos los implicados.

El proyecto se compone de varios componentes los cuales sirvieron para procesar y analizar la información:

- Archivo AccidentesAviones.csv: Archivo en el que se encuentra toda la información para el procesamiento y análisis del proyecto.
- Diccionario de datos: Diccionario creado para el proyecto.
- Accidentesaereos-2.ipynb: Archivo en donde se desarrolló el EDA con análisis inicial estadístico.
- Accidentesaereos-3.ipynb: Archivo en donde se desarrolló el segundo análisis inicial estadístico y se ejecuta el nuevo modelo logarítmico que se ajusta mejor al tipo de datos y se realizan análisis gráficos.
- Archivo AccidentesAvionesa.csv: Archivo final con el ajuste de los datos y el ajuste logarítmico de la información.

PROCESO GENERAL

1. Se revisaron los componentes del dataset para determinar la calidad y tipo de información
1. Se reviso la información para tratar de determinar un diccionario de las columnas y datos del dataset
1. Se revisa e identificaron las columnas que permitirán resolver el problema u objetivo planteado
1. Se revisa información faltante, errores en la información y que columnas tienen menos errores
1. Se hicieron los ajustes necesarios para normalizar los datos y realizar el análisis inicial estadístico y determinar nivel de confianza
1. Se proceso la información con el modelo logarítmico, el cual mostro un mejor ajuste a los datos para su posterior análisis. Este modelo permitió capturar relaciones más complejas entre variables y adaptarse a situaciones en las que los cambios en una variable no se traducen en cambios lineales, también ayudo a estabilizar la varianza entre los datos y sino que también permitió una reducción de la influencia de valores atípicos
1. Posteriormente se ejecutaron códigos para obtener estadísticas descriptivas y análisis de outliers
1. Se ejecutaron códigos para verificar tendencias en archivo .ipynb que ejecutan gráficas y  adicionalmente se ejecutan códigos para verificar correlación entre variables


PROCESO POWERBI

Se carga información a Powerbi y se hace la verificación de la información ingresada.

Se generan las medidas y columnas necesarias para generar y ver la información de total de vuelos accidentados, total de pasajeros, total fallecidos, entre otros y que sirven para dar forma a la página inicial general y para dar contexto sobre la información obtenida y a analizar tanto para este análisis como para los próximos correspondientes a los Kpis definidos.

ANALISIS GENERAL

Se desarrollan diferentes observaciones en los cuales se establece que tipo de información esta relacionada con los indicadores propuestos y que entreguen el contexto necesario para su posterior análisis. Teniendo en cuenta se ejecutan los siguientes querys:

Cantidad de viajes accidentados por año y total de la muestra, el cual nos muestra como están divididos los viajes accidentados año tras año en donde se observa al inicio una accidentalidad media hasta el año 1943, pero que a partir de 1945 se incrementan y se estabilizan a partir de 1948 hasta el año 2000, fecha en la que se reducen la cantidad de accidentes progresivamente en los siguientes 20 años. Aquí es necesario decir que no es posible saber la causa de esa disminución ya que no se tiene información si la cantidad de vuelos se mantuvo, decreció o aumento a través del tiempo; por tal razón el análisis que se hace es de tipo de descriptivo.

Se observa que el promedio de fallecidos es de 23,06 y de 9,13 de los sobrevivientes

En la grafica de pasajeros vs total fallecidos se logra ver una correlación directa entre la cantidad de fallecidos y el total de ocupantes, situación que demuestra una correlación directa y que indica que, entre más ocupación de las aeronaves, mayor la cantidad de fallecidos al momento de un accidente. Es de resaltar que se observa una paridad de los indicadores a partir de del año 2021 lo cual significaría que, a partir de esa fecha, aunque hay una baja tasa de mortalidad, tampoco hay sobrevivientes.

Por otro lado, se ve que la cantidad de fallecidos corresponde aprox a 107 mil fallecidos y 42 mil sobrevivientes que corresponde a un 71.64% y a un 28,36% respectivamente.

Finalmente, en un análisis de temporada, se hace un análisis por trimestre, que muestra al tercer trimestre como el periodo en el se transporta más personas y así mismo se evidencia más personas fallecidas.

ANÁLISIS PRIMER KPI

El total de tripulantes fallecidos es de 16,862, con un promedio de 3.65 de fallecidos por accidente. En la cual para la última década murieron 709 tripulantes y en la segunda murieron 1,345, que equivalen a un 34,52% y un 65,48% respectivamente.

Se genera un reporte de total fallecidos vs tripulación fallecida y no se observa una correlación directa, situación que se puede justificar con el hecho de que la cantidad de tripulantes por lo general siempre es la misma independiente de la cantidad de viajeros.

Se genera otro reporte para ver la cantidad de tripulantes fallecidos a través del tiempo y se observa una constante disminución para los últimos 20 años.

KPI: Disminución de un 10% la tasa de fatalidad de la tripulación en los últimos 10 años, comparado a la década anterior

La medición del kpi nos entrega en 47% de cumplimiento, el cual supera ampliamente el objetivo del 10% trazado inicialmente y que comparando década contra década a partil del 2013 se da un cambio negativo de crecimiento con respecto a la década anterior

ANÁLISIS SEGUNDO KPI

Se calculo la cantidad total de sobrevivientes que corresponde a 42,226. También se calcularon la cantidad de sobrevivientes para los dos últimos lustros y obtuvo que para el primer lustro fue de 503 sobrevivientes y para el segundo de 1,302 sobrevivientes, situación que en parte puede ser debido a la disminución en la cantidad de accidentes reportados. 

Para los últimos 5 años la cantidad porcentual de fallecidos es del 64,43% y para sobrevivientes del 35,57%

En el reporte de sobrevivientes a través del tiempo, se ve una distribución no controlada y que esta muy relacionada a la cantidad de fallecidos y total de pasajeros, mostrando picos tanto hacia arriba como hacia abajo a lo largo de los años sin ningún tipo de tendencia claro.

En el grafico de sobrevivientes vs fallecidos para los últimos 5 años, se evidencia que a partir del año 2020 la cantidad de sobrevivientes tiende a cero y se acerca a la cantidad de fallecidos.

En el análisis por trimestre, se observo que el trimestre con mayor participación de sobrevivientes es el 4 y el de menor es el 2, sin embargo, se observa una participación muy pareja entre trimestres.

Por último en el análisis por mes, se observa que el mes en el que mas participa en la cantidad de sobrevivientes es marzo y el menor es septiembre, sin encontrar una relación clara mes vs cantidad de sobrevivientes

KPI: Aumento de 7,01 a 8,41 (20%) en el promedio de sobrevivientes, con respecto a los últimos 5 años.

El kpi muestra que no se cumplió con la meta propuesta inicial, que pretendía incrementar en un 20% la cantidad de sobrevivientes a 8,45. Es de resaltar que este indicador se puede estar viendo afectado para la cantidad de accidentes presentados y por la cantidad de ocupantes,

Es de resaltar que así como el indicador de fallecidos el indicador de sobrevivientes es un indicador clave en el análisis, debido a que una disminución en la cantidad de fallecimientos no representa necesariamente un aumento en los sobrevivientes y que requiere de diferentes estrategias para su mejora.


















