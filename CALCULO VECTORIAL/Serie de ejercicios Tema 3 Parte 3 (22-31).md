# Problema 22 inciso 2

### Enunciado del problema

Determine los vectores $\mathbf{T}$ (Tangente Unitario), $\mathbf{N}$ (Normal Principal) y $\mathbf{B}$ (Binormal) para la curva $\mathbf{r}(t) = (4t, \cos 2t, \sin 2t)$ en todo $t$.

---

### Datos dados

La curva en $\mathbb{R}^3$ está definida por la función vectorial:
$$\mathbf{r}(t) = (4t, \cos 2t, \sin 2t)$$

Se buscan las expresiones para el Triedro Móvil: $\mathbf{T}(t)$, $\mathbf{N}(t)$ y $\mathbf{B}(t)$.

---

### Desarrollo paso a paso

El Triedro Móvil (o Marco de Frenet-Serret) se define mediante la aplicación directa de las siguientes fórmulas:

* **Vector Tangente Unitario:** $\mathbf{T}(t) = \frac{\mathbf{r}'(t)}{\lvert\mathbf{r}'(t)\rvert}$
* **Vector Normal Principal:** $\mathbf{N}(t) = \frac{\mathbf{T}'(t)}{\lvert\mathbf{T}'(t)\rvert}$
* **Vector Binormal:** $\mathbf{B}(t) = \mathbf{T}(t) \times \mathbf{N}(t)$

**Paso 1: Calcular el vector velocidad $\mathbf{r}'(t)$**

Derivamos la función $\mathbf{r}(t)$ componente a componente respecto a $t$:
$$\mathbf{r}'(t) = \frac{d}{dt} (4t, \cos 2t, \sin 2t)$$

$$\mathbf{r}'(t) = (4, -2\sin 2t, 2\cos 2t)$$

**Paso 2: Calcular la rapidez $\lvert\mathbf{r}'(t)\rvert$**

Calculamos la magnitud (norma) del vector velocidad:
$$\lvert\mathbf{r}'(t)\rvert = \sqrt{(4)^2 + (-2\sin 2t)^2 + (2\cos 2t)^2}$$

$$\lvert\mathbf{r}'(t)\rvert = \sqrt{16 + 4\sin^2 2t + 4\cos^2 2t}$$

Factorizamos el 4 y aplicamos la identidad pitagórica $\sin^2\theta + \cos^2\theta = 1$:
$$\lvert\mathbf{r}'(t)\rvert = \sqrt{16 + 4(\sin^2 2t + \cos^2 2t)}$$

$$\lvert\mathbf{r}'(t)\rvert = \sqrt{16 + 4(1)} = \sqrt{20}$$

$$\lvert\mathbf{r}'(t)\rvert = 2\sqrt{5}$$

**Paso 3: Calcular el vector Tangente Unitario $\mathbf{T}(t)$**

Normalizamos el vector velocidad dividiéndolo por su magnitud:
$$\mathbf{T}(t) = \frac{\mathbf{r}'(t)}{\lvert\mathbf{r}'(t)\rvert} = \frac{(4, -2\sin 2t, 2\cos 2t)}{2\sqrt{5}}$$

$$\mathbf{T}(t) = \left( \frac{4}{2\sqrt{5}}, \frac{-2\sin 2t}{2\sqrt{5}}, \frac{2\cos 2t}{2\sqrt{5}} \right)$$

$$\mathbf{T}(t) = \left( \frac{2}{\sqrt{5}}, -\frac{\sin 2t}{\sqrt{5}}, \frac{\cos 2t}{\sqrt{5}} \right)$$

**Paso 4: Calcular la derivada del tangente unitario $\mathbf{T}'(t)$**

Derivamos $\mathbf{T}(t)$ respecto a $t$ para encontrar la dirección del vector normal:
$$\mathbf{T}'(t) = \frac{d}{dt} \left[ \frac{1}{\sqrt{5}} (2, -\sin 2t, \cos 2t) \right]$$

$$\mathbf{T}'(t) = \frac{1}{\sqrt{5}} \left( \frac{d}{dt}[2], \frac{d}{dt}[-\sin 2t], \frac{d}{dt}[\cos 2t] \right)$$

$$\mathbf{T}'(t) = \frac{1}{\sqrt{5}} (0, -2\cos 2t, -2\sin 2t)$$

**Paso 5: Calcular la magnitud $\lvert\mathbf{T}'(t)\rvert$**

Calculamos la norma de $\mathbf{T}'(t)$:
$$\lvert\mathbf{T}'(t)\rvert = \sqrt{ (0)^2 + \left(\frac{-2\cos 2t}{\sqrt{5}}\right)^2 + \left(\frac{-2\sin 2t}{\sqrt{5}}\right)^2 }$$

$$\lvert\mathbf{T}'(t)\rvert = \sqrt{ 0 + \frac{4\cos^2 2t}{5} + \frac{4\sin^2 2t}{5} }$$

$$\lvert\mathbf{T}'(t)\rvert = \sqrt{ \frac{4}{5} (\cos^2 2t + \sin^2 2t) } = \sqrt{\frac{4}{5}(1)}$$

$$\lvert\mathbf{T}'(t)\rvert = \frac{2}{\sqrt{5}}$$

**Paso 6: Calcular el vector Normal Principal $\mathbf{N}(t)$**

Normalizamos el vector $\mathbf{T}'(t)$:
$$\mathbf{N}(t) = \frac{\mathbf{T}'(t)}{\lvert\mathbf{T}'(t)\rvert} = \frac{\frac{1}{\sqrt{5}} (0, -2\cos 2t, -2\sin 2t)}{\frac{2}{\sqrt{5}}}$$

$$\mathbf{N}(t) = \frac{1}{2} (0, -2\cos 2t, -2\sin 2t)$$

$$\mathbf{N}(t) = (0, -\cos 2t, -\sin 2t)$$

**Paso 7: Calcular el vector Binormal $\mathbf{B}(t)$**

Calculamos el producto cruz $\mathbf{B}(t) = \mathbf{T}(t) \times \mathbf{N}(t)$:
$$\mathbf{B}(t) = \left[ \frac{1}{\sqrt{5}} (2, -\sin 2t, \cos 2t) \right] \times \left[ (0, -\cos 2t, -\sin 2t) \right]$$

$$\mathbf{B}(t) = \frac{1}{\sqrt{5}} \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & -\sin 2t & \cos 2t \\ 0 & -\cos 2t & -\sin 2t \end{vmatrix}$$

Calculamos el determinante para cada componente:
* **Componente $\mathbf{i}$:** $\frac{1}{\sqrt{5}} [ (-\sin 2t)(-\sin 2t) - (\cos 2t)(-\cos 2t) ] = \frac{1}{\sqrt{5}} [ \sin^2 2t + \cos^2 2t ] = \frac{1}{\sqrt{5}}$
* **Componente $\mathbf{j}$:** $\frac{1}{\sqrt{5}} [ (\cos 2t)(0) - (2)(-\sin 2t) ] = \frac{1}{\sqrt{5}} [ 2\sin 2t ] = \frac{2\sin 2t}{\sqrt{5}}$
* **Componente $\mathbf{k}$:** $\frac{1}{\sqrt{5}} [ (2)(-\cos 2t) - (-\sin 2t)(0) ] = \frac{1}{\sqrt{5}} [ -2\cos 2t ] = -\frac{2\cos 2t}{\sqrt{5}}$

El vector resultante es:
$$\mathbf{B}(t) = \left( \frac{1}{\sqrt{5}}, \frac{2\sin 2t}{\sqrt{5}}, -\frac{2\cos 2t}{\sqrt{5}} \right)$$

---

### Resultado final

Las expresiones para los vectores del triedro móvil son:

**Vector Tangente Unitario:**
$$\mathbf{T}(t) = \left\langle \frac{2}{\sqrt{5}}, -\frac{\sin(2t)}{\sqrt{5}}, \frac{\cos(2t)}{\sqrt{5}} \right\rangle$$

**Vector Normal Principal:**
$$\mathbf{N}(t) = \left\langle 0, -\cos(2t), -\sin(2t) \right\rangle$$

**Vector Binormal:**
$$\mathbf{B}(t) = \left\langle \frac{1}{\sqrt{5}}, \frac{2\sin(2t)}{\sqrt{5}}, -\frac{2\cos(2t)}{\sqrt{5}} \right\rangle$$

---

### Interpretación breve del resultado

La curva $\mathbf{r}(t)$ describe una **hélice circular** que avanza a lo largo del eje $x$. Los resultados lo confirman:

1.  La **rapidez** $\lvert\mathbf{r}'(t)\rvert = 2\sqrt{5}$ es constante.
2.  La **curvatura** $\kappa = \frac{\lvert\mathbf{T}'(t)\rvert}{\lvert\mathbf{r}'(t)\rvert} = \frac{2/\sqrt{5}}{2\sqrt{5}} = \frac{1}{5}$ también es constante.
3.  El **vector Normal** $\mathbf{N}(t)$ no tiene componente en $x$ ($N_x = 0$) y siempre apunta hacia el eje $x$, que es el eje central de la hélice.

Estas son las propiedades características de una hélice uniforme.

---

✅ *Cálculos verificados: correctos.*

# Problema 22 inciso 4

### Enunciado del problema

Determine los vectores $\mathbf{T}$ (Tangente Unitario), $\mathbf{N}$ (Normal Principal) y $\mathbf{B}$ (Binormal) para la curva $\mathbf{r}(t) = (\sqrt{2}t, e^t, e^{-t})$ en el instante $t = 0$.

---

### Datos dados

