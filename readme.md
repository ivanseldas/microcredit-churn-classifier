![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Ironhack Payments: Un Análisis de Cohortes (Proyecto 1)

## Introducción y Visión General del Proyecto

El objetivo principal de este proyecto fue realizar un análisis de cohortes basado en datos proporcionados por IronHack Payment, una empresa de servicios financieros "ofreciendo soluciones innovadoras de adelanto de efectivo desde su creación en 2020".

Para ello hemos hecho uso de Python y sus respectivas herramientas de análisis, como Pandas y Plotly.

Creamos cohortes basadas en el mes de la primera transacción de cada cliente, y las analizamos para obtener perspectivas útiles e interesantes sobre el comportamiento de los clientes y su impacto en la empresa.

### Limpieza y Organización de Datos

**El código y los metodos utilizados para esta etapa se pueden encontrar en el documento Exploratory_Analysis.ipynb.**

Para empezar, utilizamos diversos métodos para limpiar y manejar los datos, y llevar a cabo un análisis exploratorio inicial de los datos. Esto se puede revisar en el documento antes mencionado, y se resume más detalladamente en el documento Conclusiones.

### Análisis Principal

**El código, los metodos y los gráficos reveladores relacionados con esta etapa del proyecto se pueden encontrar en el documento Main.ipynb.**

Para nuestra analisis principal, creamos cohortes basadas en el mes de la primera transacción de cada cliente, y de ahí nos centramos en obtener y analizar unas métricas especificas para cada cohorte:

1. **Ingresos Totales por Cohorte:**
Calculamos los ingresos generados por cada cohorte. Determinamos datos como qué cohorte lideró en ingresos y usuarios (enero dec2019); qué cohorte reflejó un mayor aumento de usuarios respecto el mes anterior(octubre de 2020); y lo que hemos denominado 'la tendencia estacional', un incremento  constante de usuarios desde primavera 2020, con picos en verano y otoño.

2. **Tasa de Retención por Cohorte:** 
Pudimos calcular la tasa de retención por cada cohorte, y creamos un heatmap para illustrar nuestros hallazgos. Entre ellos, la cohorte con la mayor tasa de retención después del primer mes (mayo de 2020).

3. **Tasa de Incidentes:** 
Estudiamos la tasa de incidentes por cohorte, es decir los distintos estados de las transacciones. Notamos una dismunición de operaciones fallidas después de junio de 2020, y destacamos la cohorte de octubre 2020 como la que tiene mayores ingresos.

4. **RFM (Recency, Frequency, Monetary) :** 
Utilizamos el modelo RFM para segmentar a los clientes en función de sus hábitos. Definimos cuatro 'monetary rankings' de Recency (qué tan recientemente un cliente realizó una compra), Frequencia (con qué frecuencia un cliente realiza una compra), y Monetary Value (cuánto dinera gasta un cliente).

Nuestros hallazgos y gráficos se pueden revisar en detalle en los documentos Exploratory_Analysis.ipynb y Conclusiones.

5. **Correlación Entre las Cantidades Prestadas y el Número de Eventos :** 
Investigamos la correlación entre la cantidad promedia prestada por cada cohorte, y el número promedio de eventos. Descubrimos que cuanto más pide prestado un cliente, más veces pedirá prestado, una relación positiva.

### Conclusiones y Agradecimientos

Nuestras conclusiones se resumen detallademente in el documento Conclusiones, y a través de nuestra presentación de PowerPoint. Esperamos que te resulten esclarecedores y interesantes, y te agradecemos por leer.
