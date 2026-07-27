# CASE ID:

Working Title: Calculo de capacidad de Planta 

Company: Geohidraulica 

Position: Jefe de produccion y mantenimiento

Year: 2022

Priority:
( Achievement | Executive Case | Signature Executive Case )

Status:
( Working Draft | Review Candidate | Approved v1.0 )

Estimated Business Impact:
( Low | Medium | High | Strategic )

---

## 0. CONTEXTO DEL LA EMPRESA

Consorcio Geohidraulica SAC es una empresa de capitales peruanos que se dedica a la fabricacion de bombas de agua para la industria de la mineria subterranea.
Son bombas especiales fabricadas en diferentes potencias desde 15 HP hasta 300 HP , diferentes materiales para aguas acidas o neutras , diferentes configuraciones para caudal o presión, etc.
Estas bombas se usan para evitar que los tuneles de explotacion minera se inunden, porque dentro de los tuneles hay vetas de agua y se necesita un sistema de bombeo en cascada para extraer el agua al exterior del tunel.
El negocio de Geohidraulica es entregar las bombas en alquiler a las unidades mineras, facturar segun los dias de uso y tener siempre bombas para stock para su envio.
Su sistema de fabricacion incluye:
- Diseño de moldes para fundicion de piezas en su area de desarrollo.
- Diseño hidraulico de bombas en su area de desarrollo.
- Mecanizado de piezas fundidas segun diseño propio en taller de mecanizado propio.
- Montaje y prueba de bombas en pozo de pruebas en taller de montaje propio.
- Mantenimiento y rebobinado de motores electricos en taller propio.
- fabricacion de tableros electricos para bombas en taller propio.
Las piezas son fundidas por empresas de fundición bajo las especificaciones de Geohidraulica.
Las Bombas que fallan en operacion son reempalzadas por otra de stock y retornan al taller de Geohidraulica , son reparadas y repuestas a las unidades mineras.
Hay clientes que compran las bombas y a ellos se les dá el servicio de mantenimiento.
Parte de la produccion de bombas nuevas es para ampliar el parque de bombas para stock, otra parte es para venta.
El taller también hace mantenimiento a bombas de otras marcas.
El parque de bombas de alquiler es de aprox 800 bombas que estan distribuidas en diferentes unidades mineras.
Semanalmente llegan al taller apro 65 bombas para mantenimiento las cuales son desmontadas, inspecionadas , se mantienen las piezas buenas , se reemplazan las malas y son montadas nuevamente desde cero como se haría con una bomba nueva.
El objetivo del area a mi cargo (produccion y mantenimiento) era restituir todas las bombas que llegaban a mantenimiento antes que llegue el siguiente lote y producir segun la demanda.

## 1. BUSINESS CONTEXT

###  ¿Qué estaba ocurriendo en la empresa?. ¿Por qué existía ese problema?.

El gerente general necesitaba conocer la capacidad instalada de su planta para poder proyectar un plan de inversiones y expansion.
Sin una capacidad real no se sabía que areas del taller de mecanizado y taller de montaje se necesitaban incrementar y era posible crear cuellos de botella.

---

## 2. INITIAL SITUATION

### ¿Cómo era la situación antes?. ¿Qué indicadores eran malos?. ¿Qué restricciones existían?.

La restriccion para conocer una capacidad instalada era
Las piezas pasaban por diferentes procesos , es decir diferentes maquinas, torno horizontales, tornos verticales, centro de mecanizado CNC, cortadores de hilo, etc
Cada pieza dependiendo de su tamaño, material o modelo podia pasar por el mismo tipo de maquina pero de diferente tamaño (pasar por un torno chico o torno grande) y demorar diferentes tiempos segun el tamaño o material.
El taller tenia diferentes tamaños de maquinas que complian la misma funcion , esto era para mecanizar piezas chicas en maquinas chicas y piezas grandes en maquinas grandes.
Las piezas se mecanizaban por lotes para optimizar el setup de las maquinas.
Algunas piezas se tenian que enviar a mecanizar en talleres externos principalmente porque era una pieza grande y no entraba en nuestra maquina o no se tenia la maquina para ese tipo de trabajo.

Los tiempos eran realtivamente estandarizados pero ante la gran variedad de piezas que se trabajaban en paralelo el control  era complejo.

---

## 3. BUSINESS OBJECTIVE

### ¿Qué esperaba conseguir la empresa?. ¿Qué esperaba tu jefe?. ¿Qué esperabas tú?

El gerente esperaba que alguien calcule la capacidad real de la planta
Yo no sabía como presentar esta informacion en un proceso con tanta variabilidad, tantas interacciones entre areas, en un flujo no lineal, organizar esta informacion y hacerla una herramienta de decision era un reto que nunca habia asumido.

---

## 4. ROOT CAUSE ANALYSIS

### ¿Cómo analizaste el problema?. ¿Por qué descartaste otras soluciones?

ante tanta incertidumbre de datos y la dificultad de aplicar teoria de resticciones de manera directa empecé por el final, es decir , imaginar como sería el resultado esperado.
Llegué a conclusion que para que sea una herramienta de decision, el resultado del trabajo debia ser un modelo matematico con la siguiente estructura:
Inputs: 
- requerimiento de bombas nuevas
- requerimiento de piezas para stock (proporcinal a las bombas existentes y a su consumo)
- requerimiento de bombas para mantenimiento
Outputs:
- porcentaje de ocupacion de cada maquina por tipo y tamaño

Con este modelo era posible indicar segun su nivel de ocupacion que maquina o area productiva iba a ser necesario reforzar para evitar cuello de botella
Ademas debia considerar la restriccion de que maquinas grandes pueden hacer el trabajo de maquinas pequeñas pero no viceversa, lo cual ya constituye parte de la refinación del modelo.
Debía considerar horas calendario, personal disponible, feriados y horas extras disponibles, porcentaje de eficiencia, tiempos de setup , tanto en el area de fabricacion de piezas como en el area de montaje.
Debia considerar ademas el impacto de maquinas nuevas y mas modernas que iban a absorver el trabajo de las mas antiguas, por ejemplo un torno CNC iba a absorver el trabajo de un torno convencional. Si teniamos planeado renovar 3 tornos convencionales estos se iban a quedar sin carga.



---

## 5. EXECUTIVE DECISION

### ¿Cuál fue la decisión más importante?. ¿Por qué?

La decision mas importante fué aceptar que sin tener toda la informacion clara y confiable porque se presentaba mucha variabilidad, debia adoptar un criterio para seleccionar la información limpia y asumir de manera confiable la información que no era limpia.
Filtrar la informacion y no asumior valores cerrados sinó tendencias y los valores que eran consistentes, retirar de la muestra los valores anomalos.
Otra decision importante fué entender que mi unidad de medida eran las horas disponibles mientras que para la gerencia eran las bombas producidas y reparadas, en el medio la unidad de conversion eran la piezas de la bombas.

---

## 6. IMPLEMENTATION

### ¿Qué hiciste exactamente?. ¿Cómo convenciste a las personas?. ¿Qué obstáculos aparecieron?

Con los criterios antes mencionados empecé a hacer la revision de toda la data existente, aplicar filtros estadisticos y para los casos que no habia data, extrapolar en funcion de variables que yo definí
El principal obstaculo era la variabilidad de la información ya que los lotes de produccion podian verse afectados por defectos de fundicion, falas de maquina, cambio en el plan de produccion, etc y esto era muy dificil de modelar
La otra dificultad era como presentar la informacion a la gerencia en un formato claro y conciso sin tantos numeros , por lo que decidí presentar escenarios y factores.
Solicité al area de ventas la proyeccion para el siguiente año, la uní con el crecimiento de nuestro parque de bombas y nuestra tendencia de consumo de repuestos alineada con el crecimiento del parque segun cada tamaño o tipo de bomba.

---

## 7. RESULTS

### Resultados cuantitativos.

Puede obtener un modelo matematico que predecía el nivel de ocupacion de el conjunto de maquinas y equipos de montaje segun la proyeccion de ventas y la demanda de bombas de manrtenimiento interno
Como los modelos de bombas iban variando durante el año, este modelo predecia la carga mensual y si queriamos fabriacr un nuevo modelo que necesita una maquina nueva, cuando debiamos comprar la nueva maquina
La planta estaba en plan de expansión fisica, las predicciones de este modelo permitian alinear la llegada de las maquinas con el espacio disponible y la contratacion del personal

### Resultados cualitativos.

La gerencia general tuvo un sustento estructurado para realizar sus expanciones e inversiones en equipos bajo diferentes escenarios.

### Resultados inesperados.



---

## 8. EXECUTIVE THINKING

### ¿Por qué consideras que esta decisión fue correcta?. ¿Qué principio de gestión demuestra?

La decision fué correcta por que satisfació los requerimientos del cliente y fué para mi una herramienta util para mi toma de decisiones 

---

## 9. REUSABLE KNOWLEDGE

### ¿Qué aprendiste?. ¿En qué otras industrias puede aplicarse?

Aprendí que en problemas de modelamiento complejo es necesario orientar la pregunta del usuario y en esta caso hacerle entender que su capacidad era una funcion de lo que el queria vender, es decir su capacidad variaba segun su forecast de ventas.
Aprendí el manejo de escenarios y comopresentar informacion para toma de decisiones de forma simplificada, cada usuario tiene diferentes requerimientos de informacion para toma de decisiones y el modelo debia satisfacer todas las necesidades comoplanes de inversion, planes de expancion, proyeccion de ventas y manejo de stocks

---

## 10. ATS COMPETENCIES

(esta parte la construiré yo)
