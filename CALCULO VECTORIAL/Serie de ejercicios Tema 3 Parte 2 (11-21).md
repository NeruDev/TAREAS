# Problema 11 inciso 3

### Enunciado del problema

Para una partícula con vector de posición dado por la función vectorial de variable real $\mathbf{h}(t) = (3t \cos t, 3t \sin t, 4t)$, determine su velocidad instantánea $\mathbf{v}(t)$, su aceleración instantánea $\mathbf{a}(t)$ y su rapidez $\nu(t)$.

---

### Datos dados

El vector de posición de la partícula es $\mathbf{h}(t) = (h_x(t), h_y(t), h_z(t))$, donde las componentes escalares son:

$$h_x(t) = 3t \cos t$$

$$h_y(t) = 3t \sin t$$

$$h_z(t) = 4t$$

---

### Desarrollo paso a paso

#### Cálculo de la Velocidad Instantánea $\mathbf{v}(t)$

La velocidad es la primera derivada del vector de posición $\mathbf{h}(t)$ respecto al tiempo $t$.
$$\mathbf{v}(t) = \frac{d\mathbf{h}}{dt} = \left(\frac{dh_x}{dt}, \frac{dh_y}{dt}, \frac{dh_z}{dt}\right)$$

Se aplica la **regla del producto** $\frac{d}{dt}(f \cdot g) = f'g + fg'$ para las componentes $h_x$ y $h_y$:

$$v_x(t) = \frac{d}{dt}(3t \cos t) = \left(\frac{d}{dt}(3t)\right) \cdot \cos t + 3t \cdot \left(\frac{d}{dt}(\cos t)\right) = 3 \cos t - 3t \sin t$$

$$v_y(t) = \frac{d}{dt}(3t \sin t) = \left(\frac{d}{dt}(3t)\right) \cdot \sin t + 3t \cdot \left(\frac{d}{dt}(\sin t)\right) = 3 \sin t + 3t \cos t$$

$$v_z(t) = \frac{d}{dt}(4t) = 4$$

Agrupando las componentes, el vector velocidad es:
$$\mathbf{v}(t) = (3 \cos t - 3t \sin t, 3 \sin t + 3t \cos t, 4)$$

#### Cálculo de la Aceleración Instantánea $\mathbf{a}(t)$

La aceleración es la primera derivada del vector de velocidad $\mathbf{v}(t)$.
$$\mathbf{a}(t) = \frac{d\mathbf{v}}{dt} = \left(\frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt}\right)$$

Derivamos las componentes de $\mathbf{v}(t)$, aplicando nuevamente la regla del producto:

$$a_x(t) = \frac{d}{dt}(3 \cos t - 3t \sin t) = -3 \sin t - \left( \frac{d}{dt}(3t \sin t) \right) = -3 \sin t - (3 \sin t + 3t \cos t)$$
$$a_x(t) = -6 \sin t - 3t \cos t$$

$$a_y(t) = \frac{d}{dt}(3 \sin t + 3t \cos t) = 3 \cos t + \left( \frac{d}{dt}(3t \cos t) \right) = 3 \cos t + (3 \cos t - 3t \sin t)$$
$$a_y(t) = 6 \cos t - 3t \sin t$$

$$a_z(t) = \frac{d}{dt}(4) = 0$$

El vector aceleración es:
$$\mathbf{a}(t) = (-6 \sin t - 3t \cos t, 6 \cos t - 3t \sin t, 0)$$

#### Cálculo de la Rapidez $\nu(t)$

La rapidez es la magnitud (norma euclidiana) del vector velocidad $\mathbf{v}(t)$.
$$\nu(t) = \|\mathbf{v}(t)\| = \sqrt{[v_x(t)]^2 + [v_y(t)]^2 + [v_z(t)]^2}$$

Sustituimos las componentes de $\mathbf{v}(t)$:
$$\nu(t) = \sqrt{(3 \cos t - 3t \sin t)^2 + (3 \sin t + 3t \cos t)^2 + (4)^2}$$

Expandimos la suma de los cuadrados de las componentes $v_x$ y $v_y$:
$$\begin{aligned} (v_x)^2 + (v_y)^2 = & (9 \cos^2 t - 18t \sin t \cos t + 9t^2 \sin^2 t) \\ + & (9 \sin^2 t + 18t \sin t \cos t + 9t^2 \cos^2 t) \end{aligned}$$

Los términos cruzados ($-18t \sin t \cos t$ y $+18t \sin t \cos t$) se cancelan. Agrupamos los términos restantes:
$$\begin{aligned} (v_x)^2 + (v_y)^2 = & (9 \cos^2 t + 9 \sin^2 t) + (9t^2 \sin^2 t + 9t^2 \cos^2 t) \end{aligned}$$

Aplicamos la identidad pitagórica $\sin^2 t + \cos^2 t = 1$:
$$\begin{aligned} (v_x)^2 + (v_y)^2 = & 9(\cos^2 t + \sin^2 t) + 9t^2(\sin^2 t + \cos^2 t) \\ = & 9(1) + 9t^2(1) \\ = & 9 + 9t^2 \end{aligned}$$

Finalmente, sustituimos este resultado y $(v_z)^2 = 4^2 = 16$ en la raíz cuadrada:
$$\nu(t) = \sqrt{(9 + 9t^2) + 16}$$

$$\nu(t) = \sqrt{25 + 9t^2}$$

---

### Resultado final

Las funciones de movimiento solicitadas son:

**Velocidad Instantánea:**
$$\mathbf{v}(t) = (3 \cos t - 3t \sin t, 3 \sin t + 3t \cos t, 4)$$

**Aceleración Instantánea:**
$$\mathbf{a}(t) = (-6 \sin t - 3t \cos t, 6 \cos t - 3t \sin t, 0)$$

**Rapidez:**
$$\nu(t) = \sqrt{25 + 9t^2}$$

---

### Interpretación breve del resultado

El movimiento describe una hélice cónica (una espiral que se abre) ascendente. La partícula se mueve hacia arriba (eje $z$) a una velocidad constante $v_z=4$, lo cual es consistente con una aceleración nula en dicho eje ($a_z=0$). Simultáneamente, en el plano $xy$, la partícula se aleja del origen (ya que $\nu(t)$ aumenta con $t$) mientras gira.

---

✅ *Cálculos verificados: correctos.*

# Problema 11 inciso 5

### Enunciado del problema

Para una partícula con vector de posición dado por la función vectorial $\mathbf{u}(t) = (3t^2, 2t^3, 3t)$, determine su velocidad instantánea $\mathbf{v}(t)$, su aceleración instantánea $\mathbf{a}(t)$ y su rapidez $\nu(t)$.

---

### Datos dados

El vector de posición de la partícula es $\mathbf{u}(t) = (u_x(t), u_y(t), u_z(t))$, donde las componentes escalares son:

$$u_x(t) = 3t^2$$

$$u_y(t) = 2t^3$$

$$u_z(t) = 3t$$

---

### Desarrollo paso a paso

#### Cálculo de la Velocidad Instantánea $\mathbf{v}(t)$

La velocidad es la primera derivada del vector de posición $\mathbf{u}(t)$ respecto al tiempo $t$.
$$\mathbf{v}(t) = \frac{d\mathbf{u}}{dt} = \left(\frac{du_x}{dt}, \frac{du_y}{dt}, \frac{du_z}{dt}\right)$$

Se aplica la **regla de la potencia** $\frac{d}{dt}(ct^n) = cnt^{n-1}$ a cada componente:

$$v_x(t) = \frac{d}{dt}(3t^2) = 6t$$

$$v_y(t) = \frac{d}{dt}(2t^3) = 6t^2$$

$$v_z(t) = \frac{d}{dt}(3t) = 3$$

El vector velocidad resultante es:
$$\mathbf{v}(t) = (6t, 6t^2, 3)$$

#### Cálculo de la Aceleración Instantánea $\mathbf{a}(t)$

La aceleración es la primera derivada del vector de velocidad $\mathbf{v}(t)$.
$$\mathbf{a}(t) = \frac{d\mathbf{v}}{dt} = \left(\frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt}\right)$$

Derivamos las componentes de $\mathbf{v}(t)$:

$$a_x(t) = \frac{d}{dt}(6t) = 6$$

$$a_y(t) = \frac{d}{dt}(6t^2) = 12t$$

$$a_z(t) = \frac{d}{dt}(3) = 0$$

