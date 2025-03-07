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

