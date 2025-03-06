La desintegración alfa esta asociada con núcleos pesados e inestables, y es raramente observada en especies con número atómico $Z < 82$. La partícula emitida es un fragmento nuclear cuatro veces más masivo que un protón.

El proceso de emisión de fragmentos con $A = 4$, es más favorable en términos energéticos que otros procesos, de modo que estos procesos tienden a prevalecer sobre la emisión de otros fragmentos más pesados.

Los fragmentos $\alpha$ emitidos, se encuentran junto con el residuo de la desintegración unido por la fuerza nuclear fuerte, pero al mismo tiempo repelidos por la energía electromagnética, la cual contribuye a la probabilidad de desintegración. 

La típica desintegración alfa $X \rightarrow Y + \alpha$ inicia en el estado fundamental del estado base $X$. Es posible también observar emisiones provenientes de un estado excitado $X^*$, es decir el proceso $X^* \rightarrow Y + \alpha$, resultando en estos casos, partículas alfas con energía mayor. Este último proceso es menos frecuentes debido a que debe competir con el proceso favorable $X^* \rightarrow X + \gamma$.

El proceso de emisión $\alpha$ se dice **mono-energético**, debido a que cada partícula $\alpha$ de un proceso es emitido con la misma energía $K_{\alpha}$, la cual generalmente se encuentra entre los $4$ y $9$ $\text{MeV}$.

### Conservación de la energía

Aplicando la ley de conservación de la energía al proceso:

$$ 
^A_Z X \rightarrow ^{A-4}_{Z-2} Y + ^4_2 \text{He} 
$$

Suponiendo el núcleo base $X$ en reposo, el producto del proceso se puede modelar como un problema de dos cuerpos. La partícula $\alpha$ emitida y el residuo $Y$, tienen momentos opuestos de igual magnitud. En términos de energía relativista, esto es:

$$ 
M_X c^2 = M_Y c^2 + K_Y + M_{\alpha} c^2 + K_{\alpha} 
$$

$$ 
\Rightarrow M(^A_Z X) c^2 =\left[ M(^A_Z X) - M(^{A-4}_Z Y) - M(^4 \text{He}) \right] c^2 + K_Y + K_{\alpha} 
$$

Esta ultima ecuación define un criterio de estabilidad para los núcleos. Se dice entonces que, *un núcleo $X$ es $\alpha$-inestable, y puede sufrir una desintegración $X \rightarrow Y$ + $\alpha$ si y solo si, la masa del núcleo $X$ excede la suma de las masas de los productos $Y$ y $\alpha$*. Dicho esto, se define la *$\alpha$-energía de desintegración*, o *$Q$-valor* para la desintegración como:

$$ 
Q = \left[ M(^A_Z X) - M(^{A-4}_Z Y) - M(^4 \text{He}) \right] c^2 
$$

Esta cantidad representa el total de la energía liberada por las partículas resultantes. Debido a la conservación del momento lineal, el momento $p$ de ambos productos debe ser iguales, y pueden ser escritos en términos de energías cinéticas no relativistas:

$$ 
Q = K_Y + K_{\alpha} = \frac{p^2}{2M_{\alpha}} + \frac{p^2}{2M_{Y}}  = \frac{p^2}{2M_{\alpha}} \left( 1 + \frac{M_{\alpha}}{M_Y} \right) = K_{\alpha} \left( 1 + \frac{M_{\alpha}}{M_Y} \right) 
$$

Notemos que las energías relativistas fueron necesarias para el cálculo de la energía total debido a que las energías en reposo, ya que cambian con las identidades de las partículas, mientras que las energías cinéticas pueden ser calculadas con fórmulas clásicas, ya que son mucho menores que las energías en reposo.
### Conservación del momento angular
  
Otra ley de conservación que juega un rol en el estado final del sistema es la conservación del momento angular. Sean $\vec{I}_X$ y $\vec{I}_Y$ los espines de los núcleos $X$ e $Y$ respectivamente. La partícula $\alpha$ tiene espín nulo. Luego el momento angular del sistema será:

$$
\vec{I}_X = \vec{I}_Y + \vec{L} 
$$

Del problema de adición de momentos, se pueden obtener cotas para los números cuánticos:

$$
|i_X - i_Y| \leq l \leq i_X + i_Y
$$

Los estados nucleares $X$ e $Y$ también están dotados con paridad definida, en sus números 
cuánticos. La paridad final del sistema estada dada por $(-1)^l$ y se puede concluir que $l$ debe ser par si $X$ e $Y$ tienen la misma paridad e impar si $X$ e $Y$ tienen paridad distintas.
### Ejemplo

El espectro de las partículas alfa emitidas en el decaimiento del $^{228}_{90}\text{Th}$ presenta dos líneas principales, una ubicada en $5,341 \text{MeV}$ y otra en $5,423 \text{MeV}$. La de mayor energía corresponde a transiciones hacia el estado fundamental del núcleo hijo, mientras que la de menor energía a transiciones hacia el estado excitado del núcleo hijo, desde el cual luego decae hacia su estado fundamental por emisión de radiación gamma.  

Calculemos la energía liberada en el decaimiento y justificar las aproximaciones realizadas y la energía del fotón gamma. Podemos describir el proceso como:

$$ 
^{228}_{90} \text{Th} \rightarrow ^{224}_{88} \text{Ra} + ^4_2 \text{He} 
$$

Usando la conservación del momento y teniendo en cuenta los electrones de los átomos en ambos miembros, se puede hallar que:

$$ 
M(^{228}_{90} \text{Th}) c^2 = M(^{224}_{88} \text{Ra}) c^2 + K_{\text{Ra}} + M(^4_2 \text{He}) c^2 + K_{\alpha} 
$$

La energía liberada en la desintegración será entonces igual al valor de la energía en reposo del $\text{Th}$ menos las energías en reposo de los productos, es decir:

$$ 
Q \equiv \left[ M(^{228}_{90} \text{Th}) - M(^{224}_{88} \text{Ra}) -  M(^4_2 \text{He}) \right]c^2 = K_{\text{Ra}} + K_{\alpha} 
$$

Debido a que la energía en reposo de los núcleos es mucho mayor que la energía cinética, se puede aproximar de forma clásica:

$$ 
\Rightarrow Q = K_{\text{Ra}} + K_{\alpha} = \frac{p^2}{2 M_{\text{Ra}}} + \frac{p^2}{2  M_{\alpha}} = K_{\alpha} \left( 1 + \frac{M_{\alpha}}{M_{\text{Ra}}} \right)
$$

Finalmente, la energía liberada en la reacción será:

$$ 
Q \approx 5.423 \left(1 + \frac{4}{228} \right) \text{MeV} = 5.518 \text{MeV}
$$

Analicemos ahora la desintegración:

$$ 
^{228}_{90} \text{Th} \rightarrow ^{224}_{88} \text{Ra}^* + ^4_2 \text{He} \rightarrow ^{224}_{88} \text{Ra} + ^4_2 \text{He} + \gamma 
$$

Usando las leyes de conservación, en donde la partícula $\alpha'$ es la partícula emitida de menor energía en el espectro.