El vector aceleración resultante es:
$$\mathbf{a}(t) = (6, 12t, 0)$$

#### Cálculo de la Rapidez $\nu(t)$

La rapidez es la magnitud (norma euclidiana) del vector velocidad $\mathbf{v}(t)$.
$$\nu(t) = \|\mathbf{v}(t)\| = \sqrt{[v_x(t)]^2 + [v_y(t)]^2 + [v_z(t)]^2}$$

Sustituimos las componentes de $\mathbf{v}(t)$:
$$\nu(t) = \sqrt{(6t)^2 + (6t^2)^2 + (3)^2}$$

Expandimos y reordenamos los términos:
$$\nu(t) = \sqrt{36t^2 + 36t^4 + 9} = \sqrt{36t^4 + 36t^2 + 9}$$

Factorizamos el $9$ común:
$$\nu(t) = \sqrt{9(4t^4 + 4t^2 + 1)}$$

$$\nu(t) = 3 \sqrt{4t^4 + 4t^2 + 1}$$

El término dentro de la raíz es un **Trinomio Cuadrado Perfecto (TCP)**, ya que sigue la forma $A^2 + 2AB + B^2$ con $A=2t^2$ y $B=1$:
$$(2t^2 + 1)^2 = (2t^2)^2 + 2(2t^2)(1) + (1)^2 = 4t^4 + 4t^2 + 1$$

Sustituimos el TCP en la expresión de la rapidez:
$$\nu(t) = 3 \sqrt{(2t^2 + 1)^2}$$

Dado que $2t^2 + 1$ es siempre positivo para cualquier valor real de $t$, la raíz cuadrada y el cuadrado se simplifican:
$$\nu(t) = 3 (2t^2 + 1)$$

$$\nu(t) = 6t^2 + 3$$

---

### Resultado final

Las funciones de movimiento solicitadas son:

**Velocidad Instantánea:**
$$\mathbf{v}(t) = (6t, 6t^2, 3)$$

**Aceleración Instantánea:**
$$\mathbf{a}(t) = (6, 12t, 0)$$

**Rapidez:**
$$\nu(t) = 6t^2 + 3$$

---

### Interpretación breve del resultado

La partícula se mueve con velocidad constante en el eje $z$ ($v_z=3$), lo cual es coherente con una aceleración nula en dicho eje ($a_z=0$). En el plano $xy$, experimenta una aceleración constante en la componente $x$ ($a_x=6$) y una aceleración variable en la componente $y$ ($a_y=12t$). La rapidez total de la partícula, $\nu(t) = 6t^2 + 3$, es una función cuadrática del tiempo, lo que indica que el movimiento se acelera (aumenta su rapidez) continuamente.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 12

### Enunciado del problema

Demostrar que para cualquier partícula en movimiento, con función de posición $\mathbf{r}(t)$, el producto escalar de los vectores de velocidad y aceleración es igual a la mitad de la derivada de la velocidad al cuadrado. Se debe probar la identidad:
$$\mathbf{v}(t) \cdot \mathbf{a}(t) = \frac{1}{2} \frac{d}{dt} \mathbf{v}^2(t)$$

---

### Datos dados

Se trabaja con las siguientes funciones vectoriales genéricas, asumiendo que $\mathbf{r}(t)$ es al menos dos veces diferenciable:
* **Posición:** $\mathbf{r}(t)$
* **Velocidad:** $\mathbf{v}(t) = \frac{d\mathbf{r}}{dt}$
* **Aceleración:** $\mathbf{a}(t) = \frac{d\mathbf{v}}{dt}$

---

### Desarrollo paso a paso

Se busca demostrar la identidad $\mathbf{v}(t) \cdot \mathbf{a}(t) = \frac{1}{2} \frac{d}{dt} \mathbf{v}^2(t)$. La demostración se realizará partiendo del lado derecho (LD) de la igualdad y, mediante definiciones y reglas de derivación vectorial, se llegará al lado izquierdo (LI).

**Paso 1: Interpretación del Lado Derecho (LD)**

El término $\mathbf{v}^2(t)$ en el LD representa la rapidez al cuadrado (un escalar), $\nu^2(t)$. Esta magnitud al cuadrado se define como el producto escalar del vector velocidad consigo mismo.
$$LD = \frac{1}{2} \frac{d}{dt} \mathbf{v}^2(t) = \frac{1}{2} \frac{d}{dt} [\|\mathbf{v}(t)\|^2]$$

Sustituimos la definición de la norma al cuadrado:
$$LD = \frac{1}{2} \frac{d}{dt} \left[ \mathbf{v}(t) \cdot \mathbf{v}(t) \right]$$

**Paso 2: Aplicación de la Regla del Producto**

Se aplica la regla del producto para la derivada de un producto escalar, que establece: $\frac{d}{dt}[\mathbf{A}(t) \cdot \mathbf{B}(t)] = \mathbf{A}'(t) \cdot \mathbf{B}(t) + \mathbf{A}(t) \cdot \mathbf{B}'(t)$.

Aplicando esta regla a nuestra expresión:
$$LD = \frac{1}{2} \left[ \left(\frac{d\mathbf{v}}{dt}\right) \cdot \mathbf{v}(t) + \mathbf{v}(t) \cdot \left(\frac{d\mathbf{v}}{dt}\right) \right]$$

**Paso 3: Sustitución de la definición de Aceleración**

Reconocemos que la derivada del vector velocidad es, por definición, el vector aceleración: $\mathbf{a}(t) = \frac{d\mathbf{v}}{dt}$.

Sustituimos $\mathbf{a}(t)$ en la expresión:
$$LD = \frac{1}{2} \left[ \mathbf{a}(t) \cdot \mathbf{v}(t) + \mathbf{v}(t) \cdot \mathbf{a}(t) \right]$$

**Paso 4: Simplificación usando Conmutatividad**

El producto escalar es conmutativo, lo que significa que $\mathbf{A} \cdot \mathbf{B} = \mathbf{B} \cdot \mathbf{A}$. Por lo tanto, podemos reescribir el primer término:
$$\mathbf{a}(t) \cdot \mathbf{v}(t) = \mathbf{v}(t) \cdot \mathbf{a}(t)$$

Sustituimos esto en la ecuación:
$$LD = \frac{1}{2} \left[ \mathbf{v}(t) \cdot \mathbf{a}(t) + \mathbf{v}(t) \cdot \mathbf{a}(t) \right]$$

**Paso 5: Simplificación final**

Sumamos los dos términos idénticos dentro del corchete:
$$LD = \frac{1}{2} \left[ 2 \cdot (\mathbf{v}(t) \cdot \mathbf{a}(t)) \right]$$

$$LD = \mathbf{v}(t) \cdot \mathbf{a}(t)$$

---

### Resultado final

Hemos demostrado que el Lado Derecho (LD) de la ecuación es idéntico al Lado Izquierdo (LI):
$$LD = \mathbf{v}(t) \cdot \mathbf{a}(t) = LI$$

Por lo tanto, la identidad queda demostrada:
$$\mathbf{v}(t) \cdot \mathbf{a}(t) = \frac{1}{2} \frac{d}{dt} \mathbf{v}^2(t)$$
*Q.E.D. (Lo Que Queda Demostrado).*

---

### Interpretación breve del resultado

Esta identidad es fundamental en física. El término $\frac{1}{2} \mathbf{v}^2(t)$ (o más comúnmente $\frac{1}{2} \nu^2$) representa la energía cinética por unidad de masa. La derivada de esta cantidad, $\frac{d}{dt} (\frac{1}{2} \nu^2)$, es la tasa de cambio de la energía cinética (por unidad de masa).

La demostración prueba que esta tasa de cambio es exactamente igual al producto escalar $\mathbf{v} \cdot \mathbf{a}$. Esto significa que el cambio en la rapidez (y por ende en la energía cinética) de una partícula solo es afectado por la componente de la aceleración que actúa en la misma dirección (o dirección opuesta) que la velocidad.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 13 inciso 1

### Enunciado del problema

Para una partícula con función de aceleración dada por $\mathbf{a}(t) = (1, 1, 1)$, calcule su vector velocidad $\mathbf{v}(t)$ y su vector de posición $\mathbf{r}(t)$, dadas las condiciones iniciales $\mathbf{v}(0) = (0, 0, 0)$ y $\mathbf{r}(0) = (0, 0, 0)$.

---

### Datos dados

Las condiciones del problema de valor inicial son:

**Función de Aceleración:**
$$\mathbf{a}(t) = (1, 1, 1)$$

