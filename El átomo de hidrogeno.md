### El átomo de hidrogeno $\text{H}$.

Antes de empezar a estudiar las moléculas evocamos el problema del átomo de hidrogeno de mecánica cuántica. Para un núcleo con carga positiva centrado en el origen y un electrón bajo el potencial electromagnético generado por este, podemos escribir el hamiltoniano de este sistema como:

$$
\hat{H}_{\text{H}} = -\frac{\hbar}{2\mu} \nabla_r^2 - \frac{ke^2}{|\vec{r}|}
$$

Con auto-energías:

$$
E_n = - \frac{\mu e^2}{2\hbar^2} \frac{1}{n^2} \qquad n = 1, 2, 3, ...
$$

Y auto-estados son de la forma $\psi_{nlm}(r, \theta, \phi) = R_n^l(r) Y_l^m(\theta, \phi)$, en donde las funciones $Y_l^m$ son los [armónicos esféricos](https://es.wikipedia.org/wiki/Anexo:Tabla_de_arm%C3%B3nicos_esf%C3%A9ricos) y las funciones $R_n^l$ son las funciones radiales normalizadas:

$$
R_n^l(r) = \left( \frac{2}{na_0} \right) ^{3/2} \sqrt{\frac{(n-l-1)!}{2n[(n+l)!]}} e^{-\frac{r}{na_0}} r^l L^{2l+1}_{n-l-1} \left(\frac{2r}{na_0} \right)
$$

Con $a_0 = \frac{4\pi\epsilon_0 \hbar}{\mu e^2}$ el valor esperado del radio para la función de onda en su estado fundamental $\psi_{100}(r, \theta, \phi)$ y $L^{2l+1}_{n-l-1}$ los [polinomios asociados de Laguerre](https://es.wikipedia.org/wiki/Polinomios_de_Laguerre). 

Los números cuánticos de momento angular $l$  y $m$ recorren los valores $l = 0, 1, ..., n$ y $m = -l, ..., l$ . 

Las primeras funciones radiales son:

| Capa | Orbital | Función radial                                                                                                               |
| ---- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
| $K$  | $s$     | $R_{1}^{0}(r) = 2 \left( \frac{1}{a_0} \right)^{3/2} e^{-r/a_0}$                                                             |
| $L$  | $s$     | $R_2^0(r) = 2\left(\frac{1}{2a_0}\right)^{3/2} \left(1 - \frac{r}{2a_0}e^{-r/2a_0}\right)$                                   |
|      | $p$     | $R_2^1(r) = \frac{1}{\sqrt{3}}\left(\frac{1}{2a_0}\right)^{3/2}\frac{r}{a_0}e^{-r/2a_0}$                                     |
| $M$  | $s$     | $R_3^0(r) = 2 \left(\frac{1}{3a_0}\right)^{3/2}\left[1 - \frac{2r}{3a_0} + \frac{2r^2}{27a_0^2}\right]e^{-r/3a_0}$           |
|      | $p$     | $R_3^1(r) = \frac{4\sqrt{2}}{3}\left(\frac{1}{3a_0}\right)^{3/2} \frac{1}{3a_0}\left(1 - \frac{r}{6a_0} \right) e^{-r/3a_0}$ |
|      | $d$     | $R_3^2(r) = \frac{2\sqrt{2}}{27\sqrt{5}} \left(\frac{1}{3a_0}\right)^{3/2}\left(\frac{r}{a_0}\right)^2e^{-r/3a_0}$           |
