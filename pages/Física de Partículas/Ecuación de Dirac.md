La ecuación de Dirac, es una ecuación de primer orden, que describe partículas de spin $1/2$. Esta es consistente con los principios de la mecánica cuántica y la relatividad y es esencial para construir el modelo estándar.

Supongamos una partícula de masa $m$ y un $4$-momento $p$. Sabemos que la magnitud de $4$-momento se conserva, luego:

$$
(p \cdot p ) = m^2 c^2 \Rightarrow p^{\mu}p_{\mu} - m^2c^2 = 0
$$

En donde las componentes $p_{\mu}$ del $4$-momento se puede sustituir por sus respectivos operadores cuánticos, es decir:

$$
p_{\mu} \rightarrow -i\hbar \partial_{\mu}
$$

Como buscamos una ecuación de primer orden, proponemos coeficientes $\gamma^{\mu}$ a fines de factorizar la primera ecuación y expresarla en términos de las componentes covariantes del momento, es decir:

$$ 
p^{\mu}p_{\mu} - m^2c^2 = (\gamma^{\mu}p_{\mu}-mc)(\gamma^{\nu}p_{\nu}+mc) = 0
$$

La ecuación anterior requiere que.

$$
\gamma^{\mu} \gamma^{\nu}p_{\mu} p_{\nu} = p^{\mu} p_{\mu} \qquad \gamma^{\mu} \gamma^{\nu} +  \gamma^{\nu} \gamma^{\mu} = 0 \quad \text{si} \quad \mu\neq \nu
$$

Podemos escribir estos requisitos en términos del anti-conmutador y el tensor métrico $g^{\mu \nu}$ :

$$
\gamma^{\mu} \gamma^{\nu} +  \gamma^{\nu} \gamma^{\mu} = \{ \gamma^{\mu},\gamma^{\nu} \} = 2g^{\mu \nu}
$$

Los coeficientes que verifican esta relación son matrices $4\times4$ y se denominan matrices de Dirac. Estas pueden en términos de las matrices de Pauli $\{\hat{\mathbb{I}}, \hat{\sigma}_1, \hat{\sigma}_2, \hat{\sigma}_3 \}$.

$$
\gamma^{0} = \begin{pmatrix}
\hat{\mathbb{I}} & 0 \\
0 & -\hat{\mathbb{I}}
\end{pmatrix}
\qquad
\gamma^{\mu} = \begin{pmatrix}
0 & \hat{\sigma}_{\mu} \\
\hat{\sigma}_{\mu} & 0 \\
\end{pmatrix}
$$

Por otra parte las funciones de onda que satisfacen esta ecuación se denominan *espinores de Dirac* y son de la forma:

$$
\psi = \begin{pmatrix} \psi^1 \\ \psi^2 \\ \psi^3 \\ \psi^4 \end{pmatrix}
$$

Finalmente podemos escribir la ecuación de Dirac, para un espinor $\psi$ como:

$$ 
i\hbar \gamma^{\mu} \partial_{\mu} \psi -mc\psi = 0
$$

### Evolución temporal

Ignoremos por un momento las componentes $1, 2, 3$ del $4$-momento $p$ que corresponden a las coordenadas espaciales de la partícula y analicemos que ocurre con la componente $0$, es decir:

$$ 
i\hbar \gamma^0 \frac{1}{c} \frac{\partial}{\partial t} \psi - mc\psi = 0
$$

En donde $\gamma^{0} = \begin{pmatrix}\hat{\mathbb{I}} & 0 \\0 & -\hat{\mathbb{I}}\end{pmatrix}$ y $\psi$ el espinor que puede dividirse en dos componentes  $\psi = \begin{pmatrix} \psi_A \\ \psi_B \end{pmatrix}$ , de forma que:

$$
\frac{\partial}{\partial t} \psi_A = -i\frac{mc^2}{\hbar} \psi_A \qquad \frac{\partial}{\partial t} \psi_B = i\frac{mc^2}{\hbar} \psi_B
$$
Luego las componentes del espinor evolucionan como:

$$ \psi_A \sim e^{-i\frac{mc^2}{\hbar}t} \qquad \psi_B \sim e^{i\frac{mc^2}{\hbar}t}$$
Dado a que el factor $mc^2$ es la energía en reposo de la partícula, la función de onda evoluciona como $\psi_A \sim e^{-i\frac{E}{h}t}$, lo cual implica propagación hacia el futuro en el tiempo y no implica ninguna inconsistencia, sin embargo, la ecuación de Dirac también admite soluciones de la forma $\psi_B \sim e^{i\frac{E}{\hbar}t}$, las cuales a primera instancia parecerían una violación de la causalidad. Estas soluciones en realidad corresponden a las *anti-partículas*, las cuales son las mismas partículas pero con carga opuestas, y pueden interpretarse en la electrodinámica cuántica como una antipartícula con energía positiva propagándose en la dirección opuesta en el espacio-tiempo  

### Ondas planas 

Supongamos ahora soluciones en forma de ondas planas, es decir: 

$$ 
\psi(x) = u(k) a e^{-ik\cdot x} 
$$

Notemos que la ecuación de Dirac se reduce a:

$$
(\hbar \gamma^{\mu} k_{\mu} - mc) u(k) = 0
$$

Notemos que la suma $\gamma^{\mu} k_{\mu}$ puede escribirse como:

$$
\gamma^{\mu} k_{\mu} = \gamma^0k_0 - \vec{\gamma}\cdot\vec{k} = k^0 \begin{pmatrix} \hat{\mathbb{I}} & 0 \\ 0 & -\hat{\mathbb{I}} \end{pmatrix} - \vec{k} \cdot \begin{pmatrix}  0 & \vec{\sigma} \\ -\vec{\sigma} & 0 \end{pmatrix} =
\begin{pmatrix} k^0\hat{\mathbb{I}} & -\vec{k} \cdot \vec{\sigma} \\ \vec{k} \cdot \vec{\sigma}  &  -k^0\hat{\mathbb{I}} \end{pmatrix}
$$
Luego la ecuación de onda se reduce a:

$$
\begin{pmatrix} \hat{\mathbb{I}}(\hbar k^0 - mc) & -\hbar \vec{k} \cdot \vec{\sigma} \\ \hbar \vec{k} \cdot \vec{\sigma} &  -\hat{\mathbb{I}}(\hbar k^0 + mc) \end{pmatrix} \begin{pmatrix} u_A \\ u_B\end{pmatrix} = 0
$$
En donde las componentes $u_A$ y $u_B$ corresponden a las partículas y anti-partículas respectivamente. Luego:

$$
u_A = \frac{(\vec{k}\cdot \vec{\sigma})}{k^0 - mc/\hbar} u_B \qquad u_B = \frac{(\vec{k}\cdot\vec{\sigma})}{k^0 + mc/\hbar} u_A
$$

Se puede probar que las componentes de $4$-vector $k$ se corresponden a las del $4$-momento $p$ como $k^{\mu} = \pm p^{\mu}/\hbar$. Para ello reemplacemos una ecuación en otra, es decir:

$$ 
u_A = \frac{(\vec{k}\cdot \vec{\sigma})^2}{k_0^2 - (mc/\hbar)^2} u_A
$$

En donde:

$$ 
\vec{k}\cdot\vec{\sigma} = k_x \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} + k_y\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} + \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} k_z & k_x - ik_y \\ k_x + ik_y & -k_z \end{pmatrix}
$$

$$ 
\Rightarrow (\vec{k} \cdot \vec{\sigma})^2  = \begin{pmatrix} k_z & k_x - ik_y \\ k_x + ik_y & -k_z \end{pmatrix}^2 = \begin{pmatrix} k_x^2 + k_y^2 + k_z^2 & 0 \\0 &  k_x^2 + k_y^2 + k_z^2 \end{pmatrix} = |\vec{k}|^2
$$

Reemplazando en $u_A$, tendremos que:

$$|\vec{k}|^2 = k_0^2 - (mc/\hbar)^2 \Rightarrow \hbar^2(k \cdot k) = m^2c^2$$