**Condición Inicial de Velocidad:**
$$\mathbf{v}(0) = (0, 0, 0)$$

**Condición Inicial de Posición:**
$$\mathbf{r}(0) = (0, 0, 0)$$

---

### Desarrollo paso a paso

Este problema se resuelve mediante integración secuencial (antiderivación) componente a componente, aplicando las condiciones iniciales para encontrar las constantes de integración.

#### Cálculo del Vector Velocidad $\mathbf{v}(t)$

La velocidad $\mathbf{v}(t)$ se obtiene integrando la aceleración $\mathbf{a}(t)$ respecto al tiempo $t$.
$$\mathbf{v}(t) = \int \mathbf{a}(t) dt = \int (1, 1, 1) dt$$

Al integrar componente a componente, se obtiene la familia de soluciones para la velocidad, introduciendo un vector constante de integración $\mathbf{C}_1$:
$$\mathbf{v}(t) = \left( \int 1 dt, \int 1 dt, \int 1 dt \right) + \mathbf{C}_1$$

$$\mathbf{v}(t) = (t + C_{1x}, t + C_{1y}, t + C_{1z}) = (t, t, t) + \mathbf{C}_1$$

Ahora, aplicamos la condición inicial $\mathbf{v}(0) = (0, 0, 0)$ para encontrar $\mathbf{C}_1$:
$$\mathbf{v}(0) = (0, 0, 0) + \mathbf{C}_1 = (0, 0, 0)$$

De lo cual se deduce que $\mathbf{C}_1 = (0, 0, 0)$. Por lo tanto, la solución particular para la velocidad es:
$$\mathbf{v}(t) = (t, t, t)$$

#### Cálculo del Vector Posición $\mathbf{r}(t)$

La posición $\mathbf{r}(t)$ se obtiene integrando la solución particular de la velocidad $\mathbf{v}(t)$.
$$\mathbf{r}(t) = \int \mathbf{v}(t) dt = \int (t, t, t) dt$$

Al integrar, introducimos un segundo vector constante de integración $\mathbf{C}_2$:
$$\mathbf{r}(t) = \left( \int t dt, \int t dt, \int t dt \right) + \mathbf{C}_2$$

$$\mathbf{r}(t) = \left(\frac{t^2}{2} + C_{2x}, \frac{t^2}{2} + C_{2y}, \frac{t^2}{2} + C_{2z}\right) = \left(\frac{t^2}{2}, \frac{t^2}{2}, \frac{t^2}{2}\right) + \mathbf{C}_2$$

Aplicamos la condición inicial $\mathbf{r}(0) = (0, 0, 0)$ para encontrar $\mathbf{C}_2$:
$$\mathbf{r}(0) = (0, 0, 0) + \mathbf{C}_2 = (0, 0, 0)$$

De lo cual se deduce que $\mathbf{C}_2 = (0, 0, 0)$. La solución particular para la posición es:
$$\mathbf{r}(t) = \left(\frac{t^2}{2}, \frac{t^2}{2}, \frac{t^2}{2}\right)$$

---

### Resultado final

Las funciones vectoriales específicas (soluciones particulares) que satisfacen las condiciones dadas son:

**Vector Velocidad:**
$$\mathbf{v}(t) = (t, t, t)$$

**Vector Posición:**
$$\mathbf{r}(t) = \left(\frac{t^2}{2}, \frac{t^2}{2}, \frac{t^2}{2}\right)$$

---

### Interpretación breve del resultado

La partícula parte del origen ($\mathbf{r}(0) = (0, 0, 0)$) y en reposo ($\mathbf{v}(0) = (0, 0, 0)$). Al estar sujeta a una aceleración constante $\mathbf{a}(t) = (1, 1, 1)$, su movimiento describe un **movimiento rectilíneo uniformemente acelerado (MRUA)**. La trayectoria de la partícula es una línea recta que avanza en la dirección del vector $(1, 1, 1)$.

---

✅ *Cálculos verificados: correctos.*

# Problema 13 inciso 5

### Enunciado del problema

Para una partícula con función de aceleración dada por $\mathbf{a}(t) = -\cos t \, \mathbf{i} - \sin t \, \mathbf{j}$, calcule su vector velocidad $\mathbf{v}(t)$ y su vector de posición $\mathbf{r}(t)$, dadas las condiciones iniciales $\mathbf{v}(0) = \mathbf{j} + \mathbf{k}$ y $\mathbf{r}(0) = \mathbf{i}$.

---

### Datos dados

Las condiciones del problema de valor inicial se expresan en notación vectorial y de tuplas:

**Función de Aceleración:**
$$\mathbf{a}(t) = -\cos t \, \mathbf{i} - \sin t \, \mathbf{j} \quad \text{o} \quad \mathbf{a}(t) = (-\cos t, -\sin t, 0)$$

**Condición Inicial de Velocidad:**
$$\mathbf{v}(0) = \mathbf{j} + \mathbf{k} \quad \text{o} \quad \mathbf{v}(0) = (0, 1, 1)$$

**Condición Inicial de Posición:**
$$\mathbf{r}(0) = \mathbf{i} \quad \text{o} \quad \mathbf{r}(0) = (1, 0, 0)$$

---

### Desarrollo paso a paso

Se resuelve mediante integración secuencial (antiderivación) componente a componente, aplicando las condiciones iniciales para encontrar las constantes de integración.

#### Cálculo del Vector Velocidad $\mathbf{v}(t)$

La velocidad $\mathbf{v}(t)$ se obtiene integrando la aceleración $\mathbf{a}(t)$.
$$\mathbf{v}(t) = \int \mathbf{a}(t) dt = \int (-\cos t, -\sin t, 0) dt$$

Al integrar, se obtiene la familia de soluciones introduciendo el vector constante $\mathbf{C}_1 = (C_{1x}, C_{1y}, C_{1z})$:
$$\mathbf{v}(t) = \left( \int (-\cos t) dt, \int (-\sin t) dt, \int 0 dt \right) + \mathbf{C}_1$$

$$\mathbf{v}(t) = (-\sin t + C_{1x}, \cos t + C_{1y}, 0 + C_{1z})$$

Aplicamos la condición inicial $\mathbf{v}(0) = (0, 1, 1)$:
$$\mathbf{v}(0) = (-\sin 0 + C_{1x}, \cos 0 + C_{1y}, C_{1z})$$

$$\mathbf{v}(0) = (0 + C_{1x}, 1 + C_{1y}, C_{1z})$$

Igualamos a la condición inicial $(0, 1, 1)$:
$$(C_{1x}, 1 + C_{1y}, C_{1z}) = (0, 1, 1)$$

Resolviendo para las constantes:
* $C_{1x} = 0$
* $1 + C_{1y} = 1 \implies C_{1y} = 0$
* $C_{1z} = 1$

La solución particular para la velocidad es:
$$\mathbf{v}(t) = (-\sin t, \cos t, 1)$$

#### Cálculo del Vector Posición $\mathbf{r}(t)$

La posición $\mathbf{r}(t)$ se obtiene integrando la solución particular de la velocidad $\mathbf{v}(t)$.
$$\mathbf{r}(t) = \int \mathbf{v}(t) dt = \int (-\sin t, \cos t, 1) dt$$

Introducimos el segundo vector constante $\mathbf{C}_2 = (C_{2x}, C_{2y}, C_{2z})$:
$$\mathbf{r}(t) = \left( \int (-\sin t) dt, \int \cos t dt, \int 1 dt \right) + \mathbf{C}_2$$

$$\mathbf{r}(t) = (\cos t + C_{2x}, \sin t + C_{2y}, t + C_{2z})$$

Aplicamos la condición inicial $\mathbf{r}(0) = (1, 0, 0)$:
$$\mathbf{r}(0) = (\cos 0 + C_{2x}, \sin 0 + C_{2y}, 0 + C_{2z})$$

$$\mathbf{r}(0) = (1 + C_{2x}, 0 + C_{2y}, C_{2z})$$

Igualamos a la condición inicial $(1, 0, 0)$:
$$(1 + C_{2x}, C_{2y}, C_{2z}) = (1, 0, 0)$$

Resolviendo para las constantes:
* $1 + C_{2x} = 1 \implies C_{2x} = 0$
* $C_{2y} = 0$
* $C_{2z} = 0$

La solución particular para la posición es:
$$\mathbf{r}(t) = (\cos t, \sin t, t)$$

---

### Resultado final

