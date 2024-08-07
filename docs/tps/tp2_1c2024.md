# Trabajo práctico 2 - Reconocimiento de dígitos a partir de señales de audio

## Objetivos

Este trabajo práctico consiste en el diseño y evaluación de distintos sistemas orientados a la clasificación automática de dígitos a partir de señales de audio. La idea es que se pongan en práctica conceptos estudiados en clase referidos al análisis de señales en el dominio de la frecuencia para diseñar un clasificador basado en técnicas clásicas de procesamiento de señales, y una segunda variante basada en técnicas de aprendizaje automático. En todos los casos, se deberán proponer métricas objetivas que permitan dar cuenta del rendimiento de los sistemas planteados.

## Desarrollo del trabajo

Podemos dividir el trabajo encomendado en dos áreas principales:

  - Diseño de un clasificador automático de dígitos hablados usando técnicas clásicas de procesamiento de señales.
  - Diseño de un clasificador automático de dígitos hablados usando técnicas de aprendizaje automático.

En ambos casos, se les provee un cuerpo de datos que consiste en 3000 grabaciones de un segundo de duración, en donde distintas personas pronuncian, en inglés, los números del 0 al 9.

### Versión clásica

Este primer enfoque está pensado para que apliquen directamente cosas que hayamos visto durante la cursada, o herramientas que se desprendan de ellas. A continuación, un par de puntos a tener en cuenta para arrancar y para tener en cuenta durante el desarrollo del trabajo:

  - Una propuesta posible de clasificador consiste en el cálculo de versiones promedio de los audios de los distintos números a detectar. De esta forma, de la cantidad de audios en donde se pronuncia el 0, por ejemplo, uno podría calcular una representación promedio, ya sea en el dominio de las muestras, en el de la frecuencia, o en algún tipo de parametrización. Una vez que se obtiene una representación promedio para cada dígito, uno podría tomar un audio cualquiera y compararlo con cada una de ellas usando alguna métrica objetiva. A partir de este resultado, el par promedio-audio que tenga la menor diferencia podría indicarnos qué dígito se está pronunciando en esa instancia en particular.
  - Es importante que propongan distintos tipos de análisis que permitan estudiar qué pasa si cambio distintos parámetros de su clasificador. Por ejemplo, siguiendo con la propuesta de las representaciones promedio de cada dígito, ¿qué pasa si trabajo en tiempo? ¿y en frecuencia? ¿pierdo algo en un caso o en otro? Este tipo de preguntas son las que se deberían hacer antes de comenzar a trabajar y son las que van a guiar su propuesta.

Es importante notar que lo explicado en esta sección es meramente orientativo, son muy bienvenidas propuestas originales para el diseño de los clasificadores (aunque se recomienda consultar preventivamente con los docentes si la propuesta es viable).

### Versión con redes neuronales

Además del cuerpo de datos, se les provee el código de una red neuronal simple destinada a la predicción del dígito pronunciado en un archivo de audio. La tarea en esta etapa del trabajo es más guiada que en la otra, se propone estudiar cómo variar el dominio en la que se presentan los datos durante el entrenamiento del modelo repercute en el resultado final y en la calidad de las predicciones. Se requieren tres versiones del modelo: una en donde el dato ingresado corresponde a la forma de onda cruda, sin ningún procesamiento; otra en donde el dato ingresado corresponde al módulo de la DFT de los audios y una última en donde se ingresan los coeficientes MFCC de las señales. ¿Hay alguna representación de los datos de entrada que de mejores resultados? ¿Por qué puede ser?

No es necesario ningún conocimiento previo de redes neuronales o aprendizaje automático para poder llevar a cabo esta etapa, lo único que deben hacer es completar con su código el archivo `dataset.py` y analizar los datos que se generan automaticamente luego de ejecutar `train.py` y `test.py`.

## Entrega

Los resultados y el análisis propuestos deben estar contenidos en un informe técnico (escrito con buena ortografía y redacción en español rioplatense) que siga el formato provisto por la cátedra. Los gráficos y tablas deben ser claros y legibles, además de tener sus correspondientes títulos y unidades (sin los cuales el gráfico o tabla se considerará nulo).

Cada resultado debe estar acompañado con un análisis en donde se discuta si lo obtenido es lo esperable o no, y por qué. Todo debe estar justificado y acompañado con gráficos o tablas que lo sustente.

Este trabajo es mucho menos guiado que el anterior, los requerimientos expresados en este documentos son los mínimos esperados pero serán muy bien recibidas preguntas nuevas y originales que escapen a las propuestas inicialmente. 

Recomendamos fuertemente hacer el trabajo con la mayor antelación posible; el tiempo que lleva el trabajo efectivo debería ser corto en contraste con el tiempo de razonamiento y análisis del problema, que puede llevar varios días. 

El trabajo se realizará en grupos de hasta 3 personas. Los grupos deben estar inscriptos en el campus de la materia, sin excepciones. 

Se debe realizar la entrega de los archivos a través de la tarea creada en el campus. En la misma se encuentra la fecha de entrega. No se considerarán entregas realizadas fuera de tiempo salvo casos de fuerza mayor.

Se espera que la entrega esté compuesta por dos archivos, un .pdf con el informe y un archivo con el código usado para el análisis y confección de los gráficos (lenguaje a elección, recomendamos Python).

**El informe no puede superar las 15 páginas (estricto).**

Se recuerda a los estudiantes que las entregas deben ser un producto original de cada estudiante, por lo que se les pide revisar el Código de Honor y Ética.