$$ 
M(^{228}_{90} \text{Th}) c^2 = M(^{224}_{88} \text{Ra}) c^2 + K_{\text{Ra}} + M(^4_2 \text{He}) c^2 + K_{\alpha'} + K_{\gamma} 
$$

$$ 
\Rightarrow \left[M(^{228}_{90} \text{Th}) c^2 - M(^{224}_{88} \text{Ra}) c^2 -M(^4_2 \text{He}) \right] = Q = K_{\text{Ra}} +  K_{\alpha'} + K_{\gamma}
$$

$$ 
\Rightarrow K_{\gamma} = Q - K_{\alpha'}\left( 1 + \frac{M_{\alpha}}{M_{\text{Ra}}} \right) = (K_{\alpha} - K_{\alpha'})\left( 1 + \frac{M_{\alpha}}{M_{\text{Ra}}} \right)
$$

Y la energía del fotón gamma emitido luego de la desintegración al estado excitado será:

$$ 
\Rightarrow K_{\gamma} \approx (5.423 - 5.341)\left( 1 + \frac{4}{224} \right) \text{MeV} = 0.083 \text{MeV}
$$

### Ejemplo

Encontremos la energía liberada en el decaimiento $\alpha$ del $^{247}\text{Bk}$, usando las masas de los isotopos:

- $M(^{247}\text{Bk}) = 247.070307 \text{u}$

- $M(^{243}\text{Am}) = 243.0613811 \text{u}$

- $M(^{4}\text{He}) = 4.002602 \text{u}$

El proceso de desintegración puede escribirse como:

$$ 
^{247}_{97} \text{Bk} \rightarrow ^{243}_{95}\text{Am} +  ^4_2\text{He}
$$

Utilizando las leyes de conservación:

$$ 
\left[M(^{247}_{97} \text{Bk}) - M(^{243}_{95}\text{Am}) - M(^4_2\text{He}) \right] c^2 \equiv Q = K_{\alpha} + K_{\text{Am}} 
$$

Debido a que las energías en reposo son mucho mayores que las energías cinéticas de los productos, se puede escribir de forma clásica:

$$ 
Q = K_{\alpha} + K_{\text{Am}} = \frac{p^2}{2M_{\alpha}} + \frac{p^2}{2M_{\text{Am}}} = K_{\alpha} \left(1 + \frac{M_{\alpha}}{M_{\text{Am}}} \right) \approx  K_{\alpha} \left(1 + \frac{4}{243} \right)
$$

Hallemos también la energía cinética y la velocidad de la partícula $\alpha$ y del núcleo residual, y analicemos la vida media del $^{247}\text{Bk}$. La partícula alfa será:

$$
K_{\alpha} \approx Q \left(1 - \frac{4}{243} \right) = (247.07031 - 243.061381 - 4.00260) \left(1 - \frac{4}{243} \right) \times 931.5 \text{MeV}$$

$$
K_{\alpha} = 5.79 \text{MeV} 
$$

Por otra parte de la energía cinética, se obtiene que:

$$ 
K_{\alpha} = \frac{p^2}{2M_{\alpha}} = \frac{1}{2} M_{\alpha} v_{\alpha}^2 \Rightarrow v_{\alpha} = \sqrt{\frac{2 K_{\alpha}}{M_{\alpha}}} \approx \sqrt{\frac{2 \times 5.79}{4 \times 931.5}c^2} \approx 0.05 c 
$$

Luego la partícula $\alpha$ emitida tendrá una velocidad igual al $5 \%$ de la velocidad de la luz. La velocidad del núcleo de $\text{Am}$ se puede calcular usando la conservación del momento lineal.

$$ 
p_{\alpha} = p_{\text{Am}} \Rightarrow v_{\text{Am}} \approx \frac{4}{243} v_{\alpha} \approx 4.12 \times 10 ^{-5}  c
$$

Mucho mas pequeña que la velocidad de la partícula alfa. Esto se debe a que el núcleo de $\text{Am}$ es mucho mas pesado. 

El radio nuclear de una especie, se relaciona con su numero de masa de la siguiente forma:

$$
R = R_0 A^{1/3} \qquad R_0 \approx 1,2\text{fm}
$$

Podemos expresar entonces la distancia entre la partícula $\alpha$ y el núcleo de $\text{Am}$ antes de la desintegración en el núcleo de $\text{Bk}$ como:

$$
R = 1.2\text{fm}(4^{1/3} + 243^{1/3}) = 9.39 \text{fm}
$$

La interacción colombiana entre la partícula $\alpha$ y el núcleo de $\text{Am}$ será de:   

$$ 
V(R) = - \frac{ke^2Z_{\alpha} Z_{\text{Am}}}{R}
$$