La curva en $\mathbb{R}^3$ está definida por la función vectorial:
$$\mathbf{r}(t) = (\sqrt{2}t, e^t, e^{-t})$$

Se buscan los vectores $\mathbf{T}(0)$, $\mathbf{N}(0)$ y $\mathbf{B}(0)$, evaluados en el punto $t = 0$.

---

### Desarrollo paso a paso

El Triedro Móvil (Marco de Frenet-Serret) se calcula aplicando las definiciones diferenciales y evaluándolas en el punto $t=0$.

**Paso 1: Calcular el vector velocidad $\mathbf{r}'(t)$ y evaluarlo en $t=0$**

Primero, calculamos la derivada simbólica $\mathbf{r}'(t)$:
$$\mathbf{r}'(t) = \frac{d}{dt} (\sqrt{2}t, e^t, e^{-t}) = (\sqrt{2}, e^t, -e^{-t})$$

Evaluamos este vector en $t=0$:
$$\mathbf{r}'(0) = (\sqrt{2}, e^0, -e^{-0}) = (\sqrt{2}, 1, -1)$$

**Paso 2: Calcular la rapidez $\lvert\mathbf{r}'(0)\rvert$**

Calculamos la magnitud (norma) del vector velocidad en $t=0$:
$$\lvert\mathbf{r}'(0)\rvert = \sqrt{(\sqrt{2})^2 + (1)^2 + (-1)^2}$$
$$\lvert\mathbf{r}'(0)\rvert = \sqrt{2 + 1 + 1} = \sqrt{4} = 2$$

**Paso 3: Calcular el vector Tangente Unitario $\mathbf{T}(0)$**

Usamos la definición $\mathbf{T}(0) = \frac{\mathbf{r}'(0)}{\lvert\mathbf{r}'(0)\rvert}$:
$$\mathbf{T}(0) = \frac{(\sqrt{2}, 1, -1)}{2}$$
$$\mathbf{T}(0) = \left( \frac{\sqrt{2}}{2}, \frac{1}{2}, -\frac{1}{2} \right)$$

**Paso 4: Calcular la derivada del tangente $\mathbf{T}'(t)$ y evaluarla en $t=0$**

Para encontrar $\mathbf{N}(0)$, necesitamos $\mathbf{T}'(0)$. Primero, encontramos la expresión simbólica de $\mathbf{T}(t)$.

Calculamos la rapidez simbólica $\lvert\mathbf{r}'(t)\rvert$:
$$\lvert\mathbf{r}'(t)\rvert = \sqrt{(\sqrt{2})^2 + (e^t)^2 + (-e^{-t})^2} = \sqrt{2 + e^{2t} + e^{-2t}}$$
Reconociendo un trinomio cuadrado perfecto: $e^{2t} + 2(e^t)(e^{-t}) + e^{-2t} = (e^t + e^{-t})^2$.
$$\lvert\mathbf{r}'(t)\rvert = \sqrt{(e^t + e^{-t})^2} = e^t + e^{-t}$$

El vector tangente simbólico es:
$$\mathbf{T}(t) = \frac{\mathbf{r}'(t)}{\lvert\mathbf{r}'(t)\rvert} = \frac{(\sqrt{2}, e^t, -e^{-t})}{e^t + e^{-t}}$$

Para derivar $\mathbf{T}(t)$, usamos la regla del producto $\mathbf{T}'(t) = \frac{d}{dt} [f(t) \cdot \mathbf{v}(t)]$, donde $f(t) = (e^t + e^{-t})^{-1}$ y $\mathbf{v}(t) = \mathbf{r}'(t) = (\sqrt{2}, e^t, -e^{-t})$.

$$\mathbf{T}'(t) = f'(t)\mathbf{v}(t) + f(t)\mathbf{v}'(t)$$

Calculamos las derivadas $f'(t)$ y $\mathbf{v}'(t)$:
$f'(t) = -1(e^t + e^{-t})^{-2} \cdot (e^t - e^{-t}) = \frac{-(e^t - e^{-t})}{(e^t + e^{-t})^2}$
$\mathbf{v}'(t) = (0, e^t, e^{-t})$

Ahora, evaluamos todas las componentes en $t=0$:
* $f(0) = (e^0 + e^0)^{-1} = (1+1)^{-1} = \frac{1}{2}$
* $f'(0) = \frac{-(e^0 - e^0)}{(e^0 + e^0)^2} = \frac{-(1-1)}{(1+1)^2} = 0$
* $\mathbf{v}(0) = (\sqrt{2}, 1, -1)$
* $\mathbf{v}'(0) = (0, e^0, e^{-0}) = (0, 1, 1)$

Sustituimos estos valores en la fórmula de $\mathbf{T}'(0)$:
$$\mathbf{T}'(0) = f'(0)\mathbf{v}(0) + f(0)\mathbf{v}'(0)$$
$$\mathbf{T}'(0) = (0) \cdot (\sqrt{2}, 1, -1) + \left(\frac{1}{2}\right) \cdot (0, 1, 1)$$
$$\mathbf{T}'(0) = (0, 0, 0) + \left(0, \frac{1}{2}, \frac{1}{2}\right)$$
$$\mathbf{T}'(0) = \left(0, \frac{1}{2}, \frac{1}{2}\right)$$

**Paso 5: Calcular la magnitud $\lvert\mathbf{T}'(0)\rvert$**

Calculamos la norma del vector $\mathbf{T}'(0)$:
$$\lvert\mathbf{T}'(0)\rvert = \sqrt{(0)^2 + (\frac{1}{2})^2 + (\frac{1}{2})^2}$$
$$\lvert\mathbf{T}'(0)\rvert = \sqrt{0 + \frac{1}{4} + \frac{1}{4}} = \sqrt{\frac{2}{4}} = \sqrt{\frac{1}{2}} = \frac{\sqrt{2}}{2}$$

**Paso 6: Calcular el vector Normal Principal $\mathbf{N}(0)$**

Usamos la definición $\mathbf{N}(0) = \frac{\mathbf{T}'(0)}{\lvert\mathbf{T}'(0)\rvert}$:
$$\mathbf{N}(0) = \frac{(0, \frac{1}{2}, \frac{1}{2})}{\frac{\sqrt{2}}{2}}$$
$$\mathbf{N}(0) = \frac{2}{\sqrt{2}} \left(0, \frac{1}{2}, \frac{1}{2}\right) = \sqrt{2} \left(0, \frac{1}{2}, \frac{1}{2}\right)$$
$$\mathbf{N}(0) = \left(0, \frac{\sqrt{2}}{2}, \frac{\sqrt{2}}{2}\right)$$

**Paso 7: Calcular el vector Binormal $\mathbf{B}(0)$**

Calculamos el producto cruz $\mathbf{B}(0) = \mathbf{T}(0) \times \mathbf{N}(0)$:
$$\mathbf{B}(0) = \left( \frac{\sqrt{2}}{2}, \frac{1}{2}, -\frac{1}{2} \right) \times \left( 0, \frac{\sqrt{2}}{2}, \frac{\sqrt{2}}{2} \right)$$

Resolvemos usando el determinante:
$$\mathbf{B}(0) = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ \frac{\sqrt{2}}{2} & \frac{1}{2} & -\frac{1}{2} \\ 0 & \frac{\sqrt{2}}{2} & \frac{\sqrt{2}}{2} \end{vmatrix}$$

* **Componente $\mathbf{i}$:** $\left( (\frac{1}{2})(\frac{\sqrt{2}}{2}) - (-\frac{1}{2})(\frac{\sqrt{2}}{2}) \right) = \frac{\sqrt{2}}{4} + \frac{\sqrt{2}}{4} = \frac{2\sqrt{2}}{4} = \frac{\sqrt{2}}{2}$
* **Componente $\mathbf{j}$:** $- \left( (\frac{\sqrt{2}}{2})(\frac{\sqrt{2}}{2}) - (-\frac{1}{2})(0) \right) = - \left( \frac{2}{4} - 0 \right) = -\frac{1}{2}$
* **Componente $\mathbf{k}$:** $\left( (\frac{\sqrt{2}}{2})(\frac{\sqrt{2}}{2}) - (\frac{1}{2})(0) \right) = \frac{2}{4} - 0 = \frac{1}{2}$

$$\mathbf{B}(0) = \left( \frac{\sqrt{2}}{2}, -\frac{1}{2}, \frac{1}{2} \right)$$

---

### Resultado final

Los vectores del triedro móvil para la curva $\mathbf{r}(t) = (\sqrt{2}t, e^t, e^{-t})$ en el instante $t = 0$ son:

**Vector Tangente Unitario:**
$$\mathbf{T}(0) = \left\langle \frac{\sqrt{2}}{2}, \frac{1}{2}, -\frac{1}{2} \right\rangle$$

**Vector Normal Principal:**
$$\mathbf{N}(0) = \left\langle 0, \frac{\sqrt{2}}{2}, \frac{\sqrt{2}}{2} \right\rangle$$

**Vector Binormal:**
$$\mathbf{B}(0) = \left\langle \frac{\sqrt{2}}{2}, -\frac{1}{2}, \frac{1}{2} \right\rangle$$

---

### Interpretación breve del resultado

Se verifica que el sistema $(\mathbf{T}(0), \mathbf{N}(0), \mathbf{B}(0))$ es ortonormal, es decir, todos los vectores son unitarios y mutuamente ortogonales (su producto punto es cero):

* $\lvert\mathbf{T}(0)\rvert = \sqrt{\frac{2}{4} + \frac{1}{4} + \frac{1}{4}} = 1$
* $\lvert\mathbf{N}(0)\rvert = \sqrt{0 + \frac{2}{4} + \frac{2}{4}} = 1$
* $\lvert\mathbf{B}(0)\rvert = \sqrt{\frac{2}{4} + \frac{1}{4} + \frac{1}{4}} = 1$
* $\mathbf{T}(0) \cdot \mathbf{N}(0) = 0 + \frac{\sqrt{2}}{4} - \frac{\sqrt{2}}{4} = 0$

