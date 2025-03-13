En electrodinámica cuántica, el fotón es la partícula mediadora de la fuerza electromagnética entre partículas cargadas. 

En electromagnetismo, el campo electromagnético esta descripto por las ecuaciones de Maxwell, las cuales se pueden en forma diferencial como:

$$
\vec{\nabla} \cdot \vec{E} = \frac{\rho}{\epsilon_0} \qquad \vec{\nabla} \cdot \vec{B} = 0
$$

$$ 
\vec{\nabla} \times \vec{E} = -\frac{\partial \vec{B}}{\partial t} \qquad  \vec{\nabla} \times \vec{B} = \mu_0 \vec{J} + \epsilon_0 \mu_0\frac{\partial \vec{E}}{\partial t}
$$

Para formular el electromagnetismo en términos de potenciales, introducimos al potencial vector $\vec{A}$, el cual es un campo vectorial que verifica:

$$ 
\vec{\nabla} \times \vec{A} = \vec{B} 
$$

Si escribimos la ley de Faraday en términos de este potencial, podemos describir al campo eléctrico $\vec{E}$ en términos del potencial vector $\vec{A}$.

$$
\vec{\nabla} \times \vec{E} = -\frac{\partial}{\partial t}(\vec{\nabla} \times \vec{A}) = \vec{\nabla}\times(-\frac{\partial\vec{A}}{\partial t})
$$

Puesto a que el rotacional del gradiente de un campo escalar es nulo, el gradiente de cualquier campo escalar dentro del paréntesis, se anularía al aplicarle el rotacional como en el ultimo termino. Esto nos permite introducir al *potencial eléctrico* $\phi$  en la ecuación y escribir el campo eléctrico como:   

$$ 
\vec{E} = -\vec{\nabla} \phi - \frac{\partial \vec{A}}{\partial t} 
$$

Reemplazando este resultado en la ley de Ampere o ultima ecuación de Maxwell, podemos expresar al potencial vector $\vec{A}$ como una onda. Veamos esto:

$$
\vec{\nabla} \times (\vec{\nabla} \times \vec{A}) = \mu_0 \vec{J} - \epsilon_0 \mu_0\frac{\partial}{\partial t}(\vec{\nabla} \phi + \frac{\partial \vec{A}}{\partial t}) 
$$

La velocidad de la luz en el vacío es una consecuencia directa de las propiedades electromagnéticas del espacio vacío,  la relación fundamental entre la velocidad de la luz , la permeabilidad del vacío ​ y la permitividad del vacío, puede escribirse como:

$$
c^2\mu_0 \epsilon_0 = 1 
$$

Desarrollando el termino rotacional, usando que $\vec{\nabla} \times (\vec{\nabla} \times \vec{A}) = \vec{\nabla}(\vec{\nabla} \cdot\vec{A}) - \nabla^2\vec{A}$ y reemplazando la relación anterior:

$$
\vec{\nabla}(\vec{\nabla} \cdot\vec{A}) - \nabla^2\vec{A} = \mu_0 \vec{J} - \frac{1}{c^2}\frac{\partial}{\partial t}\vec{\nabla} \phi - \frac{\partial^2 \vec{A}}{\partial t^2}
$$

Reordenando los términos podemos ver que el potencial vector $\vec{A}$ se propaga como una onda. 

$$
\nabla^2\vec{A} - \frac{\partial^2 \vec{A}}{\partial t^2} =  - \mu_0 \vec{J} +\vec{\nabla}(\vec{\nabla} \cdot\vec{A}+\frac{1}{c^2}\frac{\partial\phi}{\partial t})
$$

El gauge de Lorentz consiste en tomar $\vec{A}$ y $\phi$ tales que lo que se encuentre dentro del paréntesis se anule, es decir:

$$
\vec{\nabla} \cdot\vec{A} - \frac{1}{c^2}\frac{\partial \phi}{\partial t} = 0
$$

Reemplazando obtenemos la ecuación de onda para el potencial vector $\vec{A}$:

$$
\nabla^2\vec{A} - \frac{\partial^2 \vec{A}}{\partial t^2} =  - \mu_0 \vec{J}
$$

Veamos ahora que sucede con el potencial eléctrico. Volviendo a la definición de $\vec{E}$ en función de $\vec{A}$ y $\phi$, podemos tomar la divergencia de ambos miembros y recuperar la ley de Gauss o primera ecuación de Maxwell. 

$$ 
\vec{\nabla}\cdot\vec{E} = -\nabla^2 \phi - \frac{\partial (\vec{\nabla} \cdot \vec{A})}{\partial t} = \frac{\rho}{\epsilon_0}
$$

Reemplazando el gauge de Lorentz en la divergencia de $\vec{A}$, obtenemos una ecuación de onda para $\phi$ en términos de la densidad de carga $\rho$.

$$ 
\nabla^2 \phi - \frac{1}{c^2}\frac{\partial^2 \phi}{\partial t^2} = - \frac{\rho}{\epsilon_0}
$$

Esto nos dice que, tanto el potencial vector $\vec{A}$ como el potencial eléctrico $\phi$ se propagan como ondas a la velocidad de la luz. Yendo un paso mas halla, dividimos ambos miembros de la ecuación anterior por $c$. 

$$  
\nabla^2 \left(\frac{\phi}{c}\right) - \frac{1}{c^2}\frac{\partial^2}{\partial t^2}\left(\frac{\phi}{c}\right) = -\mu_0(c\rho)
$$

Las similitudes entre las ecuaciones de onda para $\vec{A}$ y $\phi$ nos llevan a definir el $4$-vector potencial $A$ y la $4$-corriente $J$ como: 

$$ 
A \equiv(\frac{\phi}{c}, \vec{A})\qquad J \equiv (c\rho, \vec{J} ) 
$$

De modo que ambas ecuaciones de onda, se reducen ahora a la ecuación:

$$ 
\partial^{\mu}\partial_{\mu} A^{\nu} = -\mu_0J^{\nu}
$$

Esto unifica elegantemente las ecuaciones de Maxwell con la teoría de la relatividad especial. Para el caso del fotón propagándose en el vacío, su comportamiento se puede describir utilizando la ecuación anterior en ausencia de cargas o corrientes, es decir $\partial^{\mu}\partial_{\mu} A ^{\nu} = 0$. Esta ecuación permite ondas planas como soluciones, es decir, potenciales de la forma:

$$
\Rightarrow A^{\nu}(x) \sim e^{-(i/\hbar)p \cdot x} \epsilon^{\nu}(p)
$$

En donde $p$ es el $4$-momento del fotón y $\epsilon$ es el $4$-vector polarización de la onda. Veamos ahora que el gauge de Lorentz puede escribirse simplemente como:

$$ 
\partial_{\nu} A^{\nu} = 0 \Rightarrow p_{\nu} \epsilon^{\nu}= 0
$$

Nótese que bajo la condición de ausencia de cargas o corrientes, el gauge de Lorentz es equivalente al gauge de Coulomb que implica $\vec{\nabla} \cdot \vec{A} = 0$. Esto ultimo nos da condiciones para la polarización del fotón.

$$ 
\epsilon^0 = 0 \qquad \vec{\epsilon} \cdot \vec{p} =0
$$

Esto ultimo nos dice que el vector polarización de un fotón es perpendicular a su dirección de propagación, la cual esta determinada por su momento $\vec{p}$. Se dice entonces que un fotón esta *transversalmente polarizado*.