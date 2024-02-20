# Guía 7 - Transformada de Laplace

1.  Usando la ecuación de análisis, dar la transformada de Laplace de la siguiente señal:

    $$x(t) = e^{-5t}u(t-1)$$

1.  Partiendo de la siguiente señal:

    $$g(t) = A e^{-5t}u(-t-t_0)$$

    dar los valores de los parámetros $A$ y $t_0$ que hacen que la forma algebraica de la transformada de Laplace $G(s)$ sea igual a la transformada de la señal del ejercicio anterior. ¿Cómo cambia la región de convergencia con respecto a dicho ejercicio?

1.  Considere la señal:

    $$x(t) = e^{-5t}u(t) + e^{-\beta t}u(t)$$

    ¿Qué condiciones se le deben imponer a la parte real y a la parte imaginaria de $\beta$ si se desea que la región de convergencia de $X(s)$ sea $\Re{(s)} >-3$?

1.  ¿Cuántas señales temporales pueden tener la una transformada de Laplace de la siguiente forma?

    $$G(s) = \frac{(s-1)}{(s+2)(s+3)(s^2+s+1)}$$

1.  Sea $x(t)$ una señal con una transformada de Laplace racional con exactamente dos polos situados en $s=-1$ y $s=-3$. Si $g(t) = e^{2t}x(t)$ y $G(j\omega)$ converge, determinar si $x(t)$ es de lado izquierdo, derecho o si es una composición de señales de ambos lados.

1.  Determinar la transformada inversa de Laplace de la siguiente señal:

    $$X(s) = \frac{2(s+2)}{s^2+7s+12},\;\Re{(s)}>-3$$

1.  Sea:

    $$g(t) = x(t) + \alpha x(-t)$$

    donde:

    $$x(t) = \beta e^{-t}u(t)$$

    y la transformada de Laplace de $g(t)$ es:

    $$G(s) = \frac{s}{s^2-1},\;-1<\Re{(s)}<1$$

    determinar los valores de las constantes $\alpha$ y $\beta$.

1.  Supongamos que sabemos la siguiente información sobre una señal $x(t)$ con transformada de Laplace $X(s)$:

    -   $x(t)$ es real y par.

    -   $X(s)$ tiene cuatro polos y ningún cero.

    -   $X(s)$ tiene un polo en $s=\frac{1}{2}e^{j\pi /4}$.

    -   $\int_{-\infty}^{\infty}x(t)dt = 4$.

    Determinar $X(s)$.

    ??? "Pista"
        Si $x(t)$ es real y tiene algún polo complejo, tiene que aparecer su conjugado.

1.  Supongamos tener dos señales $x(t)$ e $y(t)$ relacionadas por las siguientes ecuaciones diferenciales:

    $$\frac{dx(t)}{dt} = -2y(t) + \delta(t)$$

    $$\frac{dy(t)}{dt} = 2x(t)$$

    Determinar $X(s)$ e $Y(s)$, y sus respectivas regiones de convergencia.
    
1.  Hallar una función $f: \mathbb{R} \rightarrow \mathbb{R}$ que cumpla las siguientes condiciones:

    -  $f(t) = 0 \forall t<0$
    -  $||f(t)||_2 = 18$
    -  $F(s)$, su transformada de Laplace, es una función racional.
    -  $\lim_{s\rightarrow-2} F(s) = \infty$
    -  $|F(S)| \neq 0 \; \forall s \in \{z \in \mathbb{C} | \Re(z) > -2\}$
    
    Una vez que encuentre $f(t)$, de una segunda función distinta que también cumpla con las condiciones propuestas.
