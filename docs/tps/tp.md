# Trabajo práctico  - Identificación de sistemas desconocidos

## Objetivos

Este trabajo práctico consiste en la medición y análisis de un sistema desconocido, con la idea de poder describirlo para entender su funcionamiento. Puntualmente, el sistema propuesto corresponde a un circuito electrónico del cual nos interesa, a priori, su comportamiento en frecuencia.

## Desarrollo del trabajo

A cada equipo se le va a proveer un circuito electrónico ya armado que deberán tratar como si fuera una _caja negra_. Esto significa que no tienen acceso a los componentes del mismo, ni conocerán la topología del circuito que se les dio. Solo tendrán acceso a un par de pines de entrada y a otro par de pines de salida, en donde deberán conectar los distintos instrumentos de medición que permitirán simultáneamente inyectar una señal de medición al sistema y medir cómo este la afecta a la salida del circuito.

En este último punto radica uno de los temas centrales del trabajo práctico: ¿qué señal de medición (o señales) propongo para caracterizar mi sistema? Esta elección debe realizarse teniendo en cuenta que, como mínimo, la idea es entender el funcionamiento del circuito en el dominio de la frecuencia, es decir, buscamos contestar cómo afecta espectralmente a una señal de entrada arbitraria.

Temas secundarios, pero sumamente interesantes, están relacionados a la medición en sí. Yo elijo una señal de medición que asumo que caracteriza correctamente mi sistema, pero ¿es mi instrumental de medición perfecto? ¿qué nivel tiene que tener la señal de entrada? ¿qué pasa si la amplitud es muy baja? ¿y si es muy alta? Indefectiblemente la medición eléctrica que hagan va a tener que ser digitalizada para poder analizarla ¿cómo se relaciona el ancho de banda que puede procesar el equipo de medición con la frecuencia de muestreo que propongo para la discretización? ¿puedo caracterizar mi equipo de medición? ¿qué tan confiable es lo que estoy midiendo? ¿puedo proponer cotas de error para los resultados que presente? Último detalle, volviendo al mundo de señales y sistemas: Mencionamos que nos interesa caracterizar la respuesta en frecuencia del sistema pero ¿podemos decir algo acerca de la ubicación de los polos y ceros del sistema que caracterizamos?

### Condiciones necesarias y suficientes para aprobar

Como mínimo, esperamos que entreguen un informe con un diagrama de Bode del sistema que caracterizaron, acompañado de una descripción lo más detallada posible del procedimiento que siguieron para medir y procesar los datos, además de las justificaciones de las distintas decisiones que tomaron a lo largo del trabajo. Se espera que prueben más de una señal de medición de entrada y que estudien las diferencias en los resultados que obtengan con cada una de ellas.

Más allá de eso, cualquier otro análisis es bienvenido y será muy bien considerado para la nota final del trabajo. Varias de las preguntas planteadas en la sección anterior son buenos puntos de partida. No esperamos que contesten todo (¡pero nos pondría muy contentos si pasara!), pero si que intenten algo por este lado.

## Entrega

Los resultados y el análisis propuestos deben estar contenidos en un informe técnico (escrito con buena ortografía y redacción en español rioplatense) que siga el formato provisto por la cátedra. Los gráficos y tablas deben ser claros y legibles, además de tener sus correspondientes títulos y unidades (sin los cuales el gráfico o tabla se considerará nulo).

Cada resultado debe estar acompañado con un análisis en donde se discuta si lo obtenido es lo esperable o no, y por qué. Todo debe estar justificado y acompañado con gráficos o tablas que lo sustente.

El enunciado de este trabajo es intencionalmente vago, es importante que empiecen a pensar en las preguntas con la mayor antelación posible para entender el problema, que muy probablemente les resulte distinto a lo que están acostumbrados a hacer.

El trabajo se realizará en grupos de hasta 4 personas. Los grupos deben estar inscriptos en el campus de la materia, sin excepciones.

Se debe realizar la entrega de los archivos a través de la tarea creada en el campus, tanto para la pre-entrega como para la entrega final. En la misma se encuentra la fecha de entrega. No se considerarán entregas realizadas fuera de tiempo salvo casos de fuerza mayor.

La pre-entrega no será calificada, sólo servirá para orientar a la cátedra (y a ustedes) sobre las dificultades que surjan durante el desarrollo del trabajo.

Se espera que la entrega esté compuesta por dos archivos, un .pdf con el informe y un archivo con el código usado para el análisis y confección de los gráficos (lenguaje a elección, recomendamos Python).

**El informe no puede superar las 15 páginas (estricto).**

Se recuerda a los estudiantes que las entregas deben ser un producto original de cada estudiante, por lo que se les pide revisar el Código de Honor y Ética.