Esto nos dice que el vector de onda se conserva en el espacio-tiempo y que necesariamente $\hbar k = \pm p$. Esto es importante ya que nos permite expresar los espinores en términos del $4$-momento $p$ de la partícula. 

Podemos ahora hallar una base para el conjunto de ondas planas soluciones a la ecuación de Dirac. Para ello elegimos una basa para las componentes correspondientes a las partículas y hallamos las componentes correspondientes a las anti-partículas en función de estas.
 
$$
u_A^{(1)} = \begin{pmatrix} 1 \\ 0 \end{pmatrix} \Rightarrow u_B^{(1)} = \frac{\vec{p}\cdot \vec{\sigma}}{p^0 + mc} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{1}{E/c + mc} \begin{pmatrix} p_z \\ p_x + i p_y \end{pmatrix}
$$

$$ 
u_A^{(2)} = \begin{pmatrix} 0 \\ 1 \end{pmatrix} \Rightarrow u_B^{(2)} = \frac{\vec{p}\cdot \vec{\sigma}}{p^0 + mc} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \frac{1}{E/c + mc} \begin{pmatrix} p_x - i p_y \\ -p_z \end{pmatrix}
$$

Esto nos genera dos soluciones, linealmente independientes para los espinores. Podemos hallar las otras dos de la misma forma, pero esta vez fijando las componentes correspondientes a las anti-partículas y hallando las componentes de las partículas en función de estas.

$$
v_B^{(1)} = \begin{pmatrix} 1 \\ 0 \end{pmatrix} \Rightarrow v_A^{(1)} = \frac{\vec{p}\cdot \vec{\sigma}}{p^0 + mc} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{1}{E/c + mc} \begin{pmatrix} p_z \\ p_x + i p_y \end{pmatrix}
$$

$$ 
v_B^{(2)} = \begin{pmatrix} 0 \\ 1 \end{pmatrix} \Rightarrow v_A^{(2)} = \frac{\vec{p}\cdot \vec{\sigma}}{p^0 + mc} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \frac{1}{E/c + mc} \begin{pmatrix} p_x - i p_y \\ -p_z \end{pmatrix}
$$

En este ultimo caso se utilizo que $k^{\mu} = - p^{\mu}/\hbar$, de otra forma las soluciones $v_B$ divergen cuando $\vec{p} \rightarrow 0$ , ya que $p^0 \rightarrow mc$, estas soluciones corresponden a las anti-partículas, mientras que las primeras a las partículas. Finalmente podemos escribir una base para los espinores:

$$
u^{(1)} \sim \begin{pmatrix} 1 \\ 0 \\ \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \end{pmatrix} \qquad u^{(2)} \sim \begin{pmatrix} 0 \\ 1 \\ \frac{p_x - i p_y}{E/c + mc} \\ \frac{-p_z}{E/c + mc}  \end{pmatrix} \qquad 
v^{(1)} \sim \begin{pmatrix} \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \\ 1 \\ 0 \end{pmatrix} \qquad v^{(2)} \sim \begin{pmatrix} \frac{p_x - i p_y}{E/c + mc} \\ \frac{-p_z}{E/c + mc} \\ 0 \\ 1 \end{pmatrix}
$$

Buscamos ahora hallar la norma de los espinores propuestos:

$$
\begin{aligned}
(u^{(1)})^{\dagger}u^{(1)} \sim \begin{pmatrix} 1 & 0 & \frac{p_z}{E/c + mc} & \frac{p_x - i p_y}{E/c + mc}  \end{pmatrix} \begin{pmatrix} 1 \\ 0 \\ \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc} \end{pmatrix} = 1 + \frac{|\vec{p}|}{(E/c + mc)^2}\\
= 1 + \frac{(E/c)^2 - (mc)^2}{(E/c + mc)^2}  = 1 + \frac{E/c - mc}{E/c + mc} = \frac{2E/c}{E/c + mc}
\end{aligned}
$$

