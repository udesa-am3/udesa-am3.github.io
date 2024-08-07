# Trabajo práctico 1 - Series de Fourier

## Objetivos

El objetivo principal de este trabajo es el estudio de las **series de Fourier** como herramienta para aproximar funciones a partir de senos y cosenos. Además, se buscará estudiar **criterios de convergencia** de este tipo de series y verificar resultados teóricos como el **fenómeno de Gibbs**.

## Desarrollo del trabajo

Las pruebas se harán sobre dos tipos de señales: un tren de pulsos y una diente de sierra. La primera de las señales está definida según la siguiente ecuación 

$$x(t)= A\;sgn(sen(2\pi f t))$$

donde $A$ corresponde a la amplitud del pulso, $f$ a la frecuencia de oscilación, $t$ al tiempo y $sgn$ a la función signo, que se define según la ecuación

$$sgn(t)= \left\{ \begin{array}{lcc} -1 & si & t < 0 \\ \\ 0 & si & t = 0 \\ \\ 1 & si & t > 0 \end{array} \right.$$

Por otro lado, la señal diente de sierra queda definida según la ecuación 

$$x(t)= A\;\left(t\;f - \left\lfloor\frac{1}{2} + t\;f \right\rfloor\right)$$

en donde $A$ corresponde a la amplitud de la señal, $f$ a su frecuencia y $\lfloor \rfloor$ a la función piso, que toma un número real y devuelve el mayor número entero menor que el ingresado.

Ambas funciones tienen definiciones alternativas con diferencias sutiles, pueden usar la definición que quieran pero tiene que quedar asentado en su entrega.

El análisis requerido consta de los siguientes puntos:

1.  Analizar si las señales propuestas cumplen con las condiciones de Dirichlet.

2.  Desarrollarlas en series de Fourier, calculando y desarrollando sus coeficientes (a mano).

3.  A partir de los coeficientes calculados, escribir una función que permita sintetizar las señales propuestas con un número arbitrario de armónicos.

4.  Usando la función escrita, grafique las aproximaciones conseguidas en cada caso con 10, 30 y 50 armónicos. En esta parte se esperan dos gráficos, uno por señal. En cada uno de ellos deben estar graficadas las 4 señales de interés (original, aproximación con 10 armónicos, con 30 y con 50).

5.  Analice el comportamiento de las aproximaciones conseguidas en el entorno de las discontinuidades. ¿Se cumple el fenómeno de Gibbs? Verifique la amplitud de las aproximaciones en los puntos discontínuos de las señales para confirmarlo.

6.  Calcule el error cuadrático medio de las aproximaciones con 10, 30 y 50 armónicos en zonas sin discontinuidades. Reporte el resultado y analícelo teniendo en cuenta el resultado obtenido en el punto anterior.

7.  Escriba una segunda función, que en este caso no reciba una cantidad de armónicos como parámetro de entrada sino que utilice el error cuadrático medio entre la señal y la aproximación como criterio de paro. Proponga un valor de error cuadrático medio, gráfique la aproximación conseguida y reporte la cantidad de armónicos necesarios para llegar a ese resultado. ¿Cuánto influye la parte cercana a la discontinuidad en comparación con tramos lejanos a la discontinuidad en la cuenta total del error cuadrático medio? Justifíquelo.

8.  Concluya sobre el efecto de aumentar arbitrariamente el número de armónicos utilizados y su relación con el error cuadrático medio entre la aproximación y la señal original.

9.  Repita el análisis pero partiendo de una señal sin discontinuidades, como una triangular.

Punto Opcional: Interpretando esta señal como una señal de audio, escriba una función que permita sintetizar alguna de las señales propuestas, sumándole coeficientes a la serie de forma iterativa. Por ejemplo, cada 1 segundo sumar 5 armónicos, entonces el primer segundo de la señal resultante tendrá 5 armónicos, el segundo 10, el tercero 15 y así sucesivamente. Guarde la señal generada en un archivo de audio y compárelo con la señal original.

Todos los gráficos deben ser legibles, deben tener títulos en los ejes y leyendas que permitan indicar a qué corresponde cada señal mostrada. Las funciones deben tener su docstring correspondiente.

## Condiciones de entrega

El trabajo se realizará en grupos de hasta 3 personas. **Los grupos deben estar inscriptos en el campus de la materia**. Se debe realizar la entrega de los archivos de Python generados a través de la tarea creada en el campus de la materia. En la misma (y en el calendario) se encuentra la fecha de entrega.

Los archivos deben llamarse 'tp1_NOMBRE_DE_GRUPO_X.extension', en donde 'X' es un nombre representativo del contenido de ese archivo, y 'extension' corresponde justamente a la extensión del archivo.

Como mínimo se espera que entreguen dos archivos, un .py con el código de las funciones pedidas (y otras que pudieran llegar a necesitar) y un .ipynb en donde deben estar los resultados obtenidos en los distintos puntos, incluyendo análisis en forma de texto y gráficos. Para los cálculos de los coeficientes de Fourier de las señales se aceptan escanéos (o fotos en buena calidad y legibles) del desarrollo hecho a mano, pero se prefiere el uso de LaTex.

Se recuerda a los estudiantes que las entregas deben ser un producto original de cada estudiante, por lo que se les pide revisar el Código de Honor y Ética.