Los tres vectores forman una base ortonormal derecha que describe la orientación de la curva en $t=0$.

---

✅ *Cálculos verificados: correctos.*

---

# Problema 23

### Enunciado del problema

Verificar si las curvas en el espacio:
$$\mathbf{u}(T) = \left(-\frac{1}{2}\sin^2 T - \sin T, 1 - \frac{1}{2}\sin^2 T - \sin T, \frac{1}{2}\sin T \cos T + \frac{1}{2}T\right)$$

$$\mathbf{r}(t) = (t, \cos t, \sin t)$$

se cortan entre sí. En caso afirmativo, determinar el punto de intersección y el ángulo entre sus vectores tangentes en el punto de intersección. Si no se cortan, justificar.

---

### Datos dados

* Curva 1: $\mathbf{r}(t) = (t, \cos t, \sin t)$
* Curva 2: $\mathbf{u}(T) = \left(-\frac{1}{2}\sin^2 T - \sin T, 1 - \frac{1}{2}\sin^2 T - \sin T, \frac{1}{2}\sin T \cos T + \frac{1}{2}T\right)$

Se buscan los parámetros $(t_0, T_0)$ tales que $\mathbf{r}(t_0) = \mathbf{u}(T_0)$, el punto $\mathbf{P_0}$ y el ángulo $\theta$ entre $\mathbf{r}'(t_0)$ y $\mathbf{u}'(T_0)$.

---

### Desarrollo paso a paso

**Fase 1: Búsqueda del punto de intersección**

Para encontrar una intersección, debemos igualar las componentes de $\mathbf{r}(t)$ y $\mathbf{u}(T)$, lo que genera un sistema de 3 ecuaciones con 2 incógnitas ($t, T$):

$$
\begin{aligned}
(x): \quad t &= -\frac{1}{2}\sin^2 T - \sin T \\
(y): \quad \cos t &= 1 - \frac{1}{2}\sin^2 T - \sin T \\
(z): \quad \sin t &= \frac{1}{2}\sin T \cos T + \frac{1}{2}T
\end{aligned}
$$

**Paso 1.1: Resolver el subsistema (x) e (y)**

Observamos que la expresión de la Ecuación (x) aparece en la Ecuación (y). Sustituimos (x) en (y):
$$\cos t = 1 + (t)$$

Resolvemos la ecuación $\cos t = 1 + t$.
* Sabemos que el rango de $\cos t$ es $[-1, 1]$.
* Si $t > 0$, entonces $1 + t > 1$, lo cual está fuera del rango de $\cos t$.
* Si $t < 0$, entonces $1 + t < 1$.
* La única posibilidad es $t = 0$. Verificamos:
    * Lado Izquierdo: $\cos(0) = 1$
    * Lado Derecho: $1 + (0) = 1$
* Por lo tanto, la única solución real es $t = 0$.

**Paso 1.2: Encontrar T usando $t=0$**

Sustituimos $t=0$ en la Ecuación (x):
$$0 = -\frac{1}{2}\sin^2 T - \sin T$$

Factorizamos $\sin T$:
$$0 = \sin T \left( -\frac{1}{2}\sin T - 1 \right)$$

Esto genera dos posibles casos:
1.  $\sin T = 0 \implies T = k\pi$, para cualquier entero $k \in \mathbb{Z}$.
2.  $-\frac{1}{2}\sin T - 1 = 0 \implies \sin T = -2$. Esto es imposible, ya que el rango de $\sin T$ es $[-1, 1]$.

Las únicas soluciones candidatas para $T$ son $T = k\pi$.

**Paso 1.3: Verificar la Ecuación (z)**

Debemos encontrar qué pareja $(t, T) = (0, k\pi)$ satisface la Ecuación (z):
$$\sin t = \frac{1}{2}\sin T \cos T + \frac{1}{2}T$$

Sustituimos los valores:
$$\sin(0) = \frac{1}{2}\sin(k\pi)\cos(k\pi) + \frac{1}{2}(k\pi)$$

Dado que $\sin(k\pi) = 0$ para cualquier entero $k$:
$$0 = \frac{1}{2}(0)\cos(k\pi) + \frac{k\pi}{2}$$
$$0 = \frac{k\pi}{2}$$

La única solución para esta ecuación es $k=0$.
Por lo tanto, la única solución al sistema es $(t, T) = (0, 0)$. Las curvas sí se cortan.

**Paso 1.4: Determinar el punto de intersección $P_0$**

Evaluamos $\mathbf{r}(t)$ en $t=0$:
$$\mathbf{P_0} = \mathbf{r}(0) = (0, \cos 0, \sin 0)$$
$$\mathbf{P_0} = (0, 1, 0)$$

(Verificación con $\mathbf{u}(0)$: $\mathbf{u}(0) = (-\frac{1}{2}\sin^2 0 - \sin 0, 1 - \frac{1}{2}\sin^2 0 - \sin 0, \frac{1}{2}\sin 0 \cos 0 + 0) = (0, 1, 0)$. Coinciden.)

**Fase 2: Cálculo del ángulo de intersección**

**Paso 2.1: Calcular el vector tangente $\mathbf{v}_r = \mathbf{r}'(0)$**

Derivamos $\mathbf{r}(t) = (t, \cos t, \sin t)$:
$$\mathbf{r}'(t) = (1, -\sin t, \cos t)$$

Evaluamos en $t=0$:
$$\mathbf{v}_r = \mathbf{r}'(0) = (1, -\sin 0, \cos 0) = (1, 0, 1)$$

**Paso 2.2: Calcular el vector tangente $\mathbf{v}_u = \mathbf{u}'(0)$**

Derivamos $\mathbf{u}(T)$:
* $x'(T) = \frac{d}{dT} \left(-\frac{1}{2}\sin^2 T - \sin T\right) = -\frac{1}{2}(2\sin T \cos T) - \cos T = -\sin T \cos T - \cos T$
* $y'(T) = \frac{d}{dT} \left(1 - \frac{1}{2}\sin^2 T - \sin T\right) = -\sin T \cos T - \cos T$
* $z'(T) = \frac{d}{dT} \left(\frac{1}{2}\sin T \cos T + \frac{1}{2}T\right) = \frac{d}{dT} \left(\frac{1}{4}\sin(2T) + \frac{1}{2}T\right) = \frac{1}{4}(2\cos(2T)) + \frac{1}{2} = \frac{1}{2}\cos(2T) + \frac{1}{2}$

Evaluamos en $T=0$:
* $x'(0) = -\sin 0 \cos 0 - \cos 0 = 0 - 1 = -1$
* $y'(0) = -\sin 0 \cos 0 - \cos 0 = 0 - 1 = -1$
* $z'(0) = \frac{1}{2}\cos(0) + \frac{1}{2} = \frac{1}{2}(1) + \frac{1}{2} = 1$

$$\mathbf{v}_u = \mathbf{u}'(0) = (-1, -1, 1)$$

**Paso 2.3: Calcular el ángulo $\theta$**

Usamos la fórmula del producto escalar: $\cos \theta = \frac{\mathbf{v}_r \cdot \mathbf{v}_u}{\lvert\mathbf{v}_r\rvert \lvert\mathbf{v}_u\rvert}$.

Calculamos el producto escalar (numerador):
$$\mathbf{v}_r \cdot \mathbf{v}_u = (1, 0, 1) \cdot (-1, -1, 1)$$
$$\mathbf{v}_r \cdot \mathbf{v}_u = (1)(-1) + (0)(-1) + (1)(1) = -1 + 0 + 1 = 0$$

Dado que el producto escalar es 0, y los vectores tangentes no son nulos ($\lvert\mathbf{v}_r\rvert = \sqrt{2}$, $\lvert\mathbf{v}_u\rvert = \sqrt{3}$), $\cos \theta = 0$.
$$\theta = \arccos(0) = \frac{\pi}{2} \text{ radianes}$$

---

### Resultado final

* **Intersección:** Sí, las curvas se cortan.
* **Punto de Intersección:** La intersección ocurre en el único punto $\mathbf{P_0 = (0, 1, 0)}$, correspondiente a los parámetros $t=0$ y $T=0$.
* **Ángulo de Intersección:**
    $$\theta = \frac{\pi}{2} \text{ radianes (o } 90^\circ)$$

---

### Interpretación breve del resultado

El análisis del sistema de ecuaciones confirma que las curvas se cruzan en un único punto. El cálculo de los vectores tangentes en dicho punto, $\mathbf{v}_r = (1, 0, 1)$ y $\mathbf{v}_u = (-1, -1, 1)$, revela que su producto escalar es 0. Esto significa que los vectores son **ortogonales**, y por lo tanto, las curvas se cortan en un ángulo recto ($90^\circ$).

---

✅ *Cálculos verificados: correctos.*

---

# Problema 24 inciso 7

### Enunciado del problema

Calcular la curvatura de $\mathbf{r}(t) = (e^t \cos t, e^t \sin t, e^t)$.

---

### Datos dados

La curva en $\mathbb{R}^3$ está definida por la función vectorial:
$$\mathbf{r}(t) = (e^t \cos t, e^t \sin t, e^t)$$

Se busca la curvatura $\kappa(t)$ usando la fórmula general:
$$\kappa(t) = \frac{\lvert\mathbf{r}'(t) \times \mathbf{r}''(t)\rvert}{\lvert\mathbf{r}'(t)\rvert^3}$$

