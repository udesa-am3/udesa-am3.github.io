# Guía 4 - Transformada discreta de Fourier

1.  Dada la siguiente señal $x[n]$ de 8 muestras, calcular la DFT de dicha señal. 

    ::: center
    ![image](1){width="60%"}
    :::

    *Para resolver con algún lenguaje de programación:* 
    
    Escribir un algoritmo que calcule la DFT utilizando el método de cálculo rápido de la transformada (FFT).

1.  Dada la señal $y[n]$, calcular la DFT de 16 muestras. Además graficar la magnitud, la fase, parte real y la parte imaginaria de la trasnformada.

    $$y[n] = 2 sen \left(\frac{2\pi n}{8}\right)$$

1.  Dada la señal $y[n]$ de 32 muestras:

    $$y[n] = 3 - e^{-j\pi n / 4}+ e^{j\pi n/4}$$

    1.  Escriba su transformada discreta de Fourier $Y[k]$ utilizando el total de las muestras (No es necesario que se resuelva la sumatoria en función de $n$).

    1.  Inspeccionando $Y[k]$, ¿para qué valores de $k$ la respuesta en módulo de $Y[k]$ será no nula?¿Por qué? ¿Puede estimar qué magnitud tendrá $Y[k]$ para estos valores?

    *Para resolver con algún lenguaje de programación.*

    1.  Desarrolle un código para evaluar la función $Y[k]$ determinada en el primer inciso. Utilizando la función *stem*, realice dos gráficos en una única figura con el módulo y la fase de $Y[k]$. ¿Coinciden los resultados encontrados con lo que predijo en el punto b)?

1.  Dado el siguiente gráfico del módulo de la DFT de una señal real *sin leaking* $Y[k]$, encuentre la función temporal que le dio origen. Asuma que la fase es nula.

    ::: center
    ![image](5){width="50%"}
    :::

1.  Representar gráficamente toda la información (componentes real, imaginario y fase) de la DFT de 16 muestras de la siguiente señal:

    $$y[n] = -1 + sin \left(\frac{\pi}{4}n\right) - cos \left(\frac{\pi}{2}n\right)$$

1.  Dadas las 4 señales temporales discretas $y_i[n]$ de 64 muestras que se definen a continuación:

    $$y_1[n] = u[n]\;\;\; Y_1[k] = \begin{cases}\dfrac{N}{2} & k = 0 \hspace{6pt} y \hspace{6pt} k = 63\\ 0 & otro\hspace{6pt}caso \end{cases}$$
    
    $$y_2[n] = \dfrac{1}{2}sen \left(\dfrac{2\pi}{4}n\right) u[n]\;\;\; Y_2[k] = \begin{cases}\dfrac{N}{8}i & k = 8\\-\dfrac{N}{8}i & k = 56\\ 0 & otro\hspace{6pt}caso \end{cases}$$
    
    $$y_3[n] = 2cos\left(\dfrac{2\pi}{8}n\right)u[n]\;\;\; Y_3[k] = \begin{cases}N & k = 8 \hspace{6pt} y \hspace{6pt} k = 56\\ 0 & otro\hspace{6pt}caso \end{cases}$$
    
    $$y_4[n] = cos\left(\dfrac{2\pi}{12}n\right)u[n]$\;\;\; Y_4[k] = \begin{cases}\dfrac{N}{2} & k = 12 \hspace{6pt} y \hspace{6pt} k = 52\\ 0 & otro\hspace{6pt}caso \end{cases}$$

    1.  Sin realizar ningún cálculo, evalúe para cada caso si las $Y_i[k]$ provistas efectivamente corresponden a la DFT de cada función $y_i[n]$. Para esto, halle las frecuencias características de cada señal. ¿Cómo interactúan éstas con la cantidad de muestras que se evalúen?

    *Para resolver con algún lenguaje de programación:*

    1.  Desarrolle un código para graficar cada función junto con su transformada (*puede usar módulos que tengan la función FFT*). Es importante que logre centrar las respuestas en frecuencias en 0. De esta manera, debería ser posible identificar los valores de $k$ que corresponden a frecuencias negativas y aquellos que corresponden a frecuencias positivas.

1.  En este ejercicio, se busca evaluar el efecto de un desplazamiento temporal (*delay*) en la respuesta de la DFT. Calcule la transformada de la señal $x[n]$ de 16 muestras:

    $$x[n] = \delta [n]$$

    *Para resolver con algún lenguaje de programación:*

    1.  La transformada del delta es conocida; de todas formas grafíquela utilizando algún software. Para este ejercicio es de interés analizar la