Las funciones vectoriales específicas (soluciones particulares) que satisfacen las condiciones dadas son:

**Vector Velocidad:**
$$\mathbf{v}(t) = -\sin t \, \mathbf{i} + \cos t \, \mathbf{j} + \mathbf{k}$$

**Vector Posición:**
$$\mathbf{r}(t) = \cos t \, \mathbf{i} + \sin t \, \mathbf{j} + t\mathbf{k}$$

---

### Interpretación breve del resultado

El movimiento resultante es una **hélice circular**. La partícula describe un círculo de radio 1 en el plano $xy$ (componentes $\cos t \, \mathbf{i} + \sin t \, \mathbf{j}$) mientras se mueve simultáneamente a una velocidad constante $v_z = 1$ (componente $\mathbf{k}$ en $\mathbf{v}(t)$), lo que resulta en un desplazamiento lineal a lo largo del eje $z$ (componente $t\mathbf{k}$ en $\mathbf{r}(t)$).

---

✅ *Cálculos verificados: correctos.*

---
# Problema 14

### Enunciado del problema

Una pelota de béisbol es golpeada a $3 \text{ pies}$ sobre el nivel del suelo. Se aleja del bate con un ángulo de $45^\circ$ y es cachada por un jardinero a $3 \text{ pies}$ sobre el nivel del suelo y a $300 \text{ pies}$ del plato de lanzamiento.

Se busca calcular la rapidez inicial ($\nu_0$) y la altura máxima alcanzada ($y_{max}$).

---

### Datos dados

Dadas las condiciones del movimiento parabólico en el sistema imperial:

* **Posición inicial:** $(x_0, y_0) = (0, 3) \text{ pies}$.
* **Posición final (captura):** $(x_f, y_f) = (300, 3) \text{ pies}$.
* **Simetría de altura:** $y_0 = y_f = 3 \text{ pies}$.
* **Rango (Alcance):** $R = x_f - x_0 = 300 \text{ pies}$.
* **Ángulo de lanzamiento:** $\theta = 45^\circ$.
* **Aceleración gravitacional:** $g = 32 \text{ pies/s}^2$.

---

### Desarrollo paso a paso

Dado que la altura inicial ($y_0$) y la altura final ($y_f$) son idénticas, el problema es simétrico. Esto permite el uso de las fórmulas estándar de alcance y altura máxima (relativa al lanzamiento) para un tiro parabólico simétrico.

#### 1. Cálculo de la Rapidez Inicial ($\nu_0$)

Se utiliza la ecuación de rango (alcance) para un tiro parabólico donde $y_f = y_0$:
$$R = \frac{\nu_0^2 \sin(2\theta)}{g}$$

Sustituimos los valores conocidos ($R = 300$, $\theta = 45^\circ$, $g = 32$):
$$300 = \frac{\nu_0^2 \sin(2 \times 45^\circ)}{32}$$

Calculamos el término trigonométrico:
$$\sin(2 \times 45^\circ) = \sin(90^\circ) = 1$$

Sustituimos este resultado en la ecuación:
$$300 = \frac{\nu_0^2 \cdot 1}{32}$$

Despejamos $\nu_0^2$:
$$\nu_0^2 = 300 \times 32$$
$$\nu_0^2 = 9600 \text{ (pies/s)}^2$$

Calculamos la rapidez inicial $\nu_0$:
$$\nu_0 = \sqrt{9600} \text{ pies/s}$$
$$\nu_0 \approx 97.98 \text{ pies/s}$$

#### 2. Cálculo de la Altura Máxima ($y_{max}$)

La altura máxima ($y_{max}$) es la altura inicial ($y_0$) más el desplazamiento vertical máximo ($\Delta y_{max}$) alcanzado desde el punto de lanzamiento.
$$y_{max} = y_0 + \Delta y_{max}$$

La fórmula para el desplazamiento vertical máximo en un tiro simétrico es:
$$\Delta y_{max} = \frac{(\nu_0 \sin \theta)^2}{2g}$$

Para mayor precisión, reescribimos la fórmula usando $\nu_0^2$, que ya calculamos:
$$y_{max} = y_0 + \frac{\nu_0^2 (\sin \theta)^2}{2g}$$

Sustituimos los valores ($y_0 = 3$, $\nu_0^2 = 9600$, $\theta = 45^\circ$, $g = 32$):
$$y_{max} = 3 + \frac{9600 \cdot (\sin 45^\circ)^2}{2(32)}$$

Calculamos el término $(\sin 45^\circ)^2$:
$$(\sin 45^\circ)^2 = \left(\frac{\sqrt{2}}{2}\right)^2 = \frac{2}{4} = \frac{1}{2}$$

Sustituimos y resolvemos:
$$y_{max} = 3 + \frac{9600 \cdot (1/2)}{64}$$

$$y_{max} = 3 + \frac{4800}{64}$$

$$y_{max} = 3 + 75$$

$$y_{max} = 78 \text{ pies}$$

---

### Resultado final

**Rapidez Inicial:**
$$\nu_0 = \sqrt{9600} \text{ pies/s} \approx 97.98 \text{ pies/s}$$

**Altura Máxima:**
$$y_{max} = 78 \text{ pies}$$

---

### Interpretación breve del resultado

La pelota fue golpeada con una rapidez inicial de aproximadamente $98 \text{ pies/s}$ (cerca de $67 \text{ mph}$), lo cual es una velocidad de salida razonable en béisbol. Alcanzó una altura máxima total de $78 \text{ pies}$ sobre el nivel del suelo antes de descender y ser atrapada a $300 \text{ pies}$ de distancia, a la misma altura a la que fue bateada.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 15 

### Enunciado del problema

Un proyectil se lanza desde el suelo con un ángulo de $12^\circ$ con la horizontal. El proyectil debe tener un alcance de $200 \text{ pies}$. Halle la velocidad inicial mínima requerida.

---

### Datos dados

Dadas las condiciones del movimiento parabólico en el sistema imperial:

* **Alcance (Rango):** $R = 200 \text{ pies}$.
* **Ángulo de lanzamiento:** $\theta = 12^\circ$.
* **Simetría de altura:** $y_0 = y_f = 0 \text{ pies}$ (lanzamiento "desde el suelo").
* **Aceleración gravitacional:** $g = 32 \text{ pies/s}^2$.

---

### Desarrollo paso a paso

El problema describe un movimiento parabólico simétrico, ya que la altura de lanzamiento y la de aterrizaje son idénticas ($y_0 = y_f = 0$). Por lo tanto, se puede utilizar la ecuación de rango (alcance) estándar:

$$R = \frac{\nu_0^2 \sin(2\theta)}{g}$$

El objetivo es despejar la rapidez inicial ($\nu_0$) de esta ecuación.

$$\nu_0^2 = \frac{R \cdot g}{\sin(2\theta)}$$

$$\nu_0 = \sqrt{\frac{R \cdot g}{\sin(2\theta)}}$$

Sustituimos los valores dados ($R = 200 \text{ pies}$, $g = 32 \text{ pies/s}^2$, $\theta = 12^\circ$):

$$\nu_0 = \sqrt{\frac{200 \times 32}{\sin(2 \times 12^\circ)}}$$

$$\nu_0 = \sqrt{\frac{6400}{\sin(24^\circ)}}$$

Calculamos el valor del seno:

$$\sin(24^\circ) \approx 0.406737$$

Realizamos el cálculo final:

$$\nu_0 \approx \sqrt{\frac{6400}{0.406737}}$$

$$\nu_0 \approx \sqrt{15735.33}$$

$$\nu_0 \approx 125.44 \text{ pies/s}$$

---

### Resultado final

La velocidad inicial (rapidez) requerida es:

$$\nu_0 \approx 125.44 \text{ pies/s}$$

---

### Interpretación breve del resultado

La velocidad inicial mínima requerida para lograr un alcance de $200 \text{ pies}$ con un ángulo de $12^\circ$ es aproximadamente $125.44 \text{ pies/s}$. Dado que el ángulo de lanzamiento está fijo, el término "velocidad inicial mínima" se refiere a la única rapidez $\nu_0$ que satisface estas condiciones.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 16 

### Enunciado del problema

Un satélite de comunicaciones tiene una órbita circular $250 \text{ km}$ arriba de la superficie de la tierra (cuyo radio es aproximadamente de $6400 \text{ km}$). Calcula su rapidez y el tiempo que tarda en dar una vuelta completa.

---

### Datos dados