---

### Desarrollo paso a paso

**Paso 1: Calcular el vector velocidad $\mathbf{r}'(t)$**

Se aplica la regla del producto a cada componente:
* $x'(t) = \frac{d}{dt}(e^t \cos t) = e^t \cos t - e^t \sin t = e^t(\cos t - \sin t)$
* $y'(t) = \frac{d}{dt}(e^t \sin t) = e^t \sin t + e^t \cos t = e^t(\sin t + \cos t)$
* $z'(t) = \frac{d}{dt}(e^t) = e^t$

$$\mathbf{r}'(t) = (e^t(\cos t - \sin t), e^t(\sin t + \cos t), e^t)$$

**Paso 2: Calcular el vector aceleración $\mathbf{r}''(t)$**

Se derivan las componentes de $\mathbf{r}'(t)$, aplicando nuevamente la regla del producto:
* $x''(t) = \frac{d}{dt}(e^t(\cos t - \sin t)) = e^t(\cos t - \sin t) + e^t(-\sin t - \cos t) = -2e^t \sin t$
* $y''(t) = \frac{d}{dt}(e^t(\sin t + \cos t)) = e^t(\sin t + \cos t) + e^t(\cos t - \sin t) = 2e^t \cos t$
* $z''(t) = \frac{d}{dt}(e^t) = e^t$

$$\mathbf{r}''(t) = (-2e^t \sin t, 2e^t \cos t, e^t)$$

**Paso 3: Calcular el producto cruz $\mathbf{r}'(t) \times \mathbf{r}''(t)$**

$$\mathbf{r}'(t) \times \mathbf{r}''(t) = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ e^t(\cos t - \sin t) & e^t(\sin t + \cos t) & e^t \\ -2e^t \sin t & 2e^t \cos t & e^t \end{vmatrix}$$

Se factoriza $e^t$ de la segunda fila y $e^t$ de la tercera fila, resultando en un factor $e^{2t}$:
$$ = e^{2t} \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ \cos t - \sin t & \sin t + \cos t & 1 \\ -2 \sin t & 2 \cos t & 1 \end{vmatrix}$$

* $\mathbf{i}: e^{2t} [ (\sin t + \cos t)(1) - (1)(2 \cos t) ] = e^{2t} (\sin t - \cos t)$
* $\mathbf{j}: -e^{2t} [ (\cos t - \sin t)(1) - (1)(-2 \sin t) ] = -e^{2t} (\cos t + \sin t)$
* $\mathbf{k}: e^{2t} [ (\cos t - \sin t)(2 \cos t) - (\sin t + \cos t)(-2 \sin t) ]$
    $ = e^{2t} [ (2\cos^2 t - 2\sin t \cos t) - (-2\sin^2 t - 2\sin t \cos t) ]$
    $ = e^{2t} [ 2\cos^2 t + 2\sin^2 t ] = 2e^{2t}$

$$\mathbf{r}'(t) \times \mathbf{r}''(t) = (e^{2t}(\sin t - \cos t), -e^{2t}(\sin t + \cos t), 2e^{2t})$$

**Paso 4: Calcular la magnitud $\lvert\mathbf{r}'(t) \times \mathbf{r}''(t)\rvert$ (Numerador)**

$$\lvert\mathbf{r}'(t) \times \mathbf{r}''(t)\rvert = \sqrt{ [e^{2t}(\sin t - \cos t)]^2 + [-e^{2t}(\sin t + \cos t)]^2 + [2e^{2t}]^2 }$$

Se factoriza $\sqrt{e^{4t}} = e^{2t}$:
$$ = e^{2t} \sqrt{ (\sin t - \cos t)^2 + (\sin t + \cos t)^2 + 2^2 }$$
$$ = e^{2t} \sqrt{ (\sin^2 t - 2\sin t \cos t + \cos^2 t) + (\sin^2 t + 2\sin t \cos t + \cos^2 t) + 4 }$$
$$ = e^{2t} \sqrt{ (1) + (1) + 4 } = e^{2t} \sqrt{6}$$
$$\lvert\mathbf{r}'(t) \times \mathbf{r}''(t)\rvert = \sqrt{6} e^{2t}$$

**Paso 5: Calcular la magnitud $\lvert\mathbf{r}'(t)\rvert$ (Rapidez)**

$$\lvert\mathbf{r}'(t)\rvert = \sqrt{ [e^t(\cos t - \sin t)]^2 + [e^t(\sin t + \cos t)]^2 + [e^t]^2 }$$

Se factoriza $\sqrt{e^{2t}} = e^{t}$:
$$ = e^{t} \sqrt{ (\cos t - \sin t)^2 + (\sin t + \cos t)^2 + 1^2 }$$
$$ = e^{t} \sqrt{ (\cos^2 t - 2\sin t \cos t + \sin^2 t) + (\sin^2 t + 2\sin t \cos t + \cos^2 t) + 1 }$$
$$ = e^{t} \sqrt{ (1) + (1) + 1 } = e^{t} \sqrt{3}$$
$$\lvert\mathbf{r}'(t)\rvert = \sqrt{3} e^t$$

**Paso 6: Calcular $\lvert\mathbf{r}'(t)\rvert^3$ (Denominador)**

$$\lvert\mathbf{r}'(t)\rvert^3 = (\sqrt{3} e^t)^3 = (\sqrt{3})^3 (e^t)^3 = 3\sqrt{3} e^{3t}$$

**Paso 7: Calcular la curvatura $\kappa(t)$**

$$\kappa(t) = \frac{\lvert\mathbf{r}'(t) \times \mathbf{r}''(t)\rvert}{\lvert\mathbf{r}'(t)\rvert^3} = \frac{\sqrt{6} e^{2t}}{3\sqrt{3} e^{3t}}$$

Se simplifican los términos:
* Radicales: $\frac{\sqrt{6}}{3\sqrt{3}} = \frac{\sqrt{2}\sqrt{3}}{3\sqrt{3}} = \frac{\sqrt{2}}{3}$
* Exponentes: $\frac{e^{2t}}{e^{3t}} = e^{2t-3t} = e^{-t}$

$$\kappa(t) = \frac{\sqrt{2}}{3} e^{-t}$$

---

### Resultado final

La curvatura de la curva en un instante $t$ es:
$$\kappa(t) = \frac{\sqrt{2}}{3e^t}$$

---

### Interpretación breve del resultado

La curva descrita es una **espiral cónica**, ya que yace sobre la superficie del cono $z^2 = x^2 + y^2$ (puesto que $(e^t)^2 = (e^t\cos t)^2 + (e^t\sin t)^2$).

El resultado $\kappa(t) = \frac{\sqrt{2}}{3} e^{-t}$ muestra que a medida que $t$ aumenta ($t \to \infty$), la curvatura $\kappa(t)$ tiende a cero. Esto significa que la espiral se "abre" y se vuelve progresivamente "más recta" a medida que se aleja del origen (el vértice del cono).

---

✅ *Cálculos verificados: correctos.*

# Problema 24 inciso 8

### Enunciado del problema

Calcular la curvatura $\kappa$ de la curva polar $r = 1 - \sin \theta$ en $\theta = \frac{\pi}{3}$.

---

### Datos dados

La curva está definida en coordenadas polares por la ecuación:
$$r(\theta) = 1 - \sin \theta$$

El punto de evaluación es $\theta_0 = \frac{\pi}{3}$.

La fórmula de curvatura para una curva polar $r = r(\theta)$ es:
$$\kappa(\theta) = \frac{\lvert r^2 + 2(r')^2 - r r'' \rvert}{(r^2 + (r')^2)^{3/2}}$$
Donde $r' = \frac{dr}{d\theta}$ y $r'' = \frac{d^2r}{d\theta^2}$.

---

### Desarrollo paso a paso

**Paso 1: Calcular las derivadas $r'(\theta)$ y $r''(\theta)$**

$$r(\theta) = 1 - \sin \theta$$

$$r'(\theta) = \frac{d}{d\theta} (1 - \sin \theta) = -\cos \theta$$

$$r''(\theta) = \frac{d}{d\theta} (-\cos \theta) = \sin \theta$$

**Paso 2: Evaluar $r$, $r'$, y $r''$ en $\theta = \frac{\pi}{3}$**

Usamos los valores trigonométricos $\sin(\frac{\pi}{3}) = \frac{\sqrt{3}}{2}$ y $\cos(\frac{\pi}{3}) = \frac{1}{2}$.

* $r = 1 - \sin\left(\frac{\pi}{3}\right) = 1 - \frac{\sqrt{3}}{2} = \frac{2 - \sqrt{3}}{2}$
* $r' = -\cos\left(\frac{\pi}{3}\right) = -\frac{1}{2}$
* $r'' = \sin\left(\frac{\pi}{3}\right) = \frac{\sqrt{3}}{2}$

