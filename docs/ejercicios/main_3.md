# Guía 3 - Señales discretas

1.  Determine si las siguientes son señales de energía, de potencia o ninguna de las dos.

    1.  $x[n] = (-0.5)^{n} u[n]$

    1.  $x[n] = u[n]$

    1.  $x[n] = 2e^{j3n}$

    ??? "Nota"
        Para una señal discreta $x[n]$:
        
        *Energía*: $E = \sum_{k=-\infty}^{\infty} |x[k]|^2$
        
        *Potencia*: $P = \lim_{N \to \infty} \frac{1}{2N+1} \sum_{k=-N}^{N} |x[k]|^2$

1.  Dada una señal discreta $x[n]$ y su extensión periódica $y[n] = x[n+7k]$ con $k$ entero,

    $$x(n) =
      \begin{cases}
      (-1)^{n}       & \quad \text{} n \text{= 1, 2, 3}\\
      0  & \quad \text{} \text{resto}
      \end{cases}$$

    Calcular la energía y la potencia de las señales $x[n]$ e $y[n]$.

1.  Determine cuál o cuáles de las siguientes señales es periódica. Si la señal es periódica determine su período fundamental.

    1.  $x[n] = e^{j(\pi/4)n}$

    1.  $x[n] = cos \displaystyle\left(\frac{\pi}{3}n\right) + sen \left(\frac{\pi}{4}n\right)$

    1.  $x[n] = cos \displaystyle\left(\frac{n}{4}\right)$

    1.  $x[n] = cos^2 \displaystyle\left(\frac{\pi}{8}n\right)$

1.  Verificar que las siguientes funciones discretas exponenciales complejas $s_k[n]= e^{j(2\pi/N)kn}$ y $s_l[n]= e^{j(2\pi/N)ln}$ definidas en $0 \leq n < N$ son funciones ortogonales entre sí. Además, verificar numéricamente para señales de longitud $N=4$ con $k=2$ y $l=4$.

1.  Utilizando las señales exponenciales complejas del ejercicio anterior, calcular el producto interno $<s_k, s_k>$.

1.  Dada la señal continua $x(t)$, definida según:

    $$x(t) = 5sen(2\pi\;10000\;t) + cos(2\pi\;5000\;t)$$

    Grafíquela en papel, de forma aproximada, para una duración de 10 segundos. ¿Qué parámetros de $x(t)$ manejan la amplitud de la señal? ¿Y su frecuencia de oscilación?

    ¿Qué consideraciones debería tener en cuenta si quisiera llevar el gráfico hecho en papel a una computadora, mediante algún lenguaje de programación?

1.  Retomando la señal $x(t)$ del punto anterior, discretícela usando un muestreo uniforme de las siguientes características:

    1.  1000 muestras por segundo.

    1.  10000 muestras por segundo.

    1.  100000 muestras por segundo.

    Grafique las tres versiones muestreadas usando algún lenguaje de programación. Los gráficos deben ser tipo [stem](https://matplotlib.org/3.1.1/gallery/lines_bars_and_markers/stem_plot.html).

    Intuitivamente, ¿qué puede decir de los gráficos obtenidos si los compara con respecto al que hizo en el punto anterior? ¿Se parecen? ¿Afecta en algo la variación de las muestras por segundo tomadas para la discretización?.

1.  Repita los puntos 6 y 7, pero modificando $x(t)$ para que ahora sea:

    $$x(t) = 5sen(2\pi\;100\;t) + cos(2\pi\;5\;t)$$

    ¿Se modifica de alguna forma el análisis que hizo en el punto 7? ¿Qué puede concluir de esto?

1.  Tome las versiones discretizadas con 1000 muestras de las señales continuas presentadas en los puntos 6 y 8 y efectúe sobre ellas las siguientes operaciones:

    1.  Suma de ambas señales.

    1.  Resta de ambas señales.

    1.  Multiplicación de ambas por un escalar.

    1.  Producto interno entre ambas señales.