* **Altura orbital:** $h = 250 \text{ km}$
* **Radio de la Tierra:** $R_T = 6400 \text{ km}$
* **Parámetro gravitacional estándar de la Tierra (implícito):** $\mu = G \cdot M_T \approx 3.986 \times 10^{14} \text{ m}^3/\text{s}^2$
* **Condición:** Órbita circular (Fuerza gravitacional = Fuerza centrípeta).

---

### Desarrollo paso a paso

#### 1. Cálculo del Radio Orbital ($r$)

El radio orbital total ($r$) se mide desde el centro de la Tierra hasta el satélite. Es la suma del radio de la Tierra y la altura orbital.
$$r = R_T + h$$

Convertimos todas las distancias al Sistema Internacional (SI) en metros:
$R_T = 6400 \text{ km} = 6.40 \times 10^6 \text{ m}$
$h = 250 \text{ km} = 0.25 \times 10^6 \text{ m}$

$$r = (6.40 \times 10^6 \text{ m}) + (0.25 \times 10^6 \text{ m})$$
$$r = 6.65 \times 10^6 \text{ m}$$

#### 2. Cálculo de la Rapidez Orbital ($\nu$)

En una órbita circular estable, la fuerza de gravedad ($F_g$) que atrae al satélite es igual a la fuerza centrípeta ($F_c$) requerida para mantenerlo en movimiento circular.
$$F_g = F_c$$

$$G \frac{M_T m}{r^2} = \frac{m \nu^2}{r}$$

Donde $G$ es la constante gravitacional, $M_T$ la masa de la Tierra y $m$ la masa del satélite. La masa del satélite ($m$) y un factor de $r$ se cancelan en ambos lados:
$$\frac{G M_T}{r} = \nu^2$$

Usamos el parámetro gravitacional estándar $\mu = G M_T$:
$$\nu^2 = \frac{\mu}{r} \implies \nu = \sqrt{\frac{\mu}{r}}$$

Sustituimos los valores de $\mu$ y $r$:
$$\nu = \sqrt{\frac{3.986 \times 10^{14} \text{ m}^3/\text{s}^2}{6.65 \times 10^6 \text{ m}}}$$
$$\nu \approx \sqrt{5.99398... \times 10^7} \text{ m/s}$$
$$\nu \approx 7742.1 \text{ m/s}$$

#### 3. Cálculo del Periodo Orbital ($T$)

El periodo ($T$) es el tiempo que tarda en completar una órbita. Se calcula dividiendo la distancia de la órbita (la circunferencia, $2\pi r$) por la rapidez orbital ($\nu$).
$$T = \frac{2\pi r}{\nu}$$

Sustituimos los valores (utilizando el valor de $\nu$ con mayor precisión para el cálculo intermedio):
$$T = \frac{2 \pi (6.65 \times 10^6 \text{ m})}{7742.1 \text{ m/s}}$$
$$T \approx 5396.9 \text{ s}$$

---

### Resultado final

Los resultados se redondean a 3 cifras significativas, de acuerdo con la precisión del radio orbital calculado ($r = 6.65 \times 10^6 \text{ m}$).

**Rapidez del Satélite:**
$$\nu \approx 7.74 \times 10^3 \text{ m/s} \quad (\text{ó } 7.74 \text{ km/s})$$

**Tiempo de una Vuelta Completa (Periodo):**
$$T \approx 5397 \text{ s}$$
$$T \approx 5.40 \times 10^3 \text{ s}$$

---

### Interpretación breve del resultado

La rapidez del satélite es de aproximadamente $7.74 \times 10^3 \text{ m/s}$ ($7.74 \text{ km/s}$) y tarda aproximadamente $5.40 \times 10^3$ segundos (o $90.0$ minutos) en completar una órbita alrededor de la Tierra. Esta rapidez y periodo son característicos de la Órbita Terrestre Baja (LEO).

---

✅ *Cálculos verificados: correctos.*

---
# Problema 17 

### Enunciado del problema

Un satélite que tiene una órbita circular da una vuelta alrededor de la Tierra cada $88 \text{ min}$. Halla la altura del satélite con respecto a la superficie terrestre.

---

### Datos dados

* **Periodo orbital:** $T = 88 \text{ min}$
* **Parámetro gravitacional estándar de la Tierra (implícito):** $\mu = G \cdot M_T \approx 3.986 \times 10^{14} \text{ m}^3/\text{s}^2$
* **Radio de la Tierra (implícito):** $R_T \approx 6400 \text{ km} = 6.40 \times 10^6 \text{ m}$

---

### Desarrollo paso a paso

El problema se resuelve utilizando la Tercera Ley de Kepler para órbitas circulares, que relaciona el periodo ($T$) con el radio orbital total ($r$).

#### 1. Conversión de Unidades (Periodo $T$)

Primero, se convierte el periodo orbital $T$ de minutos a segundos (unidades SI):
$$T = 88 \text{ min} \times \frac{60 \text{ s}}{1 \text{ min}} = 5280 \text{ s}$$

#### 2. Cálculo del Radio Orbital Total ($r$)

La Tercera Ley de Kepler establece:
$$T^2 = \left(\frac{4\pi^2}{\mu}\right) r^3$$

Despejamos el radio orbital $r$:
$$r^3 = \frac{\mu T^2}{4\pi^2}$$

$$r = \sqrt[3]{\frac{\mu T^2}{4\pi^2}}$$

Sustituimos los valores conocidos:
$$r = \sqrt[3]{\frac{(3.986 \times 10^{14} \text{ m}^3/\text{s}^2) \times (5280 \text{ s})^2}{4\pi^2}}$$

$$r = \sqrt[3]{\frac{(3.986 \times 10^{14}) \times (27,878,400)}{4\pi^2}}$$

$$r \approx \sqrt[3]{\frac{1.1112 \times 10^{22}}{39.478}}$$

$$r \approx \sqrt[3]{2.8147 \times 10^{20}} \text{ m}^3$$

$$r \approx 6.553 \times 10^6 \text{ m (ó 6553 km)}$$

#### 3. Cálculo de la Altura ($h$)

La altura $h$ es la diferencia entre el radio orbital total ($r$) y el radio de la Tierra ($R_T$).
$$h = r - R_T$$

$$h \approx (6.553 \times 10^6 \text{ m}) - (6.40 \times 10^6 \text{ m})$$

$$h \approx 0.153 \times 10^6 \text{ m}$$

$$h \approx 153 \text{ km}$$

---

### Resultado final

El cálculo produce una altura de $h \approx 153 \text{ km}$. Sin embargo, el dato de entrada ($T = 88 \text{ min}$) tiene solo dos cifras significativas. Por lo tanto, el resultado final debe redondearse a dos cifras significativas:

$$h \approx 150 \text{ km}$$

---

### Interpretación breve del resultado

Un periodo de $88 \text{ minutos}$ es extremadamente rápido (más corto que el de la Estación Espacial Internacional), lo que implica una Órbita Terrestre Baja (LEO) muy baja. La altura calculada de aproximadamente $150 \text{ km}$ es coherente con este periodo tan corto.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 18 inciso 2

### Enunciado del problema

Determine la longitud de arco de la curva paramétrica $\mathbf{g}(t) = (t, \ln(\sec t), \ln(\sec t + \tan t))$, donde $t \in [0, \pi/4]$.

---

### Datos dados

La curva es una función vectorial $\mathbf{g}(t) = (x(t), y(t), z(t))$ con las componentes:

$$x(t) = t$$

$$y(t) = \ln(\sec t)$$

$$z(t) = \ln(\sec t + \tan t)$$

El intervalo de integración es $t \in [0, \pi/4]$.

---

### Desarrollo paso a paso

La longitud de arco ($L$) se calcula usando la fórmula integral:
$$L = \int_{a}^{b} \|\mathbf{g}'(t)\| dt = \int_{a}^{b} \sqrt{[x'(t)]^2 + [y'(t)]^2 + [z'(t)]^2} dt$$

#### 1. Cálculo del Vector Derivado $\mathbf{g}'(t)$

Primero, calculamos la derivada de cada componente:

$$x'(t) = \frac{d}{dt}(t) = 1$$

$$y'(t) = \frac{d}{dt}(\ln(\sec t)) = \frac{1}{\sec t} \cdot \frac{d}{dt}(\sec t) = \frac{1}{\sec t} \cdot (\sec t \tan t) = \tan t$$

