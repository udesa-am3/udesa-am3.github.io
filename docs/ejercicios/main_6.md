# Guía 6 - Transformada de Fourier

1.  Usando la ecuación de análisis, caluclar las transformadas de Fourier de las señales:

    1.  $f(t) = e^{-2(t-1)}u(t-1)$

    1.  $f(t) = e^{-2|t-1|}$

    Grafique de forma aproximada la magnitud de las transformadas obtenidas.

1.  Use la ecuación de análsis para encontrar la transformada de Fourier de las siguientes señales:

    1.  $f(t) = \delta(t+1) + \delta(t-1)$

    1.  $f(t) = \frac{d}{dt}\{u(-2-t) + u(t-2)\}$

    Grafique de forma aproximada la magnitud de las transformadas obtenidas.

1.  Determine la transformada de Fourier de la siguiente señal periódica:

    $$f(t) = sen\left(2\pi t + \frac{\pi}{4}\right)$$

1.  Usando la ecucación de síntesis, calcule la antitransformada de las siguientes señales:

    $$F(j\omega) = 2\pi \delta(\omega) + \pi \delta(\omega-4\pi) + \pi \delta(\omega + 4\pi)$$

1.  Usando la ecuación de síntesis, calcular la antitransformada de $X(j\omega)$, sabiendo que:

    $$|X(j\omega)| = 2\{u(\omega+3)-u(\omega-3)\}$$

    $$\angle X(j\omega) = -\frac{3}{2}\omega + \pi$$

    A partir de esa respuesta, determine los valores de $t$ para los que $x(t)$ vale $0$.

1.  Sabiendo que la transformada de Fourier de $x(t)$ es $X(j\omega)$ y usando propiedades, calcular la transformada de las siguientes señales:

    1.  $x_1(t) = x(1-t) + x(-1-t)$

    1.  $x_2(t) = x(3t-6)$

    1.  $x_3(t) = \frac{d^2}{dt^2}x(t-1)$

1.  Considere la siguiente señal:

    $$x(t)= \left\{ \begin{array}{lcc} 0 & si & t < \frac{1}{2} \\ \\ t+\frac{1}{2} & si & -\frac{1}{2} \leq t \leq \frac{1}{2} \\ \\ 1 & si & t > \frac{1}{2} \end{array} \right.$$

    1.  Usando las propiedades de integración y diferenciación en el dominiodel tiempo y la transformada de Fourier del pulso rectangular, calcule $X(j\omega)$.

    1.  ¿Cuál es la transformada de Fourier de $g(t) = x(t) - \frac{1}{2}$?

1.  Usando tablas, calcule la transformada de Fourier de la siguiente señal:

    $$x(t) = t \left(\frac{sen(t)}{\pi t}\right)^2$$

1.  Usando la relación de Parseval y el resultado del punto anterior, dar el valor numérico de la siguiente integral:

    $$\int_{-\infty}^{\infty} t^2 \left(\frac{sen(t)}{\pi t}\right)^4 dt$$

1.  Dadas las relaciones:

    $$y(t) = x(t)*h(t)$$

    donde $*$ representa al operador convolución lineal; y:

    $$g(t) = x(3t)*h(3t)$$

    y sabiendo además que $x(t)$ tiene una transformada de Fourier $X(j\omega)$, $h(t)$ tiene una $H(j\omega)$, use propiedades para demostrar que:

    $$g(t) = Ay(Bt)$$

    Determinar los valores de $A$ y $B$.

1.  Sea $x(t)$ una señal continua con transformada de Fourier $X(j\omega)$. Supongamos que nos dan la siguiente información:

    1.  $x(t)$ es real.

    1.  $x(t) = 0$ para $t\leq0$.

    1.  $\frac{1}{2\pi}\int_{-\infty}^{\infty} \Re \{X(j\omega)\}e^{j\omega t} d\omega = |t|e^{-|t|}$

    Determinar una expresión para $x(t)$.

1.  Determinar si las siguientes expresiones son verdaderas o falsas, justificando la respuesta:

    1.  Una señal impar e imaginaria siempre tiene una transformada de Fourier impar e imaginaria.

    1.  La convolución entre una transformada de Fourier impar y una transformada de Fourier par siempre es impar.
    
1.  Determinar la transformada de Fourier $F$ de una señal $f: \mathbb{R} \rightarrow \mathbb{R}$ definida como:

    $$f(t) = t e^{-|t|}$$
    
    1.  Dada $h(t) = 0.5\delta (t)+ 0.5 \delta (t-17)$, hallar $g(t) = f(t)*h(t)$.
    1.  Graficar (esquematicamente), $f(t), |F(\omega)|, h(t), g(t)$.