magnitud, la parte real y la fase de la DFT.

    1.  Realice un desplazamiento temporal de la señal. Analice la nueva señal desplazada $x_1[n]$:

        $$x_1[n] = \delta [n-1]$$

    Realice el mismo gráfico del punto a). ¿Qué puede decir sobre la nueva DFT?

    *Para resolver analíticamente:*

    1.  Escriba en papel las dos transformadas. ¿En qué se diferencian? Puede realizar un nuevo desplazamiento temporal para ayudarse. Intente deducir cómo se refleja el desplazamiento temporal en el dominio de la frecuencia.

1.  Dadas dos secuencias discretas de cuatro puntos $x[n]$ y $h[n]$:

    $x[n] = cos\left(\dfrac{\pi n}{2}\right)$ $h[n] = 2^n$ $n = 0,1,2,3$

    1.  Calcular la DFT $X[k]$ de cuatro puntos de $x[n]$, y graficar su módulo.

    1.  Calcular la DFT $H[k]$ de cuatro puntos de $h[n]$, y graficar su módulo.

    1.  Calcular la convolución circular de $x[n]$ y $h[n]$.

    *Para resolver con algún lenguaje de programación:*

    1. Desarrolle un algoritmo para realizar los cálculos de los incisos anteriores y muestre gráficamente los resultados (módulo de $X[k]$, módulo de $H[k]$ y el resultado de la convolución circular).

1.  Dados los primeros tres valores de una DFT de cuatro muestras de una determinada señal x\[n\] real:

    $$X[k] = [11\; -2+3j\; -3\;\; ???]$$

    Calcular la DFT de las siguientes señales:

    -   $x_1[n] = x[n+2]$

    -   $x_2[n] = x^2[n]$

1.  Para las siguientes señales discretas finitas de $N = 64$ muestras, determinar:

    1.  La magnitud y la fase de la DFT de la señal $x_1[n] = sen \left(\dfrac{5}{16}\pi n\right) -1$. ¿Existe el efecto de
*leaking*?

    1.  El valor de la frecuencia de la señal $x_2[n] = 2 cos \left(\dfrac{5}{64}\pi n\right)$. ¿Existe el efecto de *leaking*?

    1.  El valor **exacto** de la magnitud de la DFT de la señal del punto anterior, $|X[k]|$, solamente para las muestras $k = 2$ y $k = 3$.

    ??? "Nota"
        La transformada de una ventana rectangular de $N$ muestras $(0,...,N-1)$ es:

        $$V[k]= e^{-j\pi k \left(\frac{N-1}{N}\right)} \frac{sen(\pi k)}{sen\left(\dfrac{\pi}{N}k\right)}$$

1.  A continuación se presenta la secuencia discreta $x[n]$,

    $$x[n] = [\underline{2},-1,0,c,1]$$

    en donde $c$ es una constante desconocida y $[\,\underline{ }\,]$ denota la muestra 0.

    Por otro lado, conocemos una segunda secuencia $x_1[n]$, definida según

    $$x_1[n] = [\underline{2},1,2,-1,0]$$

    Y sabemos que existe la siguiente relación entre las DFTs $X[k]$ y $X_1[k]$:

    $$X_1[k] = X[k]e^{-j(2\pi k m /5)}$$

    A partir de esta información, calcule $c$.
   
1.  Dada una señal discreta $x$ de 32 muestras definida según la siguiente expresión:

    $$x = 0.75^n + B\delta[n-4]\;\;B \in \mathbb{R}$$
    
    1.  Calcule su DFT.
    1.  Determine el valor de $B$ de forma tal de que se cumpla la siguiente relación:
        
        $$\sum_{n=0}^{31}|x[n]|^2 = 64$$

1.  La siguiente figura muestra un espectrograma de una señal, una tipo de representación tiempo-frecuencia, en donde se puede observar cómo varía el espectro de una señal en el tiempo:

    ::: center
    ![image](11){width="65%"}
    :::

    En este tipo de representaciones, el eje $y$ simboliza la frecuencia mientras que el eje $x$ corresponde a las muestras.

    Sabemos que la señal temporal descripta por el espectrograma tiene la forma:

    $$x[n] = 2\sqrt{2} sen(\omega_0\;n + 500 cos(\omega_{mod}\;n))$$

    Inspeccionando el gráfico, determine de forma aproximada los valores de $\omega_0$ y $\omega_{mod}$. ¿Qué puede decir sobre la simetría de esta
representación? ¿Nota algo particular?