$$z'(t) = \frac{d}{dt}(\ln(\sec t + \tan t)) = \frac{1}{\sec t + \tan t} \cdot \frac{d}{dt}(\sec t + \tan t)$$

$$z'(t) = \frac{1}{\sec t + \tan t} \cdot (\sec t \tan t + \sec^2 t)$$

Factorizando $\sec t$ en el numerador:
$$z'(t) = \frac{\sec t (\tan t + \sec t)}{\sec t + \tan t} = \sec t$$

Por lo tanto, el vector derivado es:
$$\mathbf{g}'(t) = (1, \tan t, \sec t)$$

#### 2. Cálculo de la Magnitud (Norma) $\|\mathbf{g}'(t)\|$

A continuación, calculamos la magnitud (norma) de este vector:
$$\|\mathbf{g}'(t)\| = \sqrt{(1)^2 + (\tan t)^2 + (\sec t)^2}$$

$$\|\mathbf{g}'(t)\| = \sqrt{1 + \tan^2 t + \sec^2 t}$$

Usamos la identidad pitagórica fundamental $1 + \tan^2 t = \sec^2 t$:
$$\|\mathbf{g}'(t)\| = \sqrt{(\sec^2 t) + \sec^2 t}$$

$$\|\mathbf{g}'(t)\| = \sqrt{2 \sec^2 t} = \sqrt{2} \cdot \sqrt{\sec^2 t} = \sqrt{2} |\sec t|$$

En el intervalo de integración $t \in [0, \pi/4]$, la función $\cos t$ es positiva, por lo tanto $\sec t = 1/\cos t$ también es positiva. Esto nos permite eliminar el valor absoluto:
$$\|\mathbf{g}'(t)\| = \sqrt{2} \sec t$$

#### 3. Cálculo de la Integral de Longitud de Arco $L$

Finalmente, integramos la magnitud desde $a=0$ hasta $b=\pi/4$:
$$L = \int_{0}^{\pi/4} \sqrt{2} \sec t \, dt$$

$$L = \sqrt{2} \int_{0}^{\pi/4} \sec t \, dt$$

La antiderivada conocida de $\sec t$ es $\ln|\sec t + \tan t|$:
$$L = \sqrt{2} \left[ \ln|\sec t + \tan t| \right]_{0}^{\pi/4}$$

Evaluamos en los límites de integración (Regla de Barrow):
$$L = \sqrt{2} \left( \ln|\sec(\pi/4) + \tan(\pi/4)| - \ln|\sec(0) + \tan(0)| \right)$$

Sustituimos los valores trigonométricos:
* $\sec(\pi/4) = \sqrt{2}$
* $\tan(\pi/4) = 1$
* $\sec(0) = 1$
* $\tan(0) = 0$

$$L = \sqrt{2} \left( \ln|\sqrt{2} + 1| - \ln|1 + 0| \right)$$

$$L = \sqrt{2} \left( \ln(\sqrt{2} + 1) - \ln(1) \right)$$

Dado que $\ln(1) = 0$:
$$L = \sqrt{2} \left( \ln(\sqrt{2} + 1) - 0 \right)$$

---

### Resultado final

La longitud de arco exacta de la curva en el intervalo dado es:
$$L = \sqrt{2} \ln(\sqrt{2} + 1)$$

---

### Interpretación breve del resultado

El valor $L = \sqrt{2} \ln(\sqrt{2} + 1)$ (aproximadamente $1.246$ unidades) es la longitud escalar exacta de la trayectoria descrita por la función $\mathbf{g}(t)$ desde $t=0$ hasta $t=\pi/4$.

---

✅ *Cálculos verificados: correctos.*

# Problema 18 inciso 3

### Enunciado del problema

Determine la longitud de arco de la curva paramétrica $\mathbf{h}(t) = (a \cos \omega t, a \sin \omega t, b\omega)$, donde $t \in [t_0, t_1]$.

---

### Datos dados

La función vectorial es $\mathbf{h}(t)$, y el intervalo de integración es $[t_0, t_1]$.
Las variables $a$, $b$, $\omega$, $t_0$, y $t_1$ son constantes.

---

### Desarrollo paso a paso

**Nota sobre la función (Hipótesis de corrección)**

El enunciado original $\mathbf{h}(t) = (a \cos \omega t, a \sin \omega t, b\omega)$ posee una componente $z(t) = b\omega$ que es constante. Esto describiría un arco de círculo de radio $a$ en el plano horizontal $z=b\omega$ (ya que $z'(t) = 0$).

Siguiendo el análisis del prompt, se asume que existe un error tipográfico y que la función destinada al análisis es la **hélice circular** estándar, la cual es una curva tridimensional más compleja:
$$\mathbf{h}(t) = (a \cos \omega t, a \sin \omega t, b\omega t)$$
El siguiente desarrollo se basa en esta función corregida.

**1. Cálculo del Vector Derivado $\mathbf{h}'(t)$**

Se deriva la función $\mathbf{h}(t) = (a \cos \omega t, a \sin \omega t, b\omega t)$ componente a componente:
$$x'(t) = \frac{d}{dt}(a \cos \omega t) = -a\omega \sin \omega t$$

$$y'(t) = \frac{d}{dt}(a \sin \omega t) = a\omega \cos \omega t$$

$$z'(t) = \frac{d}{dt}(b\omega t) = b\omega$$

El vector derivado (velocidad) es:
$$\mathbf{h}'(t) = (-a\omega \sin \omega t, a\omega \cos \omega t, b\omega)$$

**2. Cálculo de la Magnitud (Rapidez) $\|\mathbf{h}'(t)\|$**

Se calcula la norma (magnitud) del vector derivado:
$$\|\mathbf{h}'(t)\| = \sqrt{[x'(t)]^2 + [y'(t)]^2 + [z'(t)]^2}$$

$$\|\mathbf{h}'(t)\| = \sqrt{(-a\omega \sin \omega t)^2 + (a\omega \cos \omega t)^2 + (b\omega)^2}$$

$$\|\mathbf{h}'(t)\| = \sqrt{a^2\omega^2 \sin^2 \omega t + a^2\omega^2 \cos^2 \omega t + b^2\omega^2}$$

Se factoriza $a^2\omega^2$ y se aplica la identidad trigonométrica $\sin^2 \theta + \cos^2 \theta = 1$:
$$\|\mathbf{h}'(t)\| = \sqrt{a^2\omega^2 (\sin^2 \omega t + \cos^2 \omega t) + b^2\omega^2}$$

$$\|\mathbf{h}'(t)\| = \sqrt{a^2\omega^2 (1) + b^2\omega^2}$$

Se factoriza $\omega^2$ del radical:
$$\|\mathbf{h}'(t)\| = \sqrt{\omega^2 (a^2 + b^2)}$$

$$\|\mathbf{h}'(t)\| = |\omega| \sqrt{a^2 + b^2}$$

**3. Cálculo de la Integral de Longitud de Arco $L$**

La magnitud $\|\mathbf{h}'(t)\|$ (la rapidez) es un valor constante, ya que $a$, $b$ y $\omega$ son constantes.
$$L = \int_{t_0}^{t_1} \|\mathbf{h}'(t)\| dt = \int_{t_0}^{t_1} |\omega| \sqrt{a^2 + b^2} \, dt$$

Como el integrando es constante, la integral es el producto del integrando por la longitud del intervalo de integración $(t_1 - t_0)$:
$$L = \left( |\omega| \sqrt{a^2 + b^2} \right) \int_{t_0}^{t_1} 1 \, dt$$

$$L = \left( |\omega| \sqrt{a^2 + b^2} \right) \left[ t \right]_{t_0}^{t_1}$$

$$L = \left( |\omega| \sqrt{a^2 + b^2} \right) (t_1 - t_0)$$

---

### Resultado final

La longitud de arco de la hélice circular (basada en la corrección del enunciado) en el intervalo $t \in [t_0, t_1]$ es:
$$L = |\omega| \sqrt{a^2 + b^2} (t_1 - t_0)$$

---

### Interpretación breve del resultado

La longitud de arco de esta hélice es simplemente el producto de su rapidez constante, $v = |\omega| \sqrt{a^2 + b^2}$, y el tiempo transcurrido, $\Delta t = (t_1 - t_0)$. Esto es coherente, ya que la longitud de un camino recorrido a velocidad constante es $L = v \cdot \Delta t$.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 19

### Enunciado del problema

