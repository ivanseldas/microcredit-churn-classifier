![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Ironhack Payments: Un Análisis de Cohortes (Proyecto 1)

## Introducción y Visión General del Proyecto

El objetivo principal de este proyecto fue realizar un análisis de cohortes basado en datos proporcionados por IronHack Payment, una empresa de servicios financieros "ofreciendo soluciones innovadoras de adelanto de efectivo desde su creación en 2020".

Para ello hemos hecho uso de Python y sus respectivas herramientas de análisis, como Pandas y Plotly.

Creamos cohortes basadas en el mes de la primera transacción de cada cliente, y las analizamos para obtener perspectivas útiles e interesantes sobre el comportamiento de los clientes y su impacto en la empresa.

### Limpieza y Organización de Datos

# El código y los metodos utilizados para esta etapa se pueden encontrar en el documento Exploratory_Analysis.ipynb.

Para empezar, utilizamos diversos métodos para limpiar y manejar los datos, y llevar a cabo un análisis exploratorio inicial de los datos.

Comenzamos cargando los dos datasets ‘cash’ y ‘fees’  desde archivos CSV y creamos dos DataFrames con la función pd.read_csv(). Luego utilizamos funciones como head, columns, size y describe para aprender más sobre los datos y devolver unas estadísticas como el sum, y los valores máximos y mínimos de columnas como ‘amount.

Luego miramos los diferentes data types de los dos DataFrames. Ya que la mayoría eran del tipo genérico ‘object’, convertimos varias columnas en el data type ‘datetime’, y otras en el tipo ‘category’. Esto importa ventajas como eficiencia y reducción del uso de memoria.

Después experimentamos con crear subsets de columnas que no necesitamos usar en el momento. Esto lo hicimos fácilmente por “commenting out” columnas específicas.

Hicimos uso del método duplicated() para ver si hay filas or user_ids duplicados en los DataFrames. Usamos la función unique() para mirar valores únicos, y count() para contar otros, como las ocurrencias de cada user_id, para entender la cantidad de transacciones repetidas.

Buscamos datos faltantes usando la función isnull(). Descubrimos que la cantidad de user_ids faltantes (2103) era casi igual que el número de deleted_account_ids presentes (2104). De esta manera, pudimos determinar que los user_ids faltantes representan clientes que han eliminado sus cuentas, y ahora son representados por deleted_account_ids.

Para entender mejor la relación entre los dos DataFrames ‘cash’ y ‘fees’, buscamos columnas compartidas entre ambos ('updated_at', 'id', 'status', 'created_at') y buscamos valores duplicados entre ellos.

Intentamos unir los DataFrames con la función merge, probando left merge y right merge, pero al final esta parte de conectar y encontrar correlaciones entre los dos DataFrames fue una de las partes que más nos costó conseguir y entender bien. Aun así, consideramos que llegamos a lograr un buen análisis de cohortes en los próximos pasos del proyecto. 


### Análisis Principal

# El código, los metodos y los gráficos reveladores relacionados con esta etapa del proyecto se pueden encontrar en el documento Main.ipynb.

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

Nuestras conclusiones se resumen detallademente in el documento Conclusiones, y a través de nuestra presentación PowerPoint. Esperamos que te resulten esclarecedores y interesantes, y te agradecemos por leer.
