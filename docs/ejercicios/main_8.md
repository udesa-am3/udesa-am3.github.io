# Guía 8- Transformada Z

1.  Calcular la transformada Z de las siguientes funciones:

    1.  $x[n] = \sqrt[]{3} \delta [n]$

    1.  $x[n] = u[n]$

    1.  $x[n] = cos [\beta n] u[n]$

    1.  $x[n] = u[n] - u[n-5]$

    1.  $x[n] = n\{u[n] - u[n-6]\}$

    1.  $x[n] = \left(\dfrac{1}{3}\right)^{n} u[n] - \left(\dfrac{1}{2}\right)^{n} u[-n-1]$

    1.  $x[n] = \begin{cases}a^{n-1} & n = 1,2,3,... \\ 0, & n \leq 0 \end{cases}$

1.  Calcular la transformada inversa de la siguiente función para las siguientes regiones de convergencia: 

    $$X(z) = \dfrac{3 - \dfrac{5}{6}z^{-1}}{\left(1 - \dfrac{1}{4}z^{-1}\right)\left(1 - \dfrac{1}{3}z^{-1}\right)}$$

    1.  *ROC*: $|z| > \dfrac{1}{3}$

    1.  *ROC*: $\dfrac{1}{4} < |z| < \dfrac{1}{3}$

    1.  *ROC*: $|z| < \dfrac{1}{4}$

1.  Considere la señal:

    $$x[n] = (-1)^nu[n] - \alpha^{n-n_0} u[-n-n_0]$$

    Determine las condiciones que deben cumplir el número complejo $\alpha$ y $n_0$ si la región de convergencia es $1 < |z| < 2$.

1.  Calcular todas las ROCs posibles dada la siguiente forma algebraica de una transformada Z:

    $$X(z)=\frac{1-\frac{1}{4} z^{-2}}{\left(1+\frac{1}{4} z^{-2}\right)\left(1+\frac{5}{4} z^{-1}+\frac{3}{8} z^{-2}\right)}$$

1.  Calcular la transformada inversa de la siguiente señal:

    $$X(z)=\frac{1-\frac{1}{3} z^{-1}}{\left(1-z^{-1}\right)\left(1+2 z^{-1}\right)},|z|>2$$

1.  Suponga que se conocen los siguientes 5 datos sobre una señal $x[n]$:

    -   La señal es real y de lado derecho.

    -   Su transformada Z, $X(z)$, tiene exactamente dos polos.

    -   $X(z)$ tiene dos ceros en el origen.

    -   $X(z)$ tiene un polo en $z=\frac{1}{2}e^{j\pi/3}$.

    -   $X(1) = \frac{8}{3}$.

    Determinar $X(z)$ y su región de convergencia.

1.  Considere una función $y[n]$ que está relacionada con otras dos funciones, $x_1[n]$ y $x_2[n]$ por la siguiente ecuación:

    $$y[n] = x_1[n+3] * x_2[-n+1]$$

    donde $x_1[n] = \left(\frac{1}{2}\right)^n u[n]$ y $x_2[n] = \left(\frac{1}{3}\right)^n u[n]$.

    A partir de esos datos, calcule $Y(z)$.
    
1.  La ecuación en diferencias:

    $$\left\{ \begin{array}{lcc} L_{n+2} = L_{n+1} + L_n & n \geq 0 \\ \\ L_0 = 2  \\ \\ L_1 = 1 \end{array} \right.$$
    
    puede llevarse a una forma más familar asociando $L_n=y[n]$, convirtiéndola entonces en:
    
    $$y[n+1] - y[n] - y[n-1] = -\delta[n]$$
    
    Sabiendo esto:
    
    1.  Calcule $L_{100}$.
    1.  Calcule aproximadamente $\sum_{k}^{100}L_k$


