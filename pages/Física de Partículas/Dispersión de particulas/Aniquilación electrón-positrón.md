Consideremos el proceso de aniquilación de pares: $e^+ + e^- \rightarrow \gamma + \gamma$  con el marco de referencia en el centro de masa. Proponemos los $4$-momentos el par $e^+$ y $e^-$.

$$
p_1 = (\frac{E_1}{c}, \vec{p}) \qquad p_2 = (\frac{E_2}{c}, -\vec{p})
$$

Hallemos el factor de flujo de la sección transversal:

$$ 
p_1\cdot p_2 = \frac{E_1 E_2}{c^2} + |\vec{p}| \Rightarrow \sqrt{(p_1\cdot p_2)^2 - (m_ec)^4} = \frac{E_1 + E_2}{c} |\vec{p}|
$$

Reemplazando en la sección transversal $\sigma$:

$$
\begin{aligned}
\sigma = \frac{c \hbar^2 S}{4(E_1+E_2)|\vec{p}|} \int (2\pi)^4|\mathcal{M}|^2 \delta^4(p_1+p_2-p_3-p_4) \delta^3(\vec{p}_3+\vec{p}_4) \\
\times 2\pi \delta(p_3^2)\theta(p^0_3) 2\pi \delta(p_4^2)\theta(p^0_4) \frac{d^4p_3}{(2\pi)^4} \frac{d^4p_4}{(2\pi)^4}
\end{aligned}
$$

$$ 
\begin{aligned}
\sigma = \left( \frac{\hbar c}{4\pi} \right)^2 \frac{S}{(E_1 + E_2)c|\vec{p}|} \int |\mathcal{M}|^2 \delta(\frac{E_1 + E_2}{c} -p^0_3 - p_4^0) \delta^3(\vec{p}_3 + \vec{p}_4) \\
\times \frac{\delta(p^0_3-|\vec{p}_3|)}{2|\vec{p}_3|} \frac{\delta(p^0_4-|\vec{p}_3|)}{2|\vec{p}_4|} d^4p_3 d^4p_4
\end{aligned}
$$

$$
\sigma = \left( \frac{\hbar c}{8\pi} \right)^2 \frac{S}{(E_1 + E_2)c|\vec{p}|} \int |\mathcal{M}|^2 \frac{\delta(\frac{E_1 + E_2}{c} - |\vec{p}_3| - |\vec{p}_4)}{|\vec{p}_3| |\vec{p}_4|}\delta^3(\vec{p}_3 + \vec{p}_4) d^3\vec{p}_3 d^3\vec{p}_4
$$

Integrando sobre $\vec{p}_4$ se obtiene que $|\vec{p}_4| = |\vec{p}_3| \equiv E_f/c$. Derivando sobre el ángulo solido $\Omega$, nos queda una integral en términos de $|\vec{p}_3|^2d|\vec{p}_3| = E_f^2 dE_f/c^3$. Reemplazando:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar c}{8\pi}\right)^2 \frac{S |\mathcal{M}|^2}{(E_1 + E_2)c |\vec{p}|} \int\frac{c\delta(\frac{E_1+E_2}{2}-E_f)/2}{E_f^2/c^2} E_f^2dE_f/c^3
$$

Finalmente, como en los productos se repite el fotón dos veces, $S = 1/2$, entonces, la sección eficaz diferencial será:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar c}{16\pi}\right)^2 \frac{|\mathcal{M}|^2}{(E_1 + E_2)c |\vec{p}|} 
$$

Nos queda hallar la amplitud $\mathcal{M}$. Notemos que hay dos diagramas de Feynman posibles para este proceso. Esto se debe a que los fotones emitidos son indistinguibles. 

![Aniquilación electrón positrón](../../assets/20250226005328.png)

Utilizando la regla de Feynman con el propagador para fermiones $\frac{\gamma^{\lambda}q_{\lambda} + mc}{q^2-m^2c^2}$, con el termino de conservación $\delta^4(p_1-q-p_3)$ para el primer diagrama y $\delta^4(p_1-q-p_4)$ en el segundo:

$$ 
\mathcal{M}_1 = \frac{-g_e^2}{(p_1-p_3)^2-m_e^2c^2} \bar{v}_2 \cancel{\epsilon_4}^*(\cancel{p_1}-\cancel{p_3}+m_ec) \cancel{\epsilon_3}^*u_1
$$

