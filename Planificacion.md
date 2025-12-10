 Importar las librerías
 Cargar, visualizar y sacar los parámetos básicos de nuestros csv clientes y contratos
 Realizar Analisis Exploratorio de los datos 
    - Nulos : 
        - csv (clientes) - eliminamos los 3 nulos que hay de los 1003 registros dado que no aportan valor. 3 filas al final   del dataset
        - csv (contratos) - rellenamos los 124 nulos de id_contrato con la "secuencia numérica" dado que au que suponen un 1,54 % conviene no eliminarlos para no perder información
    - Duplicados
    - Limpiamos columnas( quitamos los tiítulos de variable nombre csv clientes, cambiamos el tipo de dato de la fecha)
 Objetivos:
    - Detectar los 5 productos que más aportan en términos de uso( contratos por productos, a mas contrato mas demanda).
    - Detectar los productos que generan más ingresos. No tenemos columna de tarifas por lo que estimamos precio fijando un precio unitario (50 por ud uso).
    - No observamos productos sin uso pero si algunos que tienen poca tirada como 31,33,34 y 35. Para ello, hemos fijado el umbral por debajo de 15.
    - Analizar combinaciones frecuentes de contratación para ver los productos que contratan los clientes juntos por ejemplo.
    - Observamos la evolucion temporal catálogo por mes tanto de cliente como contratos. Respecto al catálogo de productos se observan en el gráfico pocas variaciones entre los años 2022 y 2024. Lo que nos da una idea de que el negocio no ha variado el producto. Respecto a los clientes, se observan fluctuaciones mes a mes en los distintos años, con picos y caidad,  lo que nos permite pensar que la demanda dependerá de factores externos como ofertas, campañas..etc