Si $\mathbf{r}(t)$ es una curva con derivada continua definida en el intervalo $[a, b]$, muestre que la derivada de la función de longitud de arco ($s$) con respecto al parámetro ($t$) es igual a la norma de la derivada del vector de posición $\mathbf{r}(t)$.

Demostrar la identidad:
$$\frac{ds}{dt} = \|\mathbf{r}'(t)\|$$

---

### Datos dados

* **Curva:** $\mathbf{r}(t)$ (Función vectorial de posición).
* **Función de longitud de arco:** $s(t)$.
* **Parámetro:** $t \in [a, b]$.
* **Condición:** $\mathbf{r}'(t)$ es continua en $[a, b]$ (la curva es $C^1$ o "suave").

---

### Desarrollo paso a paso

La demostración se basa en la definición formal de la función de longitud de arco y la aplicación directa del Teorema Fundamental del Cálculo (TFC).

**1. Definición de la Función Longitud de Arco $s(t)$**

La función de longitud de arco, $s(t)$, mide la distancia recorrida a lo largo de la curva desde un punto de inicio fijo $\mathbf{r}(a)$ hasta un punto arbitrario $\mathbf{r}(t)$.

Se define como la integral de la rapidez (la norma de la derivada del vector de posición) desde $a$ hasta $t$. (Se utiliza $u$ como variable muda de integración para evitar confusión con el límite superior $t$).

$$s(t) = \int_{a}^{t} \|\mathbf{r}'(u)\| du$$

**2. Diferenciación de $s(t)$**

El objetivo es encontrar la derivada de $s(t)$ con respecto a $t$:
$$\frac{ds}{dt} = \frac{d}{dt} \left[ s(t) \right]$$

Sustituimos la definición integral del Paso 1:
$$\frac{ds}{dt} = \frac{d}{dt} \left[ \int_{a}^{t} \|\mathbf{r}'(u)\| du \right]$$

**3. Aplicación del Teorema Fundamental del Cálculo (TFC)**

Invocamos la Parte 1 del TFC, que establece que si $F(t) = \int_{a}^{t} f(u) du$ y $f$ es una función continua, entonces $F'(t) = f(t)$.

Para aplicar el TFC a nuestra ecuación, debemos identificar $f(u)$ y verificar su continuidad:
* Sea $f(u) = \|\mathbf{r}'(u)\|$.

Por la condición inicial del problema, $\mathbf{r}'(t)$ es una función vectorial continua. La norma de una función vectorial continua (ej. $f(u) = \sqrt{[x'(u)]^2 + [y'(u)]^2 + [z'(u)]^2}$) es una composición de funciones continuas (suma, cuadrado, raíz cuadrada) y, por lo tanto, también es una función escalar continua.

Dado que $f(u) = \|\mathbf{r}'(u)\|$ es continua, el TFC es aplicable.

**4. Conclusión**

Al aplicar el TFC a la expresión del Paso 2, la derivada $\frac{d}{dt}$ "cancela" la integral $\int_{a}^{t} ... du$, y la variable muda $u$ es reemplazada por $t$:
$$\frac{ds}{dt} = \|\mathbf{r}'(t)\|$$

---

### Resultado final

La demostración está completa. Se ha demostrado que:
$$\frac{ds}{dt} = \|\mathbf{r}'(t)\|$$
*Q.E.D. (Lo Que Queda Demostrado).*

---

### Interpretación breve del resultado

Esta identidad es fundamental en cinemática y cálculo vectorial. Tiene una interpretación física directa:
* $\mathbf{r}'(t)$ es el vector **velocidad** $\mathbf{v}(t)$.
* $\|\mathbf{r}'(t)\|$ es la magnitud de la velocidad, conocida como **rapidez** $\nu(t)$.
* $s(t)$ es la **distancia** total recorrida a lo largo de la trayectoria.
* $\frac{ds}{dt}$ es la **tasa de cambio** (derivada) de la distancia recorrida.

La ecuación $\frac{ds}{dt} = \|\mathbf{r}'(t)\|$ se traduce como: "La tasa a la que se recorre la distancia es igual a la rapidez instantánea", lo cual es la definición misma de rapidez.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 20

### Enunciado del problema

Evaluar la veracidad de la siguiente proposición:

"Sea $\mathbf{r}(t)$ una curva con derivada continua definida en el intervalo $[a, b]$. Si la magnitud de su derivada (rapidez) es constante, $\|\mathbf{r}'(t)\| = k$, para todo $t \in [a, b]$, entonces el vector de posición $\mathbf{r}(t)$ y el vector velocidad $\mathbf{r}'(t)$ son perpendiculares para toda $t \in [a, b]$."

---

### Datos dados

* **Curva:** $\mathbf{r}(t)$ (Vector de posición).
* **Velocidad:** $\mathbf{r}'(t)$.
* **Hipótesis:** La rapidez es constante, $\|\mathbf{r}'(t)\| = k$.
* **Tesis a evaluar:** Los vectores $\mathbf{r}(t)$ y $\mathbf{r}'(t)$ son perpendiculares.
* **Condición de perpendicularidad:** La tesis es verdadera si y solo si $\mathbf{r}(t) \cdot \mathbf{r}'(t) = 0$ para todo $t \in [a, b]$.

---

### Desarrollo paso a paso

La proposición es **FALSA**.

Se refutará mediante un contraejemplo que satisface la hipótesis (rapidez constante) pero no cumple la tesis (perpendicularidad).

**1. Proposición del Contraejemplo**

Considere la curva $\mathbf{r}(t)$ que describe una línea recta simple que no pasa por el origen. Por ejemplo, en el intervalo $t \in [1, 2]$:
$$\mathbf{r}(t) = (t, 1, 0)$$

