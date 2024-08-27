<h1 align='center'>
 <b>PROYECTO INDIVIDUAL Nº2</b>
</h1>

# <h1 align="center">**`Telecomunicaciones`**</h1>

<p align='center'>
<img src="./pictures/Banner.jpg" >
<p>

## Descripción
En este proyecto, se lleva a cabo un análisis exhaustivo de los datos de distribución de Internet en Argentina, con el objetivo de identificar patrones, tendencias y áreas de mejora en la provisión de servicios de conectividad. Utilizando datos detallados sobre la velocidad de conexión en diferentes provincias, la variabilidad en el acceso a Internet y las posibles disparidades regionales.

El proyecto se enfoca en desarrollar estrategias basadas en datos para maximizar los ingresos El objetivo final es proporcionar recomendaciones prácticas para mejorar el rendimiento financiero de los proveedores de Internet y promover una conectividad más eficiente en todo el país.

## Tabla de contenido
1. [Estructura del Proyecto](#estructura-del-proyecto)
2. [EDA](#EDA)
3. [KPI](#KPI)
4. [Fuente de Datos](#fuente-de-datos)



## Estructura del Proyecto
- `data/`: Contiene los archivos de datos utilizados en el proyecto.
- `notebooks/`: Incluye los notebooks de Jupyter con el EDA.
- `pictures/`: Contiene las imagenes utilizadas en este README.md
- `report/`: Contiene el Dashboard.
- `README.md`: Archivo de documentación del proyecto.

## EDA

- Objetivos
El primer paso en el EDA fue examinar la relación entre los ingresos y otros valores disponibles en el dataset, con un enfoque particular en la velocidad de descarga de Internet. La hipótesis inicial era que los ingresos podrían estar asociados con diferentes métricas de rendimiento del servicio.

- Analisis de correlación
Para entender la relación entre los ingresos y otras variables, se realizaron análisis de correlación. Se evaluaron las correlaciones entre los ingresos y diversas métricas, incluyendo:

Velocidad Media de Descarga: Se pudo notar una alta correlación entre la velocidad de descarga y los ingresos, como demuestra el siguiente grafico:

![Ingresos y Velocidad](./pictures/Ingresos%20y%20Velocidad%20Media%20Descargada.png)

- Analisis de diferentes tecnologias y como afectan a la velocidad media

Se llevó a cabo una evaluación detallada para determinar cuál de estas tecnologías ofrece los mayores beneficios en términos de velocidad para los clientes. Este análisis se centró en el caso específico de la provincia de San Luis, que ha experimentado cambios significativos en su velocidad de Internet en los últimos años.

Los datos mostraron que la velocidad de Internet en San Luis aumentó significativamente con la implementación de fibra óptica. Las tecnologías anteriores, como ADSL y cable coaxial, ofrecían velocidades de descarga más bajas en comparación con la fibra óptica.  Antes de la expansión de fibra óptica, San Luis tenía una velocidad de conexión relativamente baja. Sin embargo, tras la implementación masiva de fibra óptica, se observó un aumento notable en la velocidad de descarga.

Se puede apreciar la correlación entre la implementacion de fibra optica y la velocidad media en el siguiente grafico:
![Velocidad y Fibra Optica](./pictures/Velocidad%20de%20Bajada%20y%20Fibra%20%C3%93ptica%20en%20San%20Luis.png)
*Es importante notar que aunque la relación es directa, hay una demora de unos años entre la implementación de fibra óptica y el aumento esperado en la velocidad*

Esto nos lleva a concluir que la mejor manera de aumentar la velocidad de bajada de los clientes, y por extención maximisar los ingresos, es implementando mas fibra óptica.

## KPI
Se realizaron 3 KPIs en el Dashboard:

1. $`KPI Fibra Optica = ((Cantidad de Fibra Óptica actual - Cantidad de Fibra Óptica anterior) / Cantidad de Fibra Óptica anterior) * 100`$

- Esto nos permite ver que instalación hubo de Fibra Optica con respecto al trimestre anterior
Demostrado en el EDA del projecto, se encontro una relación directa entre la velocidad de baja y la instalación de Fibra Optica, por lo que se intenta maximizar.

Se toma como objetivo un 2% para este KPI, el cual es alcanzado.

2. $`KPI Velocidad = ((Velocidad de Bajada actual - Velocidad de Bajada anterior) / Velocidad de Bajada anterior) * 100`$

- Esto nos permite ver que tanto aumento la velocidad promedio de descarga en el ultimo trimestre
Demostrado en el EDA del projecto, se encontro una relación directa entre la velocidad de baja y los ingresos, por lo que se intenta maximizar.

Se toma como objetivo un 4% para este KPI, ya que la velocidad aumenta 2x la instalaci{on de nueva Fibra Optica.
Este KPI no alcanza el valor objetivo, ya que hay una demora de tiempo entre implementar Nueva Fibra Óptica y el aumento de velocidad esperado.
En el caso de continuar con la estrategia sugerida, este KPI subiria al valor objetivo.

3. $`KPI Pen = ((Penetración por Hogar actual - Penetración por Hogar anterior) / Penetración por Hogar anterior) * 100`$

Se toma como objetivo un 2% para este KPI.
Este KPI no alcanza el valor objetivo, por lo que se recomienda expandir la red de internet a mas hogares.

## **Fuente de datos**
- [Datasets](https://indicadores.enacom.gob.ar/datos-abiertos)
- [Diccionario de datos](https://docs.google.com/document/d/1BYW0vT_DNIjjKM9v4hNg5KmqjRNOc7OBB1jCXc80gnI/edit#heading=h.hjukififf3ol)
 
## Autores:
Este proyecto fue realizado por: Thomas Bracamonte.
<br/>