$$ 
\mathcal{M}_2 = \frac{-g_e^2}{(p_1-p_4)^2-m_e^2c^2} \bar{v}_2 \cancel{\epsilon_3}^*(\cancel{p_1}-\cancel{p_4}+m_ec) \cancel{\epsilon_4}^*u_1
$$

Luego, la amplitud $\mathcal{M}$ será la suma de las amplitudes, es decir:

$$
\mathcal{M} = \mathcal{M}_1 + \mathcal{M}_2 
$$

Para hallar la amplitud, supongamos las partículas con una velocidad $v << c$, es decir aproximamos ambos, el electrón y el positrón como en reposo. Luego podemos elegir la dirección del eje $z$ como la dirección en la cual los fotones fueron emitidos. Escribimos entonces los momentos como:

$$
p_1 = (m_ec, \vec{0}) \qquad p_2 = (m_ec, \vec{0})\qquad  
p_3 = (\frac{\hbar\omega}{c},0,0,\frac{\hbar\omega}{c}) \qquad  p_4 = (\frac{\hbar\omega}{c},0,0,-\frac{\hbar\omega}{c}) 
$$

Para ambas contribuciones, los denominadores se expresan en términos de las diferencias $p_1 - p_3$ y  $p_1 - p_4$. Reemplazando los $4$-momentos con la aproximación anterior:

$$
p_1 - p_3 = (m_ec - \frac{\hbar \omega}{c},0,0,-\frac{\hbar \omega}{c}) \Rightarrow (p_1 - p_3)^2 =  (m_ec)^2 - 2\frac{\hbar \omega}{c}m_ec 
$$

$$
p_1 - p_4 = (m_ec - \frac{\hbar \omega}{c},0,0,+\frac{\hbar \omega}{c}) \Rightarrow (p_1 - p_4)^2 =  (m_ec)^2 - 2\frac{\hbar \omega}{c}m_ec 
$$

Ambos denominadores son iguales. Reemplazando, encontramos la constante que acompaña a $\mathcal{M}$ en términos de la constante hiperfina:

$$
\mathcal{M} \sim \frac{g_e^2}{2\hbar \omega m_e} = \frac{2\pi\alpha}{\hbar \omega m_e} = \frac{2\pi e^2}{\hbar^2 \omega m_ec}
$$
Veamos ahora los términos que se encuentran entre los espinores $\bar{v}$ y $u$. Notemos que aplicando el teorema de trazas a una polarización $\cancel{\epsilon}^*$ y un momento $\cancel{p}$ obtenemos que, por la condición de Coulomb:

$$
\cancel{\epsilon}^*\cancel{p} + \cancel{p} \cancel{\epsilon}^* = 2 \epsilon^* \cdot p = 0 \Rightarrow \cancel{\epsilon}^*\cancel{p} = -\cancel{p} \cancel{\epsilon}^*
$$

Luego, se puede simplificar usando la condición de onda plana para un espinor $u$, es decir $(\gamma^{\mu}p_{\mu} - mc)u = 0$. Veamos esto para ambas amplitudes $\mathcal{M}_1$ y $\mathcal{M}_2$:

$$
\cancel{\epsilon_4}^*(\cancel{p_1}-\cancel{p_3}+m_ec) \cancel{\epsilon_3}^*u_1 = \cancel{\epsilon_4}^* \cancel{\epsilon_3}^* (\cancel{p_1}-\cancel{p_3}+m_ec) u_1
= \cancel{\epsilon_4}^* \cancel{\epsilon_3}^* \cancel{p_3} u_1$$

$$  
\cancel{\epsilon_3}^*(\cancel{p_1}-\cancel{p_4}+m_ec) \cancel{\epsilon_4}^*u_1 = 
\cancel{\epsilon_3}^*  \cancel{\epsilon_4}^*(\cancel{p_1}-\cancel{p_4}+m_ec)u_1 
= \cancel{\epsilon_3}^* \cancel{\epsilon_4}^* \cancel{p_4} u_1
$$

Reemplazando en la amplitud $\mathcal{M}$ obtenemos la expresión:

$$
\mathcal{M} = \frac{2\pi e^2}{\hbar^2 \omega m_ec} \bar{v}_2(\cancel{\epsilon_4}^* \cancel{\epsilon_3}^*\cancel{p_3}  + \cancel{\epsilon_3}^*  \cancel{\epsilon_4}^* \cancel{p_4})u_1
$$