**2. Verificación de la Hipótesis ($\|\mathbf{r}'(t)\| = k$)**

Calculamos el vector velocidad (la derivada):
$$\mathbf{r}'(t) = \frac{d}{dt} (t, 1, 0) = (1, 0, 0)$$

Calculamos su magnitud (la rapidez):
$$\|\mathbf{r}'(t)\| = \sqrt{(1)^2 + (0)^2 + (0)^2} = \sqrt{1} = 1$$

La rapidez es $k=1$, que es un valor constante. Por lo tanto, **la hipótesis se cumple**.

**3. Verificación de la Tesis ($\mathbf{r}(t) \cdot \mathbf{r}'(t) = 0$)**

Calculamos el producto escalar entre el vector de posición y el vector velocidad:
$$\mathbf{r}(t) \cdot \mathbf{r}'(t) = (t, 1, 0) \cdot (1, 0, 0)$$

$$\mathbf{r}(t) \cdot \mathbf{r}'(t) = (t \times 1) + (1 \times 0) + (0 \times 0)$$

$$\mathbf{r}(t) \cdot \mathbf{r}'(t) = t$$

El resultado del producto escalar es $t$. Para que la tesis fuera verdadera, el resultado debería ser $0$ para todo $t$. Sin embargo, en el intervalo $t \in [1, 2]$, $t$ nunca es $0$.

Por lo tanto, **la tesis no se cumple**.

---

### Resultado final

Se ha encontrado un contraejemplo $\mathbf{r}(t) = (t, 1, 0)$ que tiene rapidez constante ($\|\mathbf{r}'(t)\| = 1$), pero cuyo vector de posición no es perpendicular al vector velocidad ($\mathbf{r}(t) \cdot \mathbf{r}'(t) = t \neq 0$).

La proposición enunciada es **FALSA**.

---

### Interpretación breve del resultado

La proposición es falsa porque la condición de *rapidez constante* ($\|\mathbf{r}'(t)\| = k$) no impone ninguna restricción sobre la perpendicularidad entre la posición y la velocidad.

Es muy probable que la proposición contenga un error tipográfico y esté confundiendo dos teoremas diferentes. La proposición que sí es verdadera es la siguiente:

**Teorema Verdadero:** Si la **magnitud del vector de posición** es constante (es decir, $\|\mathbf{r}(t)\| = k$, lo que significa que la curva se mueve sobre la superficie de una esfera centrada en el origen), entonces $\mathbf{r}(t)$ y $\mathbf{r}'(t)$ son perpendiculares.

**Prueba del Teorema Verdadero:**
Si $\|\mathbf{r}(t)\| = k$, entonces $\|\mathbf{r}(t)\|^2 = k^2$.
Esto es $\mathbf{r}(t) \cdot \mathbf{r}(t) = k^2$.
Derivamos ambos lados respecto a $t$:
$$\frac{d}{dt}[\mathbf{r}(t) \cdot \mathbf{r}(t)] = \frac{d}{dt}[k^2]$$

$$\mathbf{r}'(t) \cdot \mathbf{r}(t) + \mathbf{r}(t) \cdot \mathbf{r}'(t) = 0$$

$$2 (\mathbf{r}(t) \cdot \mathbf{r}'(t)) = 0$$

$$\mathbf{r}(t) \cdot \mathbf{r}'(t) = 0$$
Esto demuestra que $\mathbf{r}(t)$ y $\mathbf{r}'(t)$ son perpendiculares si la magnitud de la *posición* es constante, no si la magnitud de la *velocidad* es constante.

---

✅ *Cálculos verificados: correctos.*

---
# Problema 21 inciso 1

### Enunciado del problema

Reparametrice la curva $\mathbf{r}(t) = (a \cos t, a \sin t)$ por longitud de arco. Considere el punto inicial en $t_0 = 0$.

---

### Datos dados

La curva a reparametrizar es (asumiendo $a > 0$):
$$\mathbf{r}(t) = (a \cos t, a \sin t)$$

El punto inicial para medir la longitud de arco es $t_0 = 0$.

---

### Desarrollo paso a paso

El objetivo es encontrar la función $\mathbf{r}(s)$, donde $s$ es el parámetro de longitud de arco.

#### 1. Calcular el vector velocidad $\mathbf{r}'(t)$

Se deriva la función de posición $\mathbf{r}(t)$ respecto a $t$:
$$\mathbf{r}'(t) = \frac{d}{dt} (a \cos t, a \sin t)$$

$$\mathbf{r}'(t) = (-a \sin t, a \cos t)$$

#### 2. Calcular la rapidez $\|\mathbf{r}'(t)\|$

Se calcula la magnitud (norma) del vector velocidad. Esta magnitud es la rapidez.
$$\|\mathbf{r}'(t)\| = \sqrt{(-a \sin t)^2 + (a \cos t)^2}$$

$$\|\mathbf{r}'(t)\| = \sqrt{a^2 \sin^2 t + a^2 \cos^2 t}$$

$$\|\mathbf{r}'(t)\| = \sqrt{a^2 (\sin^2 t + \cos^2 t)} = \sqrt{a^2 (1)}$$

$$\|\mathbf{r}'(t)\| = |a|$$

Dado que $a$ es el radio, asumimos $a > 0$, por lo que la rapidez es constante:
$$\|\mathbf{r}'(t)\| = a$$

#### 3. Calcular la función de longitud de arco $s(t)$

La función de longitud de arco $s$ se define como la integral de la rapidez desde el punto inicial $t_0 = 0$ hasta $t$:
$$s(t) = \int_{0}^{t} \|\mathbf{r}'(u)\| du$$

$$s(t) = \int_{0}^{t} a \, du$$

$$s(t) = a \left[ u \right]_{0}^{t} = a(t - 0)$$

$$s = at$$

#### 4. Resolver $t$ en función de $s$

Se despeja el parámetro original $t$ de la ecuación de longitud de arco:
$$t = \frac{s}{a}$$

#### 5. Sustituir $t(s)$ en $\mathbf{r}(t)$

Finalmente, se sustituye la expresión de $t(s)$ en la ecuación original de la curva $\mathbf{r}(t)$ para obtener la reparametrización $\mathbf{r}(s)$:
$$\mathbf{r}(s) = \left(a \cos\left(\frac{s}{a}\right), a \sin\left(\frac{s}{a}\right)\right)$$

---

### Resultado final

La curva reparametrizada por longitud de arco, con punto inicial en $t_0=0$, es:
$$\mathbf{r}(s) = \left(a \cos\left(\frac{s}{a}\right), a \sin\left(\frac{s}{a}\right)\right)$$

---

### Interpretación breve del resultado

La nueva función $\mathbf{r}(s)$ describe la misma curva (un círculo de radio $a$). Sin embargo, ahora está parametrizada de tal manera que la derivada respecto a $s$, $\mathbf{r}'(s)$, tiene una magnitud (rapidez) constante de $1$. Esto significa que un cambio de $1$ unidad en el parámetro $s$ corresponde exactamente a $1$ unidad de distancia recorrida a lo largo de la curva.

*(Validación: $\mathbf{r}'(s) = (-\sin(s/a), \cos(s/a))$, y $\|\mathbf{r}'(s)\| = \sqrt{\sin^2(s/a) + \cos^2(s/a)} = 1$).*

---

✅ *Cálculos verificados: correctos.*

# Problema 21 inciso 2

### Enunciado del problema

Reparametrice la curva $\mathbf{r}(t) = (a \cos t, a \sin t, bt)$ por longitud de arco, iniciando en $t_0 = 0$.

---

### Datos dados

La curva a reparametrizar (una hélice circular) es:
$$\mathbf{r}(t) = (a \cos t, a \sin t, bt)$$

El punto inicial para medir la longitud de arco es $t_0 = 0$. Se asume que $a$ y $b$ son constantes no nulas.

---

### Desarrollo paso a paso

Para reparametrizar por longitud de arco $s$, seguimos un proceso de cuatro pasos.

#### 1. Cálculo de la Velocidad y la Rapidez

Primero, se calcula el vector velocidad $\mathbf{r}'(t)$:
$$\mathbf{r}'(t) = \frac{d}{dt} (a \cos t, a \sin t, bt)$$

$$\mathbf{r}'(t) = (-a \sin t, a \cos t, b)$$

A continuación, se calcula la magnitud (rapidez) $\|\mathbf{r}'(t)\|$:
$$\|\mathbf{r}'(t)\| = \sqrt{[x'(t)]^2 + [y'(t)]^2 + [z'(t)]^2}$$

$$\|\mathbf{r}'(t)\| = \sqrt{(-a \sin t)^2 + (a \cos t)^2 + (b)^2}$$

$$\|\mathbf{r}'(t)\| = \sqrt{a^2 \sin^2 t + a^2 \cos^2 t + b^2}$$

Usando la identidad $\sin^2 t + \cos^2 t = 1$:
$$\|\mathbf{r}'(t)\| = \sqrt{a^2(1) + b^2} = \sqrt{a^2 + b^2}$$

La rapidez de la hélice es constante.

#### 2. Cálculo de la Función Longitud de Arco $s(t)$

La función $s(t)$ mide la longitud de la curva desde el punto inicial $t_0 = 0$ hasta un tiempo $t$. Se define como la integral de la rapidez:
$$s(t) = \int_{0}^{t} \|\mathbf{r}'(u)\| du$$

Sustituimos la rapidez constante que encontramos:
$$s(t) = \int_{0}^{t} \sqrt{a^2 + b^2} \, du$$

$$s(t) = \left( \sqrt{a^2 + b^2} \right) \left[ u \right]_{0}^{t}$$

$$s = t \sqrt{a^2 + b^2}$$

#### 3. Resolución de $t$ en función de $s$

Se despeja el parámetro original $t$ de la ecuación de longitud de arco:
$$t = \frac{s}{\sqrt{a^2 + b^2}}$$

#### 4. Sustitución para $\mathbf{r}(s)$

Finalmente, se sustituye esta expresión de $t(s)$ en la ecuación original de la curva $\mathbf{r}(t)$:
$$\mathbf{r}(s) = \left( a \cos\left(t(s)\right), a \sin\left(t(s)\right), b \cdot t(s) \right)$$

$$\mathbf{r}(s) = \left( a \cos\left(\frac{s}{\sqrt{a^2 + b^2}}\right), a \sin\left(\frac{s}{\sqrt{a^2 + b^2}}\right), b\left(\frac{s}{\sqrt{a^2 + b^2}}\right) \right)$$

---

### Resultado final

La curva reparametrizada por longitud de arco es:
$$\mathbf{r}(s) = \left( a \cos\left(\frac{s}{\sqrt{a^2 + b^2}}\right), a \sin\left(\frac{s}{\sqrt{a^2 + b^2}}\right), \frac{bs}{\sqrt{a^2 + b^2}} \right)$$

---

### Interpretación breve del resultado

La nueva función $\mathbf{r}(s)$ describe la misma trayectoria de hélice circular. La ventaja de esta parametrización es que la rapidez respecto al parámetro $s$ es $1$ (rapidez unitaria). Esto significa que $s$ representa la distancia real recorrida a lo largo de la hélice desde el punto inicial $(a, 0, 0)$.

---

✅ *Cálculos verificados: correctos.*

---