**Paso 3: Calcular el Numerador $\lvert r^2 + 2(r')^2 - r r'' \rvert$**

Calculamos cada término del numerador por separado:
* $r^2 = \left(\frac{2 - \sqrt{3}}{2}\right)^2 = \frac{4 - 4\sqrt{3} + 3}{4} = \frac{7 - 4\sqrt{3}}{4}$
* $2(r')^2 = 2 \left(-\frac{1}{2}\right)^2 = 2 \left(\frac{1}{4}\right) = \frac{2}{4}$
* $r r'' = \left(\frac{2 - \sqrt{3}}{2}\right) \left(\frac{\sqrt{3}}{2}\right) = \frac{2\sqrt{3} - 3}{4}$

Sustituimos estos valores en la expresión del numerador:
$$\left\lvert \frac{7 - 4\sqrt{3}}{4} + \frac{2}{4} - \frac{2\sqrt{3} - 3}{4} \right\rvert$$

$$= \left\lvert \frac{(7 - 4\sqrt{3}) + 2 - (2\sqrt{3} - 3)}{4} \right\rvert$$

$$= \left\lvert \frac{7 - 4\sqrt{3} + 2 - 2\sqrt{3} + 3}{4} \right\rvert$$

$$= \left\lvert \frac{(7+2+3) + (-4\sqrt{3} - 2\sqrt{3})}{4} \right\rvert$$

$$= \left\lvert \frac{12 - 6\sqrt{3}}{4} \right\rvert = \frac{6 - 3\sqrt{3}}{2}$$

(El valor absoluto se elimina ya que $6 = \sqrt{36}$ y $3\sqrt{3} = \sqrt{27}$, por lo que $6 > 3\sqrt{3}$).

**Paso 4: Calcular el Denominador $(r^2 + (r')^2)^{3/2}$**

Primero, calculamos la base $(r^2 + (r')^2)$:
* $r^2 = \frac{7 - 4\sqrt{3}}{4}$
* $(r')^2 = \left(-\frac{1}{2}\right)^2 = \frac{1}{4}$

$$r^2 + (r')^2 = \frac{7 - 4\sqrt{3}}{4} + \frac{1}{4} = \frac{8 - 4\sqrt{3}}{4} = 2 - \sqrt{3}$$

El denominador completo es $(2 - \sqrt{3})^{3/2}$.

**Paso 5: Calcular la curvatura $\kappa$**

$$\kappa = \frac{\text{Numerador}}{\text{Denominador}} = \frac{\frac{6 - 3\sqrt{3}}{2}}{(2 - \sqrt{3})^{3/2}}$$

Factorizamos el numerador para simplificar:
$$\kappa = \frac{\frac{3(2 - \sqrt{3})}{2}}{(2 - \sqrt{3})^{3/2}}$$

Aplicamos la regla de exponentes $\frac{x}{x^{3/2}} = x^{1 - 3/2} = x^{-1/2} = \frac{1}{\sqrt{x}}$:
$$\kappa = \frac{3}{2 \cdot (2 - \sqrt{3})^{1/2}} = \frac{3}{2\sqrt{2 - \sqrt{3}}}$$

**Paso 6: Simplificación del radical anidado**

El término $\sqrt{2 - \sqrt{3}}$ puede simplificarse. Usando la identidad $\sqrt{A - \sqrt{B}} = \sqrt{\frac{A+C}{2}} - \sqrt{\frac{A-C}{2}}$ donde $C=\sqrt{A^2-B}$:
$A=2, B=3 \implies C = \sqrt{2^2 - 3} = 1$.
$\sqrt{2 - \sqrt{3}} = \sqrt{\frac{2+1}{2}} - \sqrt{\frac{2-1}{2}} = \sqrt{\frac{3}{2}} - \sqrt{\frac{1}{2}} = \frac{\sqrt{3} - 1}{\sqrt{2}}$.

Sustituimos esto en la expresión de $\kappa$:
$$\kappa = \frac{3}{2 \left( \frac{\sqrt{3} - 1}{\sqrt{2}} \right)} = \frac{3\sqrt{2}}{2(\sqrt{3} - 1)}$$

Racionalizamos el denominador:
$$\kappa = \frac{3\sqrt{2}}{2(\sqrt{3} - 1)} \cdot \frac{\sqrt{3} + 1}{\sqrt{3} + 1}$$

$$\kappa = \frac{3\sqrt{2}(\sqrt{3} + 1)}{2(3 - 1)} = \frac{3\sqrt{6} + 3\sqrt{2}}{2(2)}$$

$$\kappa = \frac{3(\sqrt{6} + \sqrt{2})}{4}$$

---

### Resultado final

La curvatura de la curva $r = 1 - \sin \theta$ en $\theta = \frac{\pi}{3}$ es:
$$\kappa = \frac{3(\sqrt{6} + \sqrt{2})}{4}$$

---

### Interpretación breve del resultado

El valor $\kappa \approx 2.896$ es un escalar positivo que mide cuán bruscamente se dobla la curva (conocida como cardioide) en el punto $\theta = \frac{\pi}{3}$. Un valor mayor indica una curva más cerrada, y un valor menor indica una curva más "plana".

---

✅ *Cálculos verificados: correctos.*

# Problema 24 inciso 9

### Enunciado del problema

Halle la ecuación del círculo de curvatura (círculo osculador) de la gráfica de la función $y = x^2$ en $x = 5$.

---

### Datos dados

* Función: $y = x^2$
* Punto de evaluación: $x_0 = 5$

Se busca la ecuación canónica del círculo $(x-h)^2 + (y-k)^2 = R^2$.

---

### Desarrollo paso a paso

**1. Calcular el punto de tangencia $(x_0, y_0)$**

Evaluamos la función en $x_0 = 5$:
$$y_0 = (5)^2 = 25$$
El punto de tangencia es $\mathbf{P_0 = (5, 25)}$.

**2. Calcular las derivadas y evaluarlas en $x_0 = 5$**

Calculamos la primera y segunda derivada de $y = x^2$:
$$y' = \frac{d}{dx}(x^2) = 2x$$
$$y'' = \frac{d}{dx}(2x) = 2$$

Evaluamos ambas en $x_0 = 5$:
* $y'(5) = 2(5) = 10$
* $y''(5) = 2$

**3. Calcular el Radio de Curvatura $R$**

Se utiliza la fórmula del radio de curvatura para una función $y=f(x)$:
$$R = \frac{(1 + (y')^2)^{3/2}}{\lvert y'' \rvert}$$

Sustituimos los valores evaluados:
$$R = \frac{(1 + (10)^2)^{3/2}}{\lvert 2 \rvert} = \frac{(1 + 100)^{3/2}}{2}$$
$$R = \frac{(101)^{3/2}}{2} = \frac{101\sqrt{101}}{2}$$

**4. Calcular el Centro de Curvatura $(h, k)$**

Las coordenadas del centro $(h, k)$ se calculan con las siguientes fórmulas:

**Coordenada $h$:**
$$h = x_0 - \frac{y'(1 + (y')^2)}{y''}$$
$$h = 5 - \frac{10(1 + (10)^2)}{2} = 5 - \frac{10(101)}{2}$$
$$h = 5 - 5(101) = 5 - 505 = -500$$

**Coordenada $k$:**
$$k = y_0 + \frac{1 + (y')^2}{y''}$$
$$k = 25 + \frac{1 + (10)^2}{2} = 25 + \frac{101}{2}$$
$$k = \frac{50}{2} + \frac{101}{2} = \frac{151}{2}$$

El centro del círculo es $\left(-500, \frac{151}{2}\right)$.

**5. Ensamblar la ecuación del círculo**

La ecuación es $(x-h)^2 + (y-k)^2 = R^2$.
Calculamos $R^2$:
$$R^2 = \left( \frac{101\sqrt{101}}{2} \right)^2 = \frac{101^2 \cdot (\sqrt{101})^2}{2^2}$$
$$R^2 = \frac{101^2 \cdot 101}{4} = \frac{101^3}{4} = \frac{1030301}{4}$$

Sustituimos $h$, $k$ y $R^2$:
$$(x - (-500))^2 + \left(y - \frac{151}{2}\right)^2 = \frac{1030301}{4}$$

---

### Resultado final

La ecuación del círculo de curvatura es:
$$(x + 500)^2 + \left(y - \frac{151}{2}\right)^2 = \frac{1030301}{4}$$

---

### Interpretación breve del resultado

La ecuación describe el círculo que mejor se aproxima a la parábola $y=x^2$ en el punto $(5, 25)$. Dado que $y'' = 2 > 0$, la parábola es cóncava hacia arriba. Esto se verifica con el resultado, ya que el centro del círculo $k = \frac{151}{2} = 75.5$ está "por encima" del punto de tangencia $y_0 = 25$.

---

✅ *Cálculos verificados: correctos.*

# Problema 24 inciso 13

### Enunciado del problema

Halle la ecuación del círculo de curvatura (círculo osculador) de la gráfica de la función $y = x^2$ en $x = 3$.

---

### Datos dados

* Función: $y = x^2$
* Punto de evaluación: $x_0 = 3$

Se busca la ecuación canónica del círculo de curvatura: $(x-h)^2 + (y-k)^2 = R^2$.

---

### Desarrollo paso a paso

**1. Calcular el punto de tangencia $(x_0, y_0)$**

Se evalúa la función en $x_0 = 3$:
$$y_0 = (3)^2 = 9$$
El punto de tangencia es $\mathbf{P_0 = (3, 9)}$.

**2. Calcular las derivadas y evaluarlas en $x_0 = 3$**

Se calcula la primera y segunda derivada de $y = x^2$:
$$y' = \frac{d}{dx}(x^2) = 2x$$
$$y'' = \frac{d}{dx}(2x) = 2$$

Se evalúan ambas derivadas en $x_0 = 3$:
* $y'(3) = 2(3) = 6$
* $y''(3) = 2$

**3. Calcular el Radio de Curvatura $R$**

Se utiliza la fórmula del radio de curvatura para una función explícita $y=f(x)$:
$$R = \frac{(1 + (y')^2)^{3/2}}{\lvert y'' \rvert}$$

Sustituyendo los valores evaluados:
$$R = \frac{(1 + (6)^2)^{3/2}}{\lvert 2 \rvert} = \frac{(1 + 36)^{3/2}}{2}$$

$$R = \frac{(37)^{3/2}}{2} = \frac{37\sqrt{37}}{2}$$

**4. Calcular el Centro de Curvatura $(h, k)$**

Las coordenadas del centro $(h, k)$ se obtienen con las siguientes fórmulas:

**Coordenada $h$:**
$$h = x_0 - \frac{y'(1 + (y')^2)}{y''}$$

$$h = 3 - \frac{6 \cdot (1 + (6)^2)}{2} = 3 - \frac{6(37)}{2}$$
$$h = 3 - 3(37) = 3 - 111 = -108$$

**Coordenada $k$:**
$$k = y_0 + \frac{1 + (y')^2}{y''}$$

$$k = 9 + \frac{1 + (6)^2}{2} = 9 + \frac{37}{2}$$
$$k = \frac{18}{2} + \frac{37}{2} = \frac{55}{2}$$

El centro del círculo es $\left(-108, \frac{55}{2}\right)$.

**5. Ensamblar la ecuación del círculo**

La ecuación canónica es $(x-h)^2 + (y-k)^2 = R^2$.
Primero, calculamos $R^2$:
$$R^2 = \left( \frac{37\sqrt{37}}{2} \right)^2 = \frac{37^2 \cdot (\sqrt{37})^2}{2^2}$$
$$R^2 = \frac{37^2 \cdot 37}{4} = \frac{37^3}{4} = \frac{50653}{4}$$

Sustituimos $h$, $k$ y $R^2$:
$$(x - (-108))^2 + \left(y - \frac{55}{2}\right)^2 = \frac{50653}{4}$$

---

### Resultado final

La ecuación del círculo de curvatura es:
$$(x + 108)^2 + \left(y - \frac{55}{2}\right)^2 = \frac{50653}{4}$$

---

### Interpretación breve del resultado

La ecuación describe el círculo que mejor se aproxima a la parábola $y=x^2$ en el punto $(3, 9)$. Dado que $y'' = 2 > 0$, la parábola es cóncava hacia arriba. Esto es coherente con el resultado, ya que la coordenada $y$ del centro ($k = \frac{55}{2} = 27.5$) está "por encima" de la coordenada $y$ del punto de tangencia ($y_0 = 9$).

---

✅ *Cálculos verificados: correctos.*

---

# Problema 25

### Enunciado del problema

Hallar la ecuación del círculo osculador en el punto máximo y mínimo de $y = \frac{1}{3}x^3 - x$.

---

### Datos dados

* Función: $y = \frac{1}{3}x^3 - x$
* Puntos de evaluación: Los puntos de extremo local (máximo y mínimo) de la función.

Se buscan las ecuaciones canónicas $(x-h)^2 + (y-k)^2 = R^2$ para dichos puntos.

---

### Desarrollo paso a paso

**Paso 1: Calcular las derivadas**

Se calcula la primera ($y'$) y segunda ($y''$) derivada de la función:
$$y = \frac{1}{3}x^3 - x$$

$$y' = \frac{d}{dx}\left(\frac{1}{3}x^3 - x\right) = x^2 - 1$$

$$y'' = \frac{d}{dx}(x^2 - 1) = 2x$$

**Paso 2: Encontrar y clasificar los puntos críticos**

Se encuentran los puntos críticos resolviendo $y' = 0$:
$$x^2 - 1 = 0 \implies x = \pm 1$$

Se clasifican usando el criterio de la segunda derivada ($y'' = 2x$):
* Para $x = -1$: $y''(-1) = 2(-1) = -2$. Como $y'' < 0$, este punto es un **Máximo Local**.
* Para $x = 1$: $y''(1) = 2(1) = 2$. Como $y'' > 0$, este punto es un **Mínimo Local**.

**Paso 3: Calcular las coordenadas de los puntos extremos**

Se calculan las coordenadas $y$ para cada punto crítico:
* **Punto Máximo ($P_{max}$)** en $x_0 = -1$:
    $$y_0 = \frac{1}{3}(-1)^3 - (-1) = -\frac{1}{3} + 1 = \frac{2}{3}$$
    $\mathbf{P_{max} = \left(-1, \frac{2}{3}\right)}$

* **Punto Mínimo ($P_{min}$)** en $x_0 = 1$:
    $$y_0 = \frac{1}{3}(1)^3 - (1) = \frac{1}{3} - 1 = -\frac{2}{3}$$
    $\mathbf{P_{min} = \left(1, -\frac{2}{3}\right)}$

**Paso 4: Calcular el Círculo Osculador 1 (En el Máximo)**

En un extremo local, la tangente es horizontal ($y'=0$). Las fórmulas para el centro $(h, k)$ y el radio $R$ se simplifican a:
* $R = \frac{1}{\lvert y'' \rvert}$
* $h = x_0$
* $k = y_0 + \frac{1}{y''}$

Usamos los datos de $P_{max}$: $(x_0, y_0) = (-1, 2/3)$ y $y'' = -2$.
* Radio $R_1$: $R_1 = \frac{1}{\lvert -2 \rvert} = \frac{1}{2}$
* Centro $h_1$: $h_1 = -1$
* Centro $k_1$: $k_1 = \frac{2}{3} + \frac{1}{-2} = \frac{2}{3} - \frac{1}{2} = \frac{4 - 3}{6} = \frac{1}{6}$

La ecuación es $(x - h_1)^2 + (y - k_1)^2 = R_1^2$:
$$(x - (-1))^2 + \left(y - \frac{1}{6}\right)^2 = \left(\frac{1}{2}\right)^2$$
$$(x + 1)^2 + \left(y - \frac{1}{6}\right)^2 = \frac{1}{4}$$

**Paso 5: Calcular el Círculo Osculador 2 (En el Mínimo)**

Usamos los datos de $P_{min}$: $(x_0, y_0) = (1, -2/3)$ y $y'' = 2$.
* Radio $R_2$: $R_2 = \frac{1}{\lvert 2 \rvert} = \frac{1}{2}$
* Centro $h_2$: $h_2 = 1$
* Centro $k_2$: $k_2 = -\frac{2}{3} + \frac{1}{2} = \frac{-4 + 3}{6} = -\frac{1}{6}$

La ecuación es $(x - h_2)^2 + (y - k_2)^2 = R_2^2$:
$$(x - 1)^2 + \left(y - \left(-\frac{1}{6}\right)\right)^2 = \left(\frac{1}{2}\right)^2$$
$$(x - 1)^2 + \left(y + \frac{1}{6}\right)^2 = \frac{1}{4}$$

---

### Resultado final

Las ecuaciones de los círculos osculadores en los puntos de extremo local son:

* **En el Punto Máximo $P_{max} = (-1, \frac{2}{3})$:**
    $$(x + 1)^2 + \left(y - \frac{1}{6}\right)^2 = \frac{1}{4}$$

* **En el Punto Mínimo $P_{min} = (1, -\frac{2}{3})$:**
    $$(x - 1)^2 + \left(y + \frac{1}{6}\right)^2 = \frac{1}{4}$$

---

### Interpretación breve del resultado

La función $y = \frac{1}{3}x^3 - x$ es una función impar (simétrica respecto al origen). Los resultados obtenidos son coherentes con esta simetría:
* Los puntos de tangencia $P_{max} = (-1, 2/3)$ y $P_{min} = (1, -2/3)$ son simétricos respecto al origen.
* Los centros de curvatura $C_1 = (-1, 1/6)$ y $C_2 = (1, -1/6)$ también son simétricos respecto al origen.
* Los radios de curvatura $R_1 = 1/2$ y $R_2 = 1/2$ son idénticos, como se esperaba.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 26

### Enunciado del problema

Muestre que el vector de aceleración $\mathbf{a}(t)$ se expresa como:
$$\mathbf{a}(t) = v \frac{d\mathbf{T}}{dt} + \frac{dv}{dt}\mathbf{T}$$

---

### Datos dados

Para esta demostración, se parte de las definiciones fundamentales de la cinemática:

* **Vector Velocidad:** $\mathbf{v}(t)$
* **Vector Aceleración:** $\mathbf{a}(t) = \frac{d}{dt}\mathbf{v}(t)$
* **Rapidez (escalar):** $v(t) = \lvert \mathbf{v}(t) \rvert$
* **Vector Tangente Unitario:** $\mathbf{T}(t) = \frac{\mathbf{v}(t)}{\lvert \mathbf{v}(t) \rvert} = \frac{\mathbf{v}(t)}{v(t)}$

---

### Desarrollo paso a paso

1.  Se inicia reordenando la definición del vector tangente unitario $\mathbf{T}(t)$ para expresar el vector velocidad $\mathbf{v}(t)$ como el producto de su magnitud (la rapidez $v(t)$) y su dirección (el vector $\mathbf{T}(t)$).

    $$\mathbf{v}(t) = v(t) \mathbf{T}(t)$$

2.  Por definición, el vector aceleración $\mathbf{a}(t)$ es la derivada temporal del vector velocidad $\mathbf{v}(t)$.

    $$\mathbf{a}(t) = \frac{d}{dt} \mathbf{v}(t)$$

3.  Se sustituye la expresión de $\mathbf{v}(t)$ del primer paso en la definición de $\mathbf{a}(t)$.

    $$\mathbf{a}(t) = \frac{d}{dt} \left[ v(t) \mathbf{T}(t) \right]$$

4.  Se aplica la regla del producto para la derivada de un escalar ($v(t)$) que multiplica a un vector ($\mathbf{T}(t)$):
    *(Regla: $\frac{d}{dt} [f(t)\mathbf{u}(t)] = f'(t)\mathbf{u}(t) + f(t)\mathbf{u}'(t)$)*

    $$\mathbf{a}(t) = \left( \frac{dv}{dt} \right) \mathbf{T}(t) + v(t) \left( \frac{d\mathbf{T}}{dt} \right)$$

5.  Utilizando la propiedad conmutativa de la suma de vectores, se reordenan los términos para que coincidan con la expresión solicitada.

    $$\mathbf{a}(t) = v(t) \frac{d\mathbf{T}}{dt} + \frac{dv}{dt}\mathbf{T}(t)$$

---

### Resultado final

Queda demostrado que la aceleración se puede expresar como:
$$\mathbf{a}(t) = v \frac{d\mathbf{T}}{dt} + \frac{dv}{dt}\mathbf{T}$$

---

### Interpretación breve del resultado

Esta ecuación es fundamental en la cinemática, ya que descompone el vector de aceleración $\mathbf{a}$ en sus dos componentes ortogonales:

* **Componente Tangencial:** El término $\frac{dv}{dt}\mathbf{T}$. Es paralelo a la dirección del movimiento (dirección $\mathbf{T}$) y describe el cambio en la **magnitud** de la velocidad (la rapidez).
* **Componente Normal:** El término $v\frac{d\mathbf{T}}{dt}$. Es perpendicular al movimiento (ya que $\mathbf{T}'$ es ortogonal a $\mathbf{T}$) y describe el cambio en la **dirección** de la velocidad.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 27

### Enunciado del problema

La posición de una partícula está determinada por la expresión $\mathbf{r}(t) = (3t^2 - 15t + 1)\mathbf{i} + (10t - 2t^2 - 2)\mathbf{j} + (5t^2 - 25t + 3)\mathbf{k}$. Calcule la distancia recorrida entre los segundos 3 y 7.

---

### Datos dados

* **Vector de Posición:** $\mathbf{r}(t) = (3t^2 - 15t + 1)\mathbf{i} + (10t - 2t^2 - 2)\mathbf{j} + (5t^2 - 25t + 3)\mathbf{k}$
* **Intervalo de tiempo:** $t_1 = 3 \text{ s}$ a $t_2 = 7 \text{ s}$.

Se busca la distancia recorrida (longitud de arco) $L$, la cual se calcula con la integral de la rapidez:
$$L = \int_{t_1}^{t_2} \lvert \mathbf{v}(t) \rvert dt = \int_{3}^{7} \lvert \mathbf{r}'(t) \rvert dt$$

---

### Desarrollo paso a paso

**Paso 1: Calcular el vector velocidad $\mathbf{v}(t)$**

Se deriva el vector de posición $\mathbf{r}(t)$ con respecto al tiempo $t$:
$$\mathbf{v}(t) = \mathbf{r}'(t) = \frac{d}{dt} \mathbf{r}(t)$$

$$\mathbf{v}(t) = \frac{d}{dt} (3t^2 - 15t + 1)\mathbf{i} + \frac{d}{dt} (10t - 2t^2 - 2)\mathbf{j} + \frac{d}{dt} (5t^2 - 25t + 3)\mathbf{k}$$

$$\mathbf{v}(t) = (6t - 15)\mathbf{i} + (10 - 4t)\mathbf{j} + (10t - 25)\mathbf{k}$$

**Paso 2: Calcular la rapidez $\lvert \mathbf{v}(t) \rvert$**

Se calcula la magnitud (norma) del vector velocidad. Para simplificar, se factorizan las componentes:
* $v_x = 6t - 15 = 3(2t - 5)$
* $v_y = 10 - 4t = -2(2t - 5)$
* $v_z = 10t - 25 = 5(2t - 5)$

El vector velocidad se puede reescribir como:
$$\mathbf{v}(t) = (2t - 5) \cdot (3\mathbf{i} - 2\mathbf{j} + 5\mathbf{k})$$

Ahora, calculamos la magnitud:
$$\lvert \mathbf{v}(t) \rvert = \lvert (2t - 5) \cdot (3\mathbf{i} - 2\mathbf{j} + 5\mathbf{k}) \rvert$$
$$\lvert \mathbf{v}(t) \rvert = \lvert 2t - 5 \rvert \cdot \lvert 3\mathbf{i} - 2\mathbf{j} + 5\mathbf{k} \rvert$$
$$\lvert \mathbf{v}(t) \rvert = \lvert 2t - 5 \rvert \cdot \sqrt{3^2 + (-2)^2 + 5^2}$$
$$\lvert \mathbf{v}(t) \rvert = \lvert 2t - 5 \rvert \cdot \sqrt{9 + 4 + 25}$$
$$\lvert \mathbf{v}(t) \rvert = \sqrt{38} \lvert 2t - 5 \rvert$$

**Paso 3: Configurar y evaluar la integral de la distancia $L$**

Se establece la integral definida para la longitud de arco:
$$L = \int_{3}^{7} \sqrt{38} \lvert 2t - 5 \rvert dt = \sqrt{38} \int_{3}^{7} \lvert 2t - 5 \rvert dt$$

Se analiza el signo del término $(2t - 5)$ en el intervalo de integración $t \in [3, 7]$. El término $2t - 5$ es cero en $t = 2.5$.
Dado que $t \ge 3$ en todo el intervalo, $2t - 5$ es siempre positivo. Por lo tanto, $\lvert 2t - 5 \rvert = (2t - 5)$ para $t \in [3, 7]$.

La integral se simplifica a:
$$L = \sqrt{38} \int_{3}^{7} (2t - 5) dt$$

Se resuelve la integral:
$$L = \sqrt{38} \left[ \frac{2t^2}{2} - 5t \right]_{3}^{7}$$
$$L = \sqrt{38} \left[ t^2 - 5t \right]_{3}^{7}$$

Aplicando el Teorema Fundamental del Cálculo:
$$L = \sqrt{38} \left[ (7^2 - 5(7)) - (3^2 - 5(3)) \right]$$
$$L = \sqrt{38} \left[ (49 - 35) - (9 - 15) \right]$$
$$L = \sqrt{38} \left[ 14 - (-6) \right]$$
$$L = \sqrt{38} (14 + 6)$$
$$L = 20\sqrt{38}$$

---

### Resultado final

La distancia recorrida por la partícula entre los segundos 3 y 7 es:
$$L = 20\sqrt{38} \text{ metros}$$

---

### Interpretación breve del resultado

La distancia total recorrida por la partícula en el intervalo de tiempo $[3 \text{ s}, 7 \text{ s}]$ es $20\sqrt{38}$ metros, que es aproximadamente $123.29$ metros. Esto se obtiene integrando la rapidez $\lvert \mathbf{v}(t) \rvert$, que resultó ser una función lineal simple $\sqrt{38}(2t-5)$ en ese intervalo.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 28

### Enunciado del problema

Un canal de desagüe pluvial, emplea dos láminas galvanizadas, las cuales se colocan sobre los planos $4x + 2y + 6z = 12$ y $3x + 6y + 2z = 6$. Determine las ecuaciones paramétricas de la trayectoria del canal (considere a $x = t$ como el parámetro).

---

### Datos dados

La trayectoria del canal es la línea de intersección de los dos planos:
* Plano 1 ($P_1$): $4x + 2y + 6z = 12$
* Plano 2 ($P_2$): $3x + 6y + 2z = 6$

La parametrización solicitada debe usar $x = t$.

---

### Desarrollo paso a paso

**Paso 1: Establecer y simplificar el sistema de ecuaciones**

Se establece el sistema de ecuaciones de los planos. Se divide la Ecuación 1 entre 2 para simplificar el álgebra:
$$
\begin{aligned}
(I) \quad 2x + y + 3z &= 6 \\
(II) \quad 3x + 6y + 2z &= 6
\end{aligned}
$$

**Paso 2: Despejar $y$ en función de $x$ (Eliminación de $z$)**

Se multiplica la Ecuación (I) por 2 y la Ecuación (II) por 3 para igualar los coeficientes de $z$:
$$
\begin{aligned}
(I) \times 2 \implies 4x + 2y + 6z = 12 \\
(II) \times 3 \implies 9x + 18y + 6z = 18
\end{aligned}
$$
Se resta la nueva Ecuación (I) de la nueva Ecuación (II):
$$(9x - 4x) + (18y - 2y) + (6z - 6z) = 18 - 12$$

$$5x + 16y = 6$$

Despejando $y$:
$$16y = 6 - 5x$$

$$y = \frac{6 - 5x}{16} = \frac{3}{8} - \frac{5}{16}x$$

**Paso 3: Despejar $z$ en función de $x$ (Eliminación de $y$)**

Se utiliza el sistema simplificado del Paso 1. Se multiplica la Ecuación (I) por 6 para igualar los coeficientes de $y$:
$$
\begin{aligned}
(I) \times 6 \implies 12x + 6y + 18z = 36 \\
(II) \implies 3x + 6y + 2z = 6
\end{aligned}
$$
Se resta la Ecuación (II) de la nueva Ecuación (I):
$$(12x - 3x) + (6y - 6y) + (18z - 2z) = 36 - 6$$

$$9x + 16z = 30$$

Despejando $z$:
$$16z = 30 - 9x$$

$$z = \frac{30 - 9x}{16} = \frac{15}{8} - \frac{9}{16}x$$

**Paso 4: Aplicar la parametrización $x = t$**

Se sustituye $x = t$ en las expresiones encontradas para $x$, $y$, y $z$:
$$x(t) = t$$

$$y(t) = \frac{3}{8} - \frac{5}{16}t$$

$$z(t) = \frac{15}{8} - \frac{9}{16}t$$

---

### Resultado final

Las ecuaciones paramétricas de la trayectoria del canal (la línea de intersección) son:
$$
\begin{aligned}
x(t) &= t \\
y(t) &= \frac{3}{8} - \frac{5}{16}t \\
z(t) &= \frac{15}{8} - \frac{9}{16}t
\end{aligned}
$$

---

### Interpretación breve del resultado

Estas ecuaciones describen una línea recta en $\mathbb{R}^3$ que representa la intersección de los dos planos (las láminas). Como se verificó en el análisis proporcionado (Paso 4 de la entrada), cualquier punto $(x, y, z)$ generado por un valor $t$ en esta línea satisface las ecuaciones de *ambos* planos simultáneamente.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 29

### Enunciado del problema

Se dispara una bala perpendicularmente hacia arriba con un arma y a una velocidad inicial de $v_0 = 300 \, m/s$. ¿Cuál es la altura máxima que alcanza la bala? Observación: No se toma en cuenta la resistencia del aire.

---

### Datos dados

* **Velocidad inicial ($v_0$):** $+300 \, m/s$
* **Posición inicial ($y_0$):** $0 \, m$ (punto de disparo)
* **Aceleración constante ($a$):** $-g = -9.8 \, m/s^2$ (actuando hacia abajo)
* **Velocidad final ($v_f$) en $h_{max}$:** $0 \, m/s$ (condición en la altura máxima)

---

### Desarrollo paso a paso

Se utiliza la ecuación de cinemática (M.R.U.A.) independiente del tiempo, ya que relaciona las velocidades, la aceleración y el desplazamiento ($h_{max}$).

$$v_f^2 = v_0^2 + 2a \cdot h_{max}$$

Sustituimos los valores conocidos en la ecuación:
$$(0)^2 = (300)^2 + 2(-9.8) \cdot h_{max}$$

$$0 = 90000 - 19.6 \cdot h_{max}$$

Despejamos $h_{max}$:
$$19.6 \cdot h_{max} = 90000$$

$$h_{max} = \frac{90000}{19.6}$$

$$h_{max} \approx 4591.8367... \, m$$

---

### Resultado final

Redondeando el resultado a 6 cifras significativas (según el protocolo):
$$h_{max} = 4591.84 \, m$$

---

### Interpretación breve del resultado

La altura máxima, $h_{max} \approx 4.59 \, km$, es el desplazamiento vertical que alcanza la bala en el instante exacto en que su velocidad vertical se reduce a $0 \, m/s$ debido a la aceleración constante de la gravedad, antes de comenzar su descenso.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 30

### Enunciado del problema

La velocidad de una partícula está dada por la expresión $\mathbf{v}(t) = (10^6 e^{-t} + 3t^2)\mathbf{i} - (2t + 2)\mathbf{j}$. Determine la distancia del origen al punto donde se encuentra la partícula en $t = 9$ s si se sabe que la partícula se encuentra en el punto $P(700, 20, 0)$ cuando $t = 12$. Considere $t$ en segundos, distancia en metros y velocidad en $m/s$.

---

### Datos dados

* **Vector Velocidad:** $\mathbf{v}(t) = (10^6 e^{-t} + 3t^2)\mathbf{i} - (2t + 2)\mathbf{j} + 0\mathbf{k}$
* **Condición de Contorno:** $\mathbf{r}(12) = (700, 20, 0)$
* **Tiempo Final de Evaluación:** $t_F = 9 \, s$

El objetivo es encontrar la distancia al origen $D = \lvert \mathbf{r}(9) \rvert$.

---

### Desarrollo paso a paso

La distancia al origen se calcula encontrando el vector de posición $\mathbf{r}(t)$ en $t=9 \, s$ y luego calculando su magnitud.

**Paso 1: Posición General $\mathbf{r}(t)$**
Se integra el vector velocidad $\mathbf{v}(t)$ para obtener el vector de posición general:
$$\mathbf{r}(t) = \int \mathbf{v}(t) dt = \int \left[ (10^6 e^{-t} + 3t^2)\mathbf{i} - (2t + 2)\mathbf{j} \right] dt$$

$$\mathbf{r}(t) = (-10^6 e^{-t} + t^3 + C_x)\mathbf{i} + (-t^2 - 2t + C_y)\mathbf{j} + C_z\mathbf{k}$$

**Paso 2: Cálculo de Constantes de Integración**
Se utiliza la condición de contorno $\mathbf{r}(12) = (700, 20, 0)$:
* $z(12) = 0 \implies C_z = 0$
* $y(12) = 20 \implies -(12)^2 - 2(12) + C_y = 20 \implies -144 - 24 + C_y = 20 \implies -168 + C_y = 20 \implies \mathbf{C_y = 188}$
* $x(12) = 700 \implies -10^6 e^{-12} + (12)^3 + C_x = 700 \implies -6.144... + 1728 + C_x = 700 \implies 1721.855... + C_x = 700 \implies \mathbf{C_x \approx -1021.856}$

**Paso 3: Posición Específica $\mathbf{r}(t)$**
Sustituyendo las constantes:
$$\mathbf{r}(t) = (-10^6 e^{-t} + t^3 - 1021.856)\mathbf{i} + (-t^2 - 2t + 188)\mathbf{j}$$

**Paso 4: Posición en $t = 9$ s**
Se evalúa $\mathbf{r}(t)$ en $t=9$:
* $x(9) = -10^6 e^{-9} + (9)^3 - 1021.856 = -123.410... + 729 - 1021.856 \approx -416.266 \, m$
* $y(9) = -(9)^2 - 2(9) + 188 = -81 - 18 + 188 = 89 \, m$
* $z(9) = 0 \, m$

$$\mathbf{r}(9) = -416.266\mathbf{i} + 89\mathbf{j}$$

**Paso 5: Distancia al Origen $D$**
$$D = \lvert \mathbf{r}(9) \rvert = \sqrt{x(9)^2 + y(9)^2 + z(9)^2}$$

$$D = \sqrt{(-416.266)^2 + (89)^2 + 0^2}$$

$$D \approx \sqrt{173277.3 + 7921} = \sqrt{181198.3}$$

$$D \approx 425.674 \, m$$

---

### Resultado final

La distancia del origen al punto donde se encuentra la partícula en $t = 9 \, s$ es:
$$D = 425.674 \, m$$

---

### Interpretación breve del resultado

Tras integrar la velocidad para hallar la trayectoria específica de la partícula (usando $\mathbf{r}(12)$ para encontrar las constantes de integración), se determina que su posición en $t=9 \, s$ es $\mathbf{r}(9) \approx (-416.27, 89, 0)$. La distancia euclidiana desde el origen $(0,0,0)$ a este punto es de $425.674 \, m$.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 31

### Enunciado del problema

Una persona se encuentra en un faro a una altura $h_1 = 18m$ y ve partir un barco con altura $h_2 = 18m$ que sigue una trayectoria: $\mathbf{p}(t) = (r\sin(10 - 4t)\cos(10 - 4t), r\sin(10 - 4t)\sin(10 - 4t), r\cos(10 - 4t))$. Donde $t$ es el tiempo en hora. ¿Cuál es la distancia que recorre el barco a lo largo de la trayectoria desde la base del faro, hasta que se deja de ver el mástil? Considere que la tierra es esférica y con un radio $r = 6371 km$.

---

### Datos dados

* **Altura del faro ($h_1$):** $18 \, m$
* **Altura del mástil ($h_2$):** $18 \, m$
* **Radio de la Tierra ($r$):** $6371 \, km = 6,371,000 \, m$
* **Trayectoria $\mathbf{p}(t)$:** *(Información distractora, ver Interpretación)*

---

### Desarrollo paso a paso

Este es un problema de horizonte geométrico. La distancia $S$ que el barco puede recorrer antes de que su mástil desaparezca del horizonte del observador en el faro es la suma de la distancia del horizonte del faro ($S_1$) y la distancia del horizonte del barco ($S_2$).

**Paso 1: Calcular la distancia del horizonte del faro ($S_1$)**

Se forma un triángulo rectángulo entre el centro de la Tierra (C), la cima del faro (F) y el punto de tangencia en el horizonte (H). La hipotenusa es $r + h_1$ y uno de los catetos es $r$. El ángulo central en C es $\theta_1$.

Usando trigonometría:
$$\cos(\theta_1) = \frac{r}{r + h_1}$$
$$\cos(\theta_1) = \frac{6,371,000}{6,371,000 + 18} = \frac{6,371,000}{6,371,018} \approx 0.999997175$$

Calculamos $\theta_1$ en radianes:
$$\theta_1 = \arccos(0.999997175) \approx 0.00237699 \, \text{rad}$$

La distancia de arco $S_1$ es $r \cdot \theta_1$:
$$S_1 = (6,371,000 \, m) \cdot (0.00237699 \, \text{rad}) \approx 15144.5 \, m$$

**Paso 2: Calcular la distancia del horizonte del barco ($S_2$)**

Dado que la altura del mástil $h_2 = 18 \, m$ es idéntica a la altura del faro $h_1$, el cálculo es el mismo:
$$S_2 = S_1 \approx 15144.5 \, m$$

**Paso 3: Calcular la distancia total $S$**

La distancia total es la suma de ambas distancias de arco:
$$S = S_1 + S_2$$
$$S \approx 15144.5 \, m + 15144.5 \, m = 30289 \, m$$

---

### Resultado final

La distancia que recorre el barco es $\mathbf{30289 \, m}$ (o $30.289 \, km$).

---

### Interpretación breve del resultado

La ecuación de la trayectoria $\mathbf{p}(t)$ es información irrelevante (un distractor). El problema se resuelve determinando la distancia geométrica máxima (la línea del horizonte) a la que dos objetos de $18m$ de altura pueden verse mutuamente en un planeta con un radio de $6371 \, km$. Esta distancia es la suma de la distancia al horizonte de cada objeto, resultando en aproximadamente $30.29 \, km$.

---

✅ *Cálculos verificados: correctos.*

---