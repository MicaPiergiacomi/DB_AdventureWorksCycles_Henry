# Visualizando el Rendimiento Adventure Works Cycles

Adventure Works Cycles (AWC) es una empresa multinacional líder en la fabricación y distribución de bicicletas, piezas y accesorios. 

El presente informe tiene como objetivo proporcionar una visión integral y detallada del rendimiento de ventas de AWC mediante el uso de la plataforma Power BI. A través de análisis exhaustivos y visualizaciones interactivas, este informe permitirá a los usuarios finales comprender mejor los factores que influyen en las ventas, los costos asociados y la rentabilidad general de la empresa. Además, servirá como una herramienta invaluable para la toma de decisiones estratégicas, al proporcionar información clave y perspicaz para identificar áreas de mejora y oportunidades de crecimiento.

### Objetivos:

• **Mejora de la calidad de los datos**: A través de procesos de limpieza y validación de datos efectivos con Power Query;

• **Modelado de datos relacional**: Se desarrolla un modelo de datos robusto y relacional que refleja las complejas interacciones entre diferentes aspectos del negocio, permitiendo un análisis integrado y coherente.

• **Cálculo de métricas clave con DAX**: Se utilizan expresiones de análisis de datos (DAX) para calcular métricas clave relacionadas con las ventas, los costos y la rentabilidad, proporcionando una comprensión más profunda del rendimiento empresarial.

• **Diseño de informes informativos y visuales**: Se diseñan informes visuales atractivos y fáciles de entender, que destacan los KPIs más relevantes y facilitan la identificación de tendencias y patrones significativos.



## Desarrollo del proyecto

### Avance 1: Conexión y Limpieza de Datos

-Se restauró en SQL la base ‘AdventureWorksDW2019’.
  
-En Power BI se conectó de la base restaurada las tablas: ‘DimProduct’, ‘DimProductcategory’. ‘DimProductSubcategory’, ‘DimDate’, ‘DimPromotion’, ‘DimSalesTerritory’, ‘DimGeography’ y ‘FactInternetSales’. Se conectó también la tabla ‘DimCustomer’.
  
-Se verificó que los encabezados de todas las tablas estén bien.
  
-Acciones: Eliminación de filas en blanco; Eliminación de columnas vacías; Unificación de columnas; Combinacion de tablas; Reemplazo los valores ‘null’ en las columnas.


### Avance 2: El enfoque principal esta en preparar los datos para futuros analisis.

-En este segundo avance del proyecto, se centró en el diseño tanto del modelo relacional eficiente en Power BI como en la creación de un mockup del informe que guiará el producto final. Para abordar el problema de negocio planteado, se buscó desarrollar un reporte que ofreciera una visión clara y detallada de los ingresos, costos, rentabilidad y otros indicadores clave a nivel de la compañía, con un enfoque especial en el mercado de Estados Unidos.

-El reporte diseñado debe responder a una serie de preguntas clave, incluyendo el total de ingresos del período actual y anterior, cantidad vendida, utilidad bruta y neta, costo de los bienes vendidos, distribución geográfica de clientes, distribución mensual de ingresos, COGS y utilidad, utilidad por segmento y subcategoría de producto, entre otros.


### Avance 3: Generar las medidas y columnas calculadas.

-Utilización de DAX para crear medidas y columnas calculadas que analicen los ingresos, costos y otros indicadores claves. 


### Avance 4: Creación de tablero y documentacion del proyecto BI.

-Se creó el reporte final en Power BI, centrado en los ingresos, costos y rentabilidad, tanto a nivel global como en el mercado de Estados Unidos.
  
-Con la herramienta Figma realicé los fondos de lienzo con las medidas personalizadas Alto: 1080, Ancho: 1920.
  
-Utilice las visualizaciones del mockup como guía para crear las visualizaciones en Power BI.
  
-Luego generé Parámetros de Campo desde la pestaña "Modelo" y creé un nuevo parámetro de campos llamado "Indicadores". Agregue las medidas requeridas (Ingresos, Utilidad Neta, Utilidad Bruta, COGS, "% Margen Neto, "% Margen Bruta, Costo de Envío"). Luego lo agregué como un segmentador visual y lo usé para filtrar la información en los mapas que muestran los clientes por país.
  
-Se creó un grupo de cálculo llamado "Variacion_Tiempo" que agrupe las medidas relacionadas con el período actual, el período anterior, la variación y la variación porcentual. 



## PORTADA DASHBOARD
![0](https://github.com/MicaPiergiacomi/Visualizacion-Rendimiento-Adventure-Works-Cycles/assets/168442686/3e04750f-d7c0-4693-bc01-6e5634c03741)

## ANALISIS DE MERCADO A NIVEL GLOBAL
![1](https://github.com/MicaPiergiacomi/Visualizacion-Rendimiento-Adventure-Works-Cycles/assets/168442686/7c35c9e8-3181-45b7-9815-188b54405b85)

Encabezado:
Logotipo de Adventure Works Cycles: Establece la identidad corporativa.

1. Resumen Financiero: KPI 
INGRESOS: $9,39 millones.
UNIDADES VENDIDAS: 21,344 unidades.
COGS (Costo de los bienes vendidos): $5,49 millones.
UTILIDAD BRUTA: $3,90 millones.
UTILIDAD NETA: $2,92 millones.

2. Mapa - Cantidad de Clientes por Estado:
Visualiza la distribución geográfica de los clientes en Estados Unidos, ofreciendo una vista rápida de los mercados más fuertes.

3. Tabla de Ingresos Anuales:
Detalle de ingresos y COGS por año (2010-2014).
Proporciona un historial de rendimiento financiero año tras año.

4. Gráficos de Tendencia:
Ingresos Acumulados Anuales: Muestra el crecimiento de ingresos a lo largo del año.
COGS y Utilidad Bruta por Ciudad: Analiza costos y utilidades a nivel de ciudad, permitiendo identificar regiones más o menos rentables.

5. Gráfico de Barras - Ingresos por Subcategoría:
Desglose de ingresos por producto, destacando las categorías principales como Road Bikes y Mountain Bikes.


## ANALISIS DE MERCADO ESTADOS UNIDOS
![2](https://github.com/MicaPiergiacomi/Visualizacion-Rendimiento-Adventure-Works-Cycles/assets/168442686/b93efd31-d10d-41ca-a649-06e48036b766)

Encabezado:
Similar al segundo tablero, pero con la opción de "ESTADOS UNIDOS" activada.

1. Resumen Financiero Ampliado:  KPI
INGRESOS: $29,36 millones.
UNIDADES VENDIDAS: 60 mil unidades.
COGS: $17,28 millones.
UTILIDAD BRUTA: $12,08 millones.
UTILIDAD NETA: $9,00 millones.

2. Mapa Global - Cantidad de Clientes por País:
Expande la vista al nivel mundial, mostrando la distribución global de clientes.

3. Gráfico de Barras y Ratios:	
Utilidad Bruta y Neta por Subcategoría: Compara la rentabilidad de diferentes líneas de productos.
Ratio Costo Operacional vs LY (Last Year): Ofrece una comparación porcentual del costo operacional actual frente al año anterior.

4. Gráfico de Tendencia Ampliado:
Ingresos, COGS y Utilidad Bruta por Mes y Año: Proporciona una visión detallada de las tendencias mensuales y anuales, permitiendo análisis de estacionalidad y crecimiento.




## Insights y Líneas Futuras de Análisis

El análisis exhaustivo del rendimiento de ventas de Adventure Works Cycles (AWC) ha proporcionado insights valiosos que contribuyen directamente a la toma de decisiones estratégicas en la empresa:

- Crecimiento Sostenido de Ingresos: Se observa un aumento constante en los ingresos anuales, lo cual indica un crecimiento sostenible de la empresa en el tiempo, pese a las fluctuaciones del mercado.

- Análisis Geográfico de Clientes: La visualización geográfica muestra que ciertas regiones en Estados Unidos y a nivel global tienen una densidad de clientes significativamente más alta, lo cual podría influir en las decisiones de marketing y expansión.

- Desempeño de Subcategorías de Productos: Las bicicletas de ruta y montaña generan la mayor parte de los ingresos, destacando su popularidad y potencial para inversiones futuras en innovación y marketing.

- Estabilidad en Costos de Operación: Aunque los COGS han permanecido estables, es crucial continuar monitoreándolos para asegurar que no disminuya la rentabilidad con el tiempo.

- Eficiencia Operacional: El ratio de costo operacional frente al año anterior muestra un manejo eficiente, aunque con espacio para mejorar en la reducción de costos y optimización de procesos.

Líneas Futuras de Análisis: Para continuar mejorando la comprensión del rendimiento de AWC y apoyar decisiones aún más informadas, se recomiendan las siguientes líneas de análisis:

- Análisis de Rentabilidad por Producto: Profundizar en el análisis de rentabilidad a nivel de SKU para identificar productos no rentables o que están sub-rendimiento. Esto podría incluir un análisis de la contribución marginal para ajustar la estrategia de precios o promociones.

- Segmentación de Clientes Más Detallada: Utilizar técnicas de análisis predictivo para segmentar a los clientes no solo por ubicación, sino por comportamiento de compra y preferencias. Esto podría ayudar a personalizar las campañas de marketing y aumentar la eficacia de las mismas.

- Análisis de Tendencias Temporales Más Amplio: Examinar las ventas y la rentabilidad a lo largo del tiempo con un enfoque en la estacionalidad y los eventos económicos globales para prever mejor las fluctuaciones en el rendimiento de la empresa.

- Optimización de la Cadena de Suministro: Analizar más a fondo los procesos de la cadena de suministro para identificar oportunidades de reducción de costos, especialmente en las áreas con altos COGS.

- Impacto de Promociones y Descuentos: Evaluar el impacto real de las promociones y descuentos en los ingresos netos y la lealtad del cliente. Esto puede incluir análisis de regresión para entender la elasticidad-precio de los productos.

- Adopción de Tecnologías Emergentes: Considerar la implementación de tecnologías avanzadas como IA y machine learning para mejorar la precisión de los pronósticos de ventas y operaciones, y para personalizar la experiencia del cliente.

Al seguir estas líneas de análisis, AWC no solo mejorará su entendimiento del negocio actual sino que también podrá anticiparse a los cambios del mercado y ajustar su estrategia operativa y comercial de manera proactiva para mantener su posición de liderazgo en la industria.


## Herramientas utilizadas:

- SQL Server
- Power Bi
- Power Query
- DAX
- Figma