El mismo resultado se puede hallar para el resto de los espinores. Luego si se busca que la norma de estos sea $2E/c$ (Convención Halzen-Martin) , entonces:
$$ \frac{2E/c}{E/c + mc} N^2 = 2E/c \Rightarrow N = \sqrt{E/c + mc} $$ Finalmente, las soluciones canónicas para la ecuación de Dirac serán para las partículas:

$$ 
\psi^{(1)} = \frac{1}{\sqrt{E/c + mc}} \begin{pmatrix} 1 \\ 0 \\ \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \end{pmatrix} e^{-i\frac{mc^2}{\hbar}t} \qquad \psi^{(2)} = \frac{1}{\sqrt{E/c + mc}} \begin{pmatrix} 0 \\ 1 \\ \frac{p_x - i p_y}{E/c + mc} \\ \frac{-p_z}{E/c + mc}  \end{pmatrix}  e^{-i\frac{mc^2}{\hbar}t}
$$

Y para las antipartículas:

$$
\psi^{(3)} = \frac{1}{\sqrt{E/c + mc}} \begin{pmatrix} \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \\ 1 \\ 0 \end{pmatrix} e^{i\frac{mc^2}{\hbar}t} \qquad \psi^{(4)} = \frac{1}{\sqrt{E/c + mc}} \begin{pmatrix} \frac{p_x - i p_y}{E/c + mc} \\ \frac{-p_z}{E/c + mc} \\ 0 \\ 1 \end{pmatrix}  e^{i\frac{mc^2}{\hbar}t}
$$

### Espines.

Consideremos la matriz $\vec{S}$ compuesta por las matrices de Pauli:

$$
\vec{S} = \frac{\hbar}{2}\begin{pmatrix} \vec{\sigma} & 0 \\ 0 & \vec{\sigma} \end{pmatrix}
$$

Es fácil ver que los espinores encontrados no son auto-estados de la matriz $\vec{S}$. Basta con verificar para $u^{(1)}$ con la componente $\hat{S}_z$.

$$ \hat{\sigma}_z \begin{pmatrix} \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \end{pmatrix} \neq \lambda z \begin{pmatrix} \frac{p_z}{E/c + mc} \\ \frac{p_x + i p_y}{E/c + mc}  \end{pmatrix}  $$

Sin embargo si orientamos los espinores en la dirección $z$, esto es orientar el sistema de coordenadas espacial de modo que la dirección de la partícula coincida con $z$, podemos expresar los espinores como:

$$ 
u^{(1)} = \frac{1}{\sqrt{E/c + mc}} \begin{pmatrix} 1 \\ 0 \\ \frac{c |\vec{p}|}{E + mc^2} \\ 0 \end{pmatrix} = \begin{pmatrix} \sqrt{(E + mc^2)/c} \\ 0 \\ \sqrt{(E - m c^2)/c} \\ 0 \end{pmatrix} 
$$

De la misma forma:

$$ 
u^{(2)} = \begin{pmatrix} 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \\ -\sqrt{(E - m c^2)/c} \end{pmatrix} \qquad v^{(1)} =  \begin{pmatrix} 0 \\  -\sqrt{(E - m c^2)/c}  \\ 0 \\ \sqrt{(E + mc^2)/c} \end{pmatrix} \qquad v^{(2)} = - \begin{pmatrix} \sqrt{(E - m c^2)/c} \\ 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \end{pmatrix} 
$$

Podemos ver que estos son autoestados del operador $\hat{S}_z$.

$$ 
\hat{S}_z u^{(1)} = \frac{\hbar}{2} \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{pmatrix} \begin{pmatrix} \sqrt{(E + mc^2)/c} \\ 0 \\ \sqrt{(E - m c^2)/c} \\ 0 \end{pmatrix} =  \frac{\hbar}{2}  \begin{pmatrix} \sqrt{(E + mc^2)/c} \\ 0 \\ \sqrt{(E - m c^2)/c} \\ 0 \end{pmatrix} = \frac{\hbar}{2} u^{(1)}
$$

