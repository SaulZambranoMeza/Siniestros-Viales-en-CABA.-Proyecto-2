# EDA


##  Introducción.
En el presente proyecto se toma el rol de un Analista de Datos, contratado por la Secretaria de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires (CABA). Se nos ha encomendado desarrollar un proyecto para analizar datos con el propósito de proporcionar información que ayude a las autoridades locales a tomar medidas que reduzcan las muertes por accidentes de tráfico en CABA. Para ello, se dispone de un conjunto de datos sobre homicidios en accidentes de tráfico ocurridos en Buenos Aires entre 2016 y 2021. Se espera la entrega de un informe detallado sobre las actividades realizadas, las metodologías empleadas y las conclusiones principales, además de la presentación de un panel interactivo que facilite la interpretación y el análisis de la información.

 ![image](https://github.com/SaulZambranoMeza/Siniestros-Viales-en-CABA.-Proyecto-2/assets/99093279/07b37645-437d-4091-b84d-3eddc58277eb)


##  Contexto.
Para poder avanzar en el proyecto tenemos que comprender la naturaleza del fenómeno que estamos por analizar y así mismo el lugar geográfico para obtener un análisis más detallado y preciso. Los **accidentes de trafico** son aquellos eventos en donde se involucran diferentes tipos de vehículos, como lo son autos, motocicletas, vehículos de carga, de pasajeros, entre otros. Al igual cabe aclarar que las colisiones pueden ser contra otros vehículos, peatones, objetos fijos, etc. Estos accidentes pueden dar como resultado perdidas materiales, lesiones y en los peores casos, la perdida de una vida.

Dichos accidentes viales y su incremento son una gran preocupación para la secretaria de Transporte del Gobierno de la **Ciudad Autónoma de Buenos Aires (CABA)**, debido a que todos estos incidentes tienen una repercusión en la población de CABA y en su calidad de vida.
Con esto en cuenta podemos ver la importancia y la urgencia de realizar este análisis para poder reducir el numero de accidentes viales y a su vez, la perdida de vidas en dichos accidentes.

##  Datos.
Los datos con los que trabajaremos en este proyecto provienen de dos bases de datos explicadas a continuación.
**Base de datos de Hechos:** Encontramos toda la información relacionada al lugar del accidente, fecha del accidente, las partes involucradas (víctima y acusado), así como el ID para cada incidente, este será una de las columnas más importantes debido a que es un identificador único que nos permite identificar cada accidente sin ningún tipo de confusión.

**Base de datos de víctimas:** Aquí encontraremos referenciado el ID de los hechos el cual también nos servirá como identificador único que cada accidente, aunado a esto también encontramos información relevante como es la edad, sexo, vehículo de la víctima, entre otros elementos que nos ayudarán al análisis.

##  Tecnologías utilizadas.
 ![image](https://github.com/SaulZambranoMeza/Siniestros-Viales-en-CABA.-Proyecto-2/assets/99093279/81b448ad-dab5-4718-9795-a04a7796c019)

Para realizar este proyecto podemos dividir el uso de tecnologías en dos etapas que explicaremos a continuación.
**Etapa 1:** En esta etapa nos enfocamos en la extracción de los datos, su conversión en dataframes, la verificación en la calidad de los mismo y en un análisis exploratorio mediante graficas y poder tener métricas para realizar observaciones. Para esta etapa usamos Python con las siguientes librerías: Pandas, seaborn y matplotlib.

**Etapa 2:** La segunda etapa consistía en poder visualizar los KPIs así como datos relevantes para poder analizar y verificar si se cumplieron los objetivos planteado en este proyecto. Para esta etapa usamos Power bi.

## EDA.
En este apartado realizamos la extracción de los datos, así como verificar la integridad de estos, buscamos valores faltantes, valores duplicados y valores nulos. Así mismo se hizo el análisis de outliers para verificar si esos datos eran solo valores atípicos o realmente eran errores, cabe señalar esto se realizó en ambos dataframes.

Recurrimos al uso de graficas para analizar métricas específicas, las cuales nos podrían arrojar datos interesantes que podríamos tomar en cuenta para análisis futuros. Al igual se realizó la corroboración de los 3 kPIs.


##  análisis.

 ![image](https://github.com/SaulZambranoMeza/Siniestros-Viales-en-CABA.-Proyecto-2/assets/99093279/09a6afb7-fdf2-4728-b1cc-c2ea9ba31fbb)

1.Comenzamos el análisis con una grafica por año de todos los **accidentes que han ocurrido entre 2016 y 2021**, esto con la finalidad de poder tener un panorama general de como han venido variando el numero de accidentes a lo largo de estos años. Después de analizar este grafico podemos decir que el número de accidentes ha variado año con año y no ha sido una reducción gradual, sin embargo, si podemos ver un descenso el número de accidentes si comparamos el año más antiguo (2016) con el año más reciente (2021), aunque este último no ha sido el año con menor número de accidentes entre todos los años analizados. Otro factor para tomar en cuenta es que la reducción en el año 2020, recordemos que ese año se dio la pandemia por COVID-19, así que podríamos sugerir que ese descenso en el numero de accidentes se debe a la pandemia.

2.Así mismo hicimos un análisis por meses para verificar en que meses había una **mayor incidencia en accidentes**, en el que el primer lugar lo tiene el mes de diciembre, con esto podríamos sugerir que el aumento en el numero de accidentes se debe a las celebraciones de fin de año.
**Sugerencia:** Realizar operativos de control de tránsito, así como campañas de prevención en las fechas de diciembre para prevenir accidentes y comenzar a reducir el numero de incidentes en este mes.

3.Analizamos que **vehículos tenían una mayor incidencia** siendo la parte acusada en los incidentes de tránsito, en los cuales tenemos en primer lugar autos y en segundo lugar pasajeros (transporte publico)
Sugerencia: Teniendo esto en cuenta podemos recomendar que aquellas personas que vayan a tramitar una licencia de conducir para un vehículo (auto), realicen pruebas más exhaustivas al igual que charlas para crear una conciencia vial, esto último también se recomienda aplicar en forma de publicidad en los transportes públicos para reducir la segunda causa con mayor recurrencia que son los pasajeros.

4.También realizamos un análisis en el cual queríamos obtener que **vehículo era el que tenía más frecuencia como victima** en accidentes viales, en el cual obtuvimos que el mayor número de víctimas que resultan de accidentes son las motos y los peatones.
**Sugerencias:** Debido a esto recomendamos las siguientes medidas. En cuanto a las motos recomendamos el uso obligatorio de equipo de seguridad para disminuir el número de víctimas. En cuanto al peatón sugerimos realizar un chequeo en las diversas comunas para corroborar si el peatón cuenta con infraestructura (pasos peatonales, puentes de cruce, entre otros) para proteger su integridad.

5.Otra métrica relevante que analizamos fue el rango de edad con más frecuencia de incidencia en accidentes viales, en está métrica en particular pudimos observar que las personas que se encuentran entre 21 y 30 años son las que más incidentes de tránsito.
**Sugerencia:** Requerir pruebas más exhaustivas al momento que las personas en esta edad tramiten su licencia de conducir, además de campañas con charlas de conciencia vial y requerir equipos de seguridad y seguros para sus vehículos. 

##  KPI

![image](https://github.com/SaulZambranoMeza/Siniestros-Viales-en-CABA.-Proyecto-2/assets/99093279/ebc90f70-bd39-4e15-8917-c71376c8935e)

Teniendo en cuenta la información anterior, podemos comenzar con el análisis de los KPI y corroborar si pudimos alcanzar las metas en cada uno de ellos.
**1.Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.**

Definimos a la tasa de homicidios en siniestros viales como el número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000.

Analizando la información obtenida el primer KPI en el cual se busca reducir la tasa de homicidios en siniestros viales en los últimos 6 meses comparados con el mismo semestre del año anterior, podemos concluir que este KPI se consiguió realizar de manera exitosa debido a que en los últimos 6 meses la tasa de homicidios fue de 1.345% comparada con la tasa del semestre anterior, la cual fue de 1.7619, con estos datos podemos calcular que hubo una reducción en la tasa de homicidios de un -23.64%.

**2.Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.**

Definimos a la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año actual - Número de accidentes mortales con víctimas en moto en el año anterior) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100

Con los datos obtenidos podemos evaluar el cumplimiento o no de nuestro KPI, en este caso se buscaba una reducción en los accidentes en donde las victimas fueran motocicletas en un 7%, lamentablemente no se consiguió lograr este KPI, en cambio los accidentes aumentaron. Teniendo en cuenta que en el año 2020 tuvimos un total de 29 accidentes en donde la victima conducía una motocicleta y si lo comparamos con el año 2021 en donde el total de víctimas fue de 46, lamentablemente tuvimos un aumento del 58.62%.

Recomendaciones: Como recomendaciones para poder alcanzar este KPI, sugerimos el que sea obligatorio el uso de equipo de seguridad en todas aquellas personas que manejan motocicletas como lo son los cascos, chamarras de protección entre otras, así como capsulas de conciencia vial a todas las personas que vayan a tramitar sus próximas licencias para conducir, sin importar el tipo de vehículo que manejen.

**3. Reducir en un 5% las muertes en las personas con un rango etario de 21 a 30 años en los últimos dos años.**

En este tercer KPI lo que buscábamos era poder tener una reducción del 5% entre las personas que tuvieran entre 21 y 30 años comparando el 2021 con el 2020, lamentablemente no conseguimos esa disminución del 5%, al contrario. Hubo un aumento del 35.29%
Recomendaciones: Requerir pruebas más exhaustivas al momento que las personas en esta edad tramiten su licencia de conducir, además de campañas con charlas de conciencia vial y requerir equipos de seguridad y seguros para sus vehículos. 


##  Conclusiones.

 ![image](https://github.com/SaulZambranoMeza/Siniestros-Viales-en-CABA.-Proyecto-2/assets/99093279/2dcf3219-860c-45f4-958b-390daae8b70e)

En la Ciudad Autónoma de Buenos Aires (CABA) de 2016 a 2021se han registrado un total de 717 victimas fatales en accidentes de tráfico. De los cuales los cuales el 2018 fue el año con más muertes teniendo el 20.8%, seguido del año 2016 con 20.4% del total de las muertes.

En estos años el mes con mayor incidencia fue el mes de diciembre, tomando en cuenta las celebraciones de fin de año, podríamos sugerir que esa es la causa. Como principales vehículos que causan accidentes, tenemos que el 28% son autos y un 24% son pasajeros (transporte publico).

Así mismo las personas que están más involucradas en accidentes viales son aquellas que están en el rango de edad de 21 a 30 años y por último la comuna en donde suceden más accidentes, es la comuna 1 llegando a casi 90 casos.

**Recomendaciones.**

Uso obligatorio de equipo seguridad para las personas que manejen motocicletas.

Campañas de conciencia vial en el transporte público.

Exámenes más exhaustivos y charlas de conciencia vial a las personas que tramitan su licencia de conducir entre las edades de 21 a 30 años.

Campañas de concientización sobre el respeto al peatón.
