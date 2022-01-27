# Sprint-4_covid
Informe Pandémico: Estadística Aplicada



Propósito y Scope

Te encuentras trabajando en una ONG de Data Science que se dedica a hacer estudios con enfoque estadístico sobre distintos temas de interés social. En este caso, te contrataron para que elabores un informe sobre características básicas de la pandemia de COVID-19 y elabores un algoritmo capaz de entender, a partir de las curvas de contagios, si las poblaciones están vacunadas o hicieron cuarentena.

En este estudio tendrás que entender qué significan algunos indicadores de la pandemia, y cómo medirlos a partir de las curvas de contagio. Luego, tendrás que aplicar métodos estadísticos para analizar los datos de algunos países y sacar conclusiones a partir de eso. Será de mucha utilidad la documentación de las librerías de Python. No dudes en consultar comunidades online como Stack Overflow y, por supuesto, buscar en la web (googlear).

Interpretando curvas de contagio

¡Bienvenidos/as investigadores! Nos alegramos que se hayan interesado por este tema. En esta oportunidad vamos a trabajar en el análisis estadístico de datos, para entender y evaluar el éxito de las políticas públicas que tomaron los países para enfrentar la pandemia.

Instrucciones

Lee atentamente el notebook e investiga un poco sobre modelos pandémicos de aplicación para elaborar tu proyecto. El objetivo es que apliques las herramientas que conoces  para estudiar distintos aspectos de la pandemia. Recuerda que puedes volver a consultar todas las bitácoras y notebooks de este sprint para refrescar los conocimientos.

A continuación encontrarás el notebook con las consignas y el dataset. Ten en cuenta que ya esperamos cierto grado de independencia de parte tuya. Por eso, las consignas y recomendaciones de los notebooks no son exhaustivas. Es decir, si hay un paso en el flujo de trabajo que no está mencionado en el notebook que te dejamos, no implica que no haya que hacerlo. Recuerda que debes revisar el Exit Criteria para confirmar que cumples con todos los puntos.

Primera parte: ¿Cómo empezó la pandemia?

En la primera parte el objetivo del proyecto es entender cómo empezó la pandemia, es decir, estudiar la etapa de “crecimiento exponencial” de la misma. La idea es que comprendas qué parámetro guía esto y de qué depende. Luego, tienes que intentar entender si puedes predecir el comportamiento global de la pandemia a partir del estudio de unos pocos países bien elegidos y utilizando herramientas estadísticas estudiadas en este sprint.

•	Dataset. En este link puedes encontrar el dataset de cantidad de contagios en cada país del mundo. Descárgalo en formato .csv y ponlo en una carpeta de Drive para luego trabajar con él. En el notebook se muestra cómo cargar los datos desde tu Drive usando la librería pandas.

•	Notebook. Aquí te dejamos un notebook con algunas recomendaciones y líneas de código para que empieces a explorar los datos.


Segunda parte: Evaluando estrategias
En esta segunda parte tienes más libertad. Debes elegir al menos una estrategia que los estados hayan elegido para enfrentar la pandemia (vacunar o hacer cuarentena) y pensar indicadores del éxito o fracaso de dicha estrategia que se puedan medir en la curva de contagios.

Un ejemplo posible de esto puede ser: si eliges analizar la cuarentena, puedes ver si se redujo el parámetro de crecimiento k (esto está mejor explicado en la primer parte del notebook) o cuánto tardó la curva de nuevos contagios en alcanzar el pico o qué porcentaje de población se contagió.

Una vez que elijas algunos indicadores, busca información sobre países que hayan implementado o no esa estrategia. Por ejemplo, si se trata de la cuarentena, sabemos que China aplicó una cuarentena muy estricta y que Brasil no aplicó esa medida. A partir del estudio de varios ejemplos de cada tipo, debes construir clasificadores por regresión logística, uno por cada indicador que hayas elegido. Allí se debe poder predecir la política aplicada según la medición del indicador.

Un ejemplo podría ser intentar predecir si un país hizo cuarentena a partir de medir el porcentaje de población que se contagió en el momento del pico.
Cuando hayas terminado tu clasificador, úsalo para interpretar los datos de nuevos países, que aún no hayas incluido (recuerda que tienes mucha información en el dataset).


Tercera parte: Elaboración de Informe Final
Para finalizar, elabora un informe sobre lo que significa el parámetro de crecimiento y con qué estrategias epidemiológicas puede modificarse. Por un lado, debes mencionar si es posible elaborar un análisis estadístico que brinde información sobre lo que pasa en todo el mundo a partir del estudio de algunos casos particulares. Por otro lado, también debes discutir si es posible identificar las políticas adoptadas por los países a partir del clasificador que armaste. Debes debatir en el informe sobre las razones por las cuales lo que hayas hecho funciona o no, en las dos partes previas del trabajo.
Recuerda incluir distintos gráficos, histogramas, ajustes de modelos, evolución de los contagios o cualquier cosa que se te ocurra, para argumentar en tu informe.


Condiciones de Entrega
Deberás entregar un notebook de Jupyter y un informe con la resolución de las distintas consignas.el notebook debe poder ejecutarse sin errores.
•	En el notebook debe estar el link al repositorio (por ejemplo, de GitHub) donde se pueda encontrar el proyecto entregado.
•	El informe debe argumentar claramente por qué funcionó o no (según corresponda) el análisis implementado, y debe incluir distintos gráficos que ayuden a la justificación.


Story Points
A continuación podrás ver el listado de Story Points. Estos te ayudarán rápidamente a ordenar, planificar, estimar y priorizar tu backlog de tareas.
la totalidad de los requerimientos mínimos.
Podrás escoger diferentes requerimientos del listado del backlog. Deberás sumar una mínima cantidad de 128 Story Points. Llegarás a este valor completando la totalidad de los requerimientos mínimos. Anímate también a completar los requerimientos adicionales. ¡Cuantos más sumes, mejor!
  
Exit Criteria
¡Ya casi estamos! Ahora necesitamos de tu ayuda para organizar el trabajo de retroalimentación. Vamos a usar criterios de aceptación para que puedas comprender el feedback de tu Tech Reviewer. Estos criterios son ejemplos concretos reales de uso del sistema para que puedas probar el funcionamiento de tu producto. De esta forma, lograremos que la evaluación sea más estandarizada y transparente. Para cada historia de usuario listada anteriormente, se asignan criterios de aceptación. Te contamos aquí los criterios técnicos que se toman para llegar a cada requerimiento.


Criterios de Aceptación
Sugerencias para desarrollar el proyecto:
•	La resolución del proyecto te puede enfrentar a desafíos que no trabajaste durante las meetings. Es importante que desarrolles la capacidad de resolverlos.
•	Todos los pasos deben estar correctamente justificados.
•	Las preguntas que se respondan deben estar correctamente explicitadas.
•	Imagina que este proyecto lo usarías para presentar en una entrevista de trabajo, o que lo debes presentar en tu trabajo actual. Presta mucha atención a la redacción, presentación de gráficos, etc.


Parte 1 - Exploración de Datos y estudio de la etapa exponencial
•	El análisis Exploratorio de Datos debe servir para comprender el dataset y todo el flujo de trabajo que le siga.
•	Debes responder al menos una pregunta original con este dataset. La pregunta debe estar correctamente explicitada.
•	Debes entender el rol del parámetro k y ver si es posible entender el k mundial a partir de analizar una población de países.
•	Justifica cada una de las respuestas.


Parte 2 - Evaluando estrategias
•	Debes elegir indicadores que sirvan para clasificar una determinada política pública.
•	Debes poder determinar por qué los clasificadores funcionan bien o mal.
•	Si el modelo lo permite, debes explorar qué información utiliza para predecir e interpretar el resultado: ¿coincide con lo que esperabas a partir de tu experiencia con el dataset?


Parte 3 - Investigación
•	Debes explicar qué te gustaría probar, por qué y cómo lo harías. Si tienes referencias (por ejemplo, un artículo que hayas encontrado, capítulo de libro, etc.) debes mencionarlas.
•	Debes comentar también qué resultados esperas encontrar. Por ejemplo, puedes implementar una prueba rápida y mostrar resultados preliminares, para ver si estás correctamente orientado.
•	Debes elaborar un informe que condense y explique todo tu trabajo.
 
Ahora sí, ¡hora del delivery! Recuerda que puedes entregar hasta tres veces. Iterar es la forma de mejorar y aprender durante el camino. Recibirás el feedback del tech reviewer en un lapso de no más de 7 días desde el momento de la entrega.
Ánimos y… ¡felicidades! Llegar hasta aquí ya es todo un logro.