$$ 
\hat{S}_z u^{(2)} = \frac{\hbar}{2} \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{pmatrix} \begin{pmatrix} 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \\ -\sqrt{(E - m c^2)/c} \end{pmatrix} = -\frac{\hbar}{2}  \begin{pmatrix} 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \\ -\sqrt{(E - m c^2)/c} \end{pmatrix} = -\frac{\hbar}{2} u^{(2)}
$$

$$ 
\hat{S}_z v^{(1)} = \frac{\hbar}{2} \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{pmatrix} \begin{pmatrix} 0 \\  -\sqrt{(E - m c^2)/c}  \\ 0 \\ \sqrt{(E + mc^2)/c} \end{pmatrix} =  -\frac{\hbar}{2}  \begin{pmatrix} 0 \\  -\sqrt{(E - m c^2)/c}  \\ 0 \\ \sqrt{(E + mc^2)/c} \end{pmatrix} = -\frac{\hbar}{2} v^{(1)}
$$

$$ 
\hat{S}_z v^{(2)} = - \frac{\hbar}{2} \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{pmatrix} \begin{pmatrix} \sqrt{(E - m c^2)/c} \\ 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \end{pmatrix} =  - \frac{\hbar}{2}  \begin{pmatrix} \sqrt{(E - m c^2)/c} \\ 0 \\ \sqrt{(E + mc^2)/c} \\ 0 \end{pmatrix} = \frac{\hbar}{2} v^{(2)}
$$

Luego $u^{(1)}$, $u^{(2)}$, $v^{(1)}$, $v^{(2)}$ como *auto-espinores* del operador $\hat{S}_z$, en donde  $u^{(1)}$, $u^{(2)}$ corresponden a electrones con espines $\ket{\uparrow}$ y $\ket{\downarrow}$ respectivamente, y a  $v^{(1)}$, $v^{(2)}$ como positrones con espín $\ket{\uparrow}$ y $\ket{\downarrow}$ respectivamente.

### Conjugados de carga

Otro operador importante que se puede identificar, es el de conjugación de carga ($C$), el cual transforma un espinor de Dirac $\psi$ en el espinor conjugado de carga $\psi_c$ dado por:

$$ \psi_c = i \gamma^2 \psi^* $$

Donde $\gamma^2$ es la tercera matriz de Dirac, dada por:

$$ 
\gamma^2 = \begin{pmatrix} 0 & 0 & 0 & -i \\  0 & 0 & i & 0 \\ 0 & i & 0 & 0 \\ -i & 0 & 0 & 0 \end{pmatrix} 
$$

Se puede probar que los conjugados de carga de los auto-espinores de las partículas $u^{(1)}$ y $u^{(2)}$ son iguales a los auto-espinores $v^{(1)}$ y $v^{(2)}$ de las anti-partículas, respectivamente. Esto es:

$$ 
u^{(1)}_c = i \gamma^2 (u^{(1)})^* \sim \begin{pmatrix} 0 & 0 & 0 & 1 \\  0 & 0 & -1 & 0 \\ 0 & -1 & 0 & 0 \\ 1 & 0 & 0 & 0 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \\ \frac{cp_z}{E + mc^2} \\ \frac{c(p_x - i p_y)}{E + mc^2} \end{pmatrix} = \begin{pmatrix} \frac{c(p_x - i p_y)}{E + mc^2} \\ -\frac{cp_z}{E + mc^2} \\ 0 \\ 1 \end{pmatrix} = v^{(1)}
$$
  
$$ 
u^{(2)}_c = i \gamma^2 (u^{(2)})^* \sim \begin{pmatrix} 0 & 0 & 0 & 1 \\  0 & 0 & -1 & 0 \\ 0 & -1 & 0 & 0 \\ 1 & 0 & 0 & 0 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \\ \frac{c(p_x - i p_y)}{E + mc^2} \\ -\frac{cp_z}{E + mc^2} \end{pmatrix} =\begin{pmatrix}  \frac{cp_z}{E + mc^2} \\  \frac{c(p_x - i p_y)}{E + mc^2} \\1 \\0 \end{pmatrix} = v^{(2)}
$$
  