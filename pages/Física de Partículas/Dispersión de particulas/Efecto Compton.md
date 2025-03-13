El efecto Compton (o dispersión Compton) consiste en el aumento de la longitud de onda de un fotón cuando choca con un electrón libre y pierde parte de su energía. 

Este proceso puede escribirse como $e^- + \gamma \rightarrow e^- + \gamma$.  Escribamos sus $4$-momentos desde un marco de referencia para el cual la $3$-velocidad inicial del electrón es nula y el fotón viaja sobre el eje $z$.

$$
p_1 = (m_ec, \vec{0}) \quad p_2 = (\frac{\hbar \omega}{c},0,0, \frac{\hbar \omega}{c}) \quad p_3 = (\frac{E}{c}, \vec{p}) \quad p_4 = (\frac{\hbar \omega'}{c}, \hbar \vec{k})
$$

Como el fotón no tiene masa, el factor de flujo se reduce a $4(p_1\cdot p_2) = 4m_ec \hbar\omega$ . Luego la sección transversal será:

$$ 
\begin{aligned}
\sigma = \frac{\hbar^2 S}{4m_ec \hbar\omega}\int(2\pi)^4|\mathcal{M}|^2 \delta^4(p_1+p_2-p_3-p_4) \\
\times 2 \pi \delta(p_3^2 - m_e^2c^2)\theta(p^0_3) 2 \pi \delta(p_4^2)\theta(p^0_4) \frac{d^4p_3}{(2\pi)^4} \frac{d^4p_4}{(2\pi)^4}
\end{aligned}
$$

$$ 
\begin{aligned}
\sigma = \frac{\hbar S}{4\omega m_e} \frac{1}{(2\pi)^2} \int |\mathcal{M}^2| \delta(m_ec + \hbar \omega/c -p_3^0 -p_4^0) \delta^3(\hbar \omega/c\vec{z} - \vec{p} -\hbar \vec{k}) \\
\times \frac{\delta(p^0_3-\sqrt{|\vec{p}|^2+m_e^2c^2})}{2\sqrt{|\vec{p}|^2+m_e^2c^2}} \frac{\delta(p_4^0-\hbar|\vec{k|})}{2 \hbar|\vec{k|}} d^4p_3 d^4p_4
\end{aligned}
$$

$$ 
\sigma = \left(\frac{1}{8\pi} \right)^2 \frac{\hbar S}{\omega m_e} \int |\mathcal{M}|^2 \frac{\delta(m_ec + \hbar \omega/c - \sqrt{|\vec{p}|^2+m_e^2c^2} - \hbar |\vec{k}|)}{\hbar |\vec{k}| \sqrt{|\vec{p}|^2+m_e^2c^2}} \delta^3(h/\lambda \hat{z} - \vec{p}-\hbar \vec{k}|) d^3\vec{p} d^3( \hbar\vec{k})
$$
Analicemos la delta de Dirac restante. Sea $\theta$ el ángulo entre el eje $z$ y la dirección para la cual el electrón sale dispersado.

$$
\hbar \vec{k} + \vec{p} = \frac{\hbar \omega}{c} \hat{z} \Rightarrow |\vec{p}| = \hbar \sqrt{\left(\frac{\omega}{c}\right)^2+ |\vec{k}|^2 -2\frac{\omega}{c}|\vec{k}| \cos\theta}
$$

Podemos escribir la energía resultante del electrón como:

$$ 
\sqrt{|\vec{p}|^2+m_e^2c^2} = \hbar  \sqrt{\left(\frac{\omega}{c}\right)^2 + \left(\frac{m_ec}{\hbar}\right)^2+ |\vec{k}|^2 -2\frac{\omega}{c}|\vec{k}| \cos\theta} 
$$

Tomando $u = \sqrt{|\vec{p}|^2+m_e^2c^2} + \hbar |\vec{k}|$ y reemplazando lo anterior:

$$
u = \hbar  \sqrt{\left(\frac{\omega}{c}\right)^2 + \left(\frac{m_ec}{\hbar}\right)^2+ |\vec{k}|^2 -2\frac{\omega}{c}|\vec{k}| \cos\theta}  + \hbar |\vec{k}|
$$

Derivando sobre el ángulo solido $\Omega$, la integral queda solo en términos del modulo $|\vec{k}| \equiv k$. Reemplazando $u$ en la integral:

$$\frac{d\sigma}{d\Omega} = \left(\frac{1}{8\pi}\right)^2 \frac{\hbar S}{\omega m_e} |\mathcal{M}|^2 \int_0^{\infty} \frac{\delta(m_ec + \hbar \omega/c - u)}{\hbar k  (u-\hbar k)} (\hbar k)^2 d(\hbar k)$$

Derivando $u$ sobre $\hbar k$:

$$ 
\frac{d u}{d (\hbar k)} = \frac{\hbar k- \hbar \frac{\omega}{c} \cos \theta}{\hbar \sqrt{\left(\frac{\omega}{c}\right)^2 + \left(\frac{m_ec}{\hbar}\right)^2+ k^2 -2\frac{\omega}{c}k \cos\theta}}  + 1 = \frac{u - \hbar \frac{\omega}{c} \cos\theta}{u - \hbar k}
$$

Reemplazando en la integral $d(\hbar k)$ por $d u$:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{1}{8\pi}\right)^2 \frac{\hbar S}{\omega m_e} |\mathcal{M}|^2 \int_0^{\infty} \frac{\delta(m_ec + \hbar \omega/c - u)}{ u - \hbar \frac{\omega}{c} \cos\theta} \hbar k du
$$

Integrando sobre la delta Dirac podemos hallar que:

$$ 
u = m_ec + \hbar \frac{\omega}{c} = \hbar  \sqrt{\left(\frac{\omega}{c}\right)^2 + \left(\frac{m_ec}{\hbar}\right)^2+ k^2 -2\frac{\omega}{c}k \cos\theta}  + \hbar k \\
$$

$$
\left(\frac{m_ec}{\hbar}+\frac{\omega}{c} - k \right )^2 = \left(\frac{\omega}{c}\right)^2 + \left(\frac{m_ec}{\hbar}\right)^2+ k -2\frac{\omega}{c}k \cos\theta
$$

$$
\frac{m_e \omega}{\hbar}  \hbar c = (\frac{\omega}{c}k + \frac{m_e c}{\hbar}k -\frac{\omega}{c}k \cos\theta) \hbar c
$$

$$ 
k = \frac{m_ec \omega}{\hbar \omega(1-\cos\theta) + m_e c^2} $$

Podemos finalmente reemplazara en la sección eficaz diferencial este valor de $k$ con $S = 1$ y obtenemos:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar c}{8\pi}\right)^2 \frac{|\mathcal{M}|^2}{\left[ \hbar \omega(1-\cos\theta) + m_e c^2 \right]^2}
$$

Nos queda ahora hallar la amplitud de dispersión $\mathcal{M}$. Notemos que para este proceso tenemos dos diagramas de Feynman posibles.

![Efecto Compton](../../assets/20250226010357.png)

Utilizando la regla de Feynman con el propagador para fermiones $\frac{\gamma^{\lambda}q_{\lambda} + mc}{q^2-m^2c^2}$, con el termino de conservación $\delta^4(p_1-q-p_3)$ en el primer diagrama y $\delta^3(p_1 + p_2 - q)$ obtenemos las amplitudes:

$$ 
\mathcal{M}_1 = \frac{-g_e^2}{(p_1-p_3)^2-m_e^2c^2} \bar{u}_4 \cancel{\epsilon_2}(\cancel{p_1}-\cancel{p_3}+m_ec) \cancel{\epsilon_3^*}u_1
$$

$$ 
\mathcal{M}_2 = \frac{-g_e^2}{(p_1+p_2)^2-m_e^2c^2} \bar{u}_4 \cancel{\epsilon_3^*} (\cancel{p_1}+\cancel{p_2}+m_ec)\cancel{\epsilon_2} u_1
$$