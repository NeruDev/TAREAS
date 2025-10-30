# Problema 1 inciso 1

### Enunciado del problema

Determinar el dominio de la función vectorial $\mathbf{f}(t) = (\sqrt{9 - t^2}, \ln(t - 3), \frac{2t - 3}{4})$.

* * *

### Datos dados

La función vectorial es $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$, donde las funciones componentes son:

- $f_1(t) = \sqrt{9 - t^2}$
- $f_2(t) = \ln(t - 3)$
- $f_3(t) = \frac{2t - 3}{4}$

* * *

### Desarrollo paso a paso

El dominio de una función vectorial $\mathbf{f}(t)$ es la **intersección** de los dominios de sus funciones componentes. Calculamos el dominio para cada componente por separado.

$$
D_f = D_1 \cap D_2 \cap D_3
$$

**1\. Dominio de $f_1(t)$**

La componente $f_1(t) = \sqrt{9 - t^2}$ es una raíz cuadrada. Para que esté definida en los números reales ($\mathbb{R}$), el radicando (la expresión dentro de la raíz) debe ser mayor o igual a cero.

$$
9 - t^2 \ge 0
$$

Resolvemos la inecuación:

$$
9 \ge t^2
$$

$$
|t| \le \sqrt{9}
$$

$$
|t| \le 3
$$

Esta desigualdad es equivalente al intervalo cerrado:

$$
D_1 = [-3, 3]
$$

**2\. Dominio de $f_2(t)$**

La componente $f_2(t) = \ln(t - 3)$ es un logaritmo natural. Para que esté definido, su argumento (la expresión dentro del paréntesis) debe ser estrictamente positivo.

$$
t - 3 > 0
$$

Resolvemos la inecuación:

$$
t > 3
$$

El dominio es el intervalo abierto:

$$
D_2 = (3, \infty)
$$

**3\. Dominio de $f_3(t)$**

La componente $f_3(t) = \frac{2t - 3}{4}$ es una función polinómica (lineal) dividida por una constante. El denominador es $4$, que es distinto de cero. No existe ninguna restricción para $t$.

$$
D_3 = (-\infty, \infty) \text{ o } \mathbb{R}
$$

**4\. Intersección de Dominios**

El dominio final $D_f$ es la intersección de los tres dominios calculados:

$$
D_f = D_1 \cap D_2 \cap D_3
$$

Sustituimos los conjuntos:

$$
D_f = [-3, 3] \cap (3, \infty) \cap \mathbb{R}
$$

La intersección con $\mathbb{R}$ no altera el resultado, por lo que nos centramos en:

$$
D_f = [-3, 3] \cap (3, \infty)
$$

Buscamos los números $t$ que cumplan ambas condiciones simultáneamente:

- Condición 1 (de $D_1$): $-3 \le t \le 3$ ( $t$ debe ser menor o igual a 3)
- Condición 2 (de $D_2$): $t > 3$ ( $t$ debe ser estrictamente mayor que 3)

No existe ningún número real $t$ que pueda ser al mismo tiempo menor o igual a 3 y estrictamente mayor que 3.

* * *

### Resultado final

La intersección de los dominios es el conjunto vacío.

$$
D_f = \emptyset
$$

* * *

### Interpretación breve del resultado

El dominio de la función vectorial $\mathbf{f}(t)$ es el **conjunto vacío** ($\emptyset$), lo que significa que no existe ningún valor real $t$ para el cual las tres funciones componentes estén definidas simultáneamente.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 1 inciso 5

### Enunciado del problema

Determinar el dominio de la función vectorial $\mathbf{v}(t) = (e^{-t}, \frac{1}{t}, \frac{t}{t^2 + 1})$.

* * *

### Datos dados

La función vectorial es $\mathbf{v}(t) = (v_1(t), v_2(t), v_3(t))$, donde las funciones componentes son:

- $v_1(t) = e^{-t}$
- $v_2(t) = \frac{1}{t}$
- $v_3(t) = \frac{t}{t^2 + 1}$

* * *

### Desarrollo paso a paso

El dominio de una función vectorial $\mathbf{v}(t)$ es la **intersección** de los dominios de sus funciones componentes. Calculamos el dominio para cada componente por separado.

$$
D_v = D_1 \cap D_2 \cap D_3
$$

**1\. Dominio de $v_1(t)$**

La componente $v_1(t) = e^{-t}$ es una función exponencial. La función exponencial está definida para cualquier exponente real. Por lo tanto, no hay restricciones para $t$.

$$
D_1 = \mathbb{R} \quad \text{o} \quad (-\infty, \infty)
$$

**2\. Dominio de $v_2(t)$**

La componente $v_2(t) = \frac{1}{t}$ es una función racional. El dominio requiere que el denominador sea distinto de cero.

$$
t \ne 0
$$

El dominio es el conjunto de todos los números reales excepto el cero:

$$
D_2 = \mathbb{R} - \{0\} \quad \text{o} \quad (-\infty, 0) \cup (0, \infty)
$$

**3\. Dominio de $v_3(t)$**

La componente $v_3(t) = \frac{t}{t^2 + 1}$ es una función racional. Buscamos valores de $t$ que anulen el denominador:

$$
t^2 + 1 = 0
$$

$$
t^2 = -1
$$

Esta ecuación no tiene solución en el conjunto de los números reales ($\mathbb{R}$), ya que $t^2$ es siempre mayor o igual a cero ($t^2 \ge 0$), lo que implica que $t^2 + 1$ es siempre mayor o igual a uno ($t^2 + 1 \ge 1$). El denominador nunca es cero.

$$
D_3 = \mathbb{R} \quad \text{o} \quad (-\infty, \infty)
$$

**4\. Intersección de Dominios**

El dominio final $D_v$ es la intersección de los tres dominios calculados:

$$
D_v = D_1 \cap D_2 \cap D_3
$$

Sustituimos los conjuntos:

$$
D_v = \mathbb{R} \cap (\mathbb{R} - \{0\}) \cap \mathbb{R}
$$

La intersección de estos tres conjuntos es el conjunto más restrictivo, $D_2$.

$$
D_v = \mathbb{R} - \{0\}
$$

* * *

### Resultado final

El dominio de la función vectorial $\mathbf{v}(t)$ es el conjunto de todos los números reales excepto $t=0$.

$$
D_v = \mathbb{R} - \{0\}
$$

Expresado en notación de intervalos:

$$
D_v = (-\infty, 0) \cup (0, \infty)
$$

* * *

### Interpretación breve del resultado

El dominio de la función $\mathbf{v}(t)$ son todos los números reales $t$ excepto $t=0$. En $t=0$, la segunda componente de la función, $\frac{1}{t}$, no está definida.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 2 inciso 1

### Enunciado del problema

Dibuje la curva en el espacio generada por la función vectorial:

$$
\mathbf{f}(t) = (1 + t, 3 + t, 2 + 2t)
$$

* * *

### Datos dados

La función vectorial $\mathbf{f}(t)$ define las siguientes ecuaciones paramétricas en $\mathbb{R}^3$, asumiendo $t \in \mathbb{R}$:

- $x(t) = 1 + t$
- $y(t) = 3 + t$
- $z(t) = 2 + 2t$

* * *

### Desarrollo paso a paso

1.  **Identificación de la forma canónica**  
    Observamos que las tres ecuaciones paramétricas ($x, y, z$) son funciones lineales del parámetro $t$. Esto indica que la curva es una **línea recta**.
    
    Podemos reescribir la función vectorial $\mathbf{f}(t)$ para separar los términos constantes (el punto) de los términos dependientes de $t$ (el vector director).
    
    $$
    \mathbf{f}(t) = (1, 3, 2) + (t, t, 2t)
    $$
    
    Factorizando $t$, obtenemos la ecuación vectorial canónica de la recta, $\mathbf{r}(t) = \mathbf{r}_0 + t\mathbf{v}$:
    
    $$
    \mathbf{f}(t) = (1, 3, 2) + t(1, 1, 2)
    $$
    
2.  **Identificación de elementos**  
    De la ecuación canónica, identificamos los elementos geométricos de la recta:
    
    - Un punto de paso $\mathbf{r}_0$ (evaluando $t=0$): $P_0 = (1, 3, 2)$.
    - El vector director $\mathbf{v}$: $\mathbf{v} = (1, 1, 2)$.
3.  **Obtención de puntos para el trazado**  
    Para dibujar la recta, necesitamos al menos dos puntos distintos.
    
    - **Punto $P_0$ (para $t=0$):**
        
        $$
        P_0 = (1, 3, 2)
        $$
        
    - **Punto $P_1$ (evaluando en $t=1$):**
        
        $$
        P_1 = (1+1, 3+1, 2+2(1)) = (2, 4, 4)
        $$
        
4.  **Validación (Ecuaciones Simétricas)**  
    Si despejamos $t$ de las ecuaciones paramétricas:
    
    - $t = x - 1$
    - $t = y - 3$
    - $t = \frac{z - 2}{2}$
    
    Al igualar los parámetros, obtenemos las ecuaciones simétricas de la recta, lo que confirma que es una recta que pasa por $(1, 3, 2)$ con vector director $(1, 1, 2)$:
    
    $$
    x - 1 = y - 3 = \frac{z - 2}{2}
    $$
    

* * *

### Resultado final

La curva generada por $\mathbf{f}(t)$ es una **línea recta** en $\mathbb{R}^3$.

Para dibujarla, se traza la línea infinita que pasa por los puntos:

- $P_0 = (1, 3, 2)$
- $P_1 = (2, 4, 4)$

Esta recta tiene como vector director $\mathbf{v} = (1, 1, 2)$.

* * *

### Interpretación breve del resultado

La función $\mathbf{f}(t)$ parametriza una línea recta en el espacio tridimensional. A medida que $t$ (el parámetro) varía, la función describe todos los puntos sobre esta recta.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 2 inciso 3

### Enunciado del problema

Dibuje la curva en el espacio generada por la función vectorial:

$$
\mathbf{h}(t) = (2\cos t, 2\sin t, \frac{t}{2})
$$

* * *

### Datos dados

La función vectorial $\mathbf{h}(t)$ define las siguientes ecuaciones paramétricas en $\mathbb{R}^3$, asumiendo $t \in \mathbb{R}$:

- $x(t) = 2\cos t$
- $y(t) = 2\sin t$
- $z(t) = \frac{t}{2}$

* * *

### Desarrollo paso a paso

1.  **Análisis de la Proyección en el Plano $xy$**  
    Analizamos la relación entre las componentes $x(t)$ e $y(t)$ para encontrar la forma de la proyección de la curva en el plano $xy$.
    
    $$
    x = 2\cos t
    $$
    
    $$
    y = 2\sin t
    $$
    
    Elevamos al cuadrado ambas ecuaciones y las sumamos:
    
    $$
    x^2 = (2\cos t)^2 = 4\cos^2 t
    $$
    
    $$
    y^2 = (2\sin t)^2 = 4\sin^2 t
    $$
    
    $$
    x^2 + y^2 = 4\cos^2 t + 4\sin^2 t
    $$
    
    Factorizamos el 4 y aplicamos la identidad trigonométrica fundamental $(\cos^2 t + \sin^2 t = 1)$:
    
    $$
    x^2 + y^2 = 4(\cos^2 t + \sin^2 t)
    $$
    
    $$
    x^2 + y^2 = 4(1)
    $$
    
    $$
    x^2 + y^2 = 4
    $$
    
    Esta es la ecuación de un **círculo** centrado en el origen $(0,0)$ con radio $r = \sqrt{4} = 2$. Esto significa que la curva, vista desde arriba, se proyecta sobre este círculo.
    
2.  **Análisis de la Componente $z$**  
    La componente $z$ (altura) está dada por:
    
    $$
    z(t) = \frac{t}{2}
    $$
    
    La altura $z$ es directamente proporcional al parámetro $t$. A medida que $t$ aumenta, la altura $z$ aumenta linealmente.
    
3.  **Identificación de la Curva (Hélice)**  
    Al combinar ambos análisis:
    
    - La curva se enrolla sobre la superficie de un cilindro circular de radio 2, centrado en el eje $z$ (dado por $x^2 + y^2 = 4$).
    - Mientras se enrolla, la curva asciende (o desciende) a un ritmo constante (dado por $z(t) = \frac{t}{2}$).
    
    Esta forma geométrica es una **hélice circular**.
    
4.  **Características para el Trazado (Paso de la Hélice)**  
    El "paso" (pitch) de la hélice es la distancia vertical que recorre en una revolución completa (es decir, cuando $t$ varía en $2\pi$).
    
    - Altura inicial (en $t=0$):  
        $z_{\text{inicio}} = z(0) = \frac{0}{2} = 0$
    - Altura final (en $t=2\pi$):  
        $z_{\text{fin}} = z(2\pi) = \frac{2\pi}{2} = \pi$
    
    El paso de la hélice es $z_{\text{fin}} - z_{\text{inicio}} = \pi - 0 = \pi$.
    
5.  **Puntos Clave para el Dibujo**  
    Calculamos algunos puntos para esbozar la curva:
    
    - $t=0$: $\mathbf{h}(0) = (2\cos 0, 2\sin 0, 0) = (2, 0, 0)$
    - $t=\pi/2$ (cuarto de vuelta): $\mathbf{h}(\pi/2) = (2\cos \frac{\pi}{2}, 2\sin \frac{\pi}{2}, \frac{\pi/2}{2}) = (0, 2, \frac{\pi}{4})$
    - $t=\pi$ (media vuelta): $\mathbf{h}(\pi) = (2\cos \pi, 2\sin \pi, \frac{\pi}{2}) = (-2, 0, \frac{\pi}{2})$
    - $t=2\pi$ (vuelta completa): $\mathbf{h}(2\pi) = (2\cos 2\pi, 2\sin 2\pi, \frac{2\pi}{2}) = (2, 0, \pi)$

* * *

### Resultado final

La curva generada por $\mathbf{h}(t)$ es una **hélice circular** que se enrolla alrededor del eje $z$.

- **Radio:** $r = 2$ (la curva yace sobre el cilindro $x^2 + y^2 = 4$).
- **Sentido:** Antihorario (visto desde el eje $z$ positivo).
- **Paso (Pitch):** $\pi$. Por cada vuelta completa ($2\pi$ en $t$), la hélice asciende $\pi$ unidades en $z$.

* * *

### Interpretación breve del resultado

Para dibujar la curva, trace un cilindro de radio 2 centrado en el eje $z$. La curva comienza en el punto $(2, 0, 0)$ (sobre el eje $x$) y se enrolla hacia arriba alrededor del cilindro. Después de una revolución completa, llega al punto $(2, 0, \pi)$, exactamente $\pi$ unidades por encima de donde empezó.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 3 inciso 2

### Enunciado del problema

Determine una función vectorial $\mathbf{r}(t)$ que recorra la curva de intersección de las superficies $z = x^2 + y^2$ y $z = 4$, usando el parámetro dado $x = 2\cos t$.

* * *

### Datos dados

- Superficie 1 (Paraboloide): $S_1: z = x^2 + y^2$
- Superficie 2 (Plano): $S_2: z = 4$
- Parametrización dada: $x(t) = 2\cos t$

* * *

### Desarrollo paso a paso

El objetivo es encontrar la función vectorial $\mathbf{r}(t) = (x(t), y(t), z(t))$ que describe la curva de intersección.

**1\. Determinar $x(t)$ y $z(t)$**

Las componentes $x(t)$ y $z(t)$ se obtienen directamente de los datos del problema:

- La curva debe estar en el plano $z = 4$, por lo tanto, la componente $z$ es constante:
    
    $$
    z(t) = 4
    $$
    
- El problema especifica la parametrización para $x$:
    
    $$
    x(t) = 2\cos t
    $$
    

**2\. Determinar $y(t)$**

Para encontrar $y(t)$, sustituimos las componentes $x(t)$ y $z(t)$ conocidas en la ecuación de la otra superficie (el paraboloide $z = x^2 + y^2$):

$$
z(t) = x(t)^2 + y(t)^2
$$

$$
4 = (2\cos t)^2 + y(t)^2
$$

A continuación, despejamos $y(t)$:

$$
4 = 4\cos^2 t + y(t)^2
$$

$$
y(t)^2 = 4 - 4\cos^2 t
$$

Factorizamos el 4:

$$
y(t)^2 = 4(1 - \cos^2 t)
$$

Usamos la identidad trigonométrica fundamental $\sin^2 t + \cos^2 t = 1$, de la cual se deduce que $1 - \cos^2 t = \sin^2 t$:

$$
y(t)^2 = 4\sin^2 t
$$

Tomamos la raíz cuadrada en ambos lados. Para obtener la parametrización estándar (sentido antihorario visto desde $+z$), seleccionamos la raíz positiva:

$$
y(t) = \sqrt{4\sin^2 t} = 2\sin t
$$

**3\. Ensamblar la Función Vectorial**

Reunimos las tres componentes $x(t)$, $y(t)$ y $z(t)$:

$$
\mathbf{r}(t) = (x(t), y(t), z(t))
$$

$$
\mathbf{r}(t) = (2\cos t, 2\sin t, 4)
$$

* * *

### Resultado final

La función vectorial que recorre la curva de intersección es:

$$
\mathbf{r}(t) = (2\cos t, 2\sin t, 4)
$$

* * *

### Interpretación breve del resultado

La intersección del paraboloide $z = x^2 + y^2$ con el plano horizontal $z = 4$ ocurre cuando $4 = x^2 + y^2$. Esta ecuación describe un **círculo** en el plano $z=4$, centrado en el eje $z$ (origen $x,y$ de $(0,0)$) y con un radio $r = \sqrt{4} = 2$.

La función vectorial $\mathbf{r}(t)$ obtenida parametriza correctamente este círculo de radio 2, que se encuentra a una altura constante $z=4$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 3 inciso 5

### Enunciado del problema

Determine una función vectorial $\mathbf{r}(t)$ que recorra la curva intersección de las superficies $x^2 + y^2 + z^2 = 4$ y $x + z = 2$, use el parámetro dado $x = 1 + \sin t$.

* * *

### Datos dados

- Superficie 1 (Esfera): $S_1: x^2 + y^2 + z^2 = 4$
- Superficie 2 (Plano): $S_2: x + z = 2$
- Parametrización dada: $x(t) = 1 + \sin t$

* * *

### Desarrollo paso a paso

Se busca la función vectorial $\mathbf{r}(t) = (x(t), y(t), z(t))$ que satisface las tres ecuaciones dadas.

**1\. Componente $x(t)$**

La componente $x(t)$ es dada por el enunciado del problema:

$$
x(t) = 1 + \sin t
$$

**2\. Componente $z(t)$**

Se despeja $z(t)$ de la ecuación del plano ($S_2: x + z = 2$):

$$
z(t) = 2 - x(t)
$$

Sustituimos la expresión conocida para $x(t)$:

$$
z(t) = 2 - (1 + \sin t)
$$

$$
z(t) = 2 - 1 - \sin t
$$

$$
z(t) = 1 - \sin t
$$

*(Verificación: $x(t) + z(t) = (1 + \sin t) + (1 - \sin t) = 2$. La ecuación del plano se cumple.)*

**3\. Componente $y(t)$**

Se despeja $y(t)$ de la ecuación de la esfera ($S_1: x^2 + y^2 + z^2 = 4$):

$$
y(t)^2 = 4 - x(t)^2 - z(t)^2
$$

Sustituimos las expresiones encontradas para $x(t)$ y $z(t)$:

$$
y(t)^2 = 4 - (1 + \sin t)^2 - (1 - \sin t)^2
$$

Expandimos los binomios al cuadrado:

$$
y(t)^2 = 4 - (1 + 2\sin t + \sin^2 t) - (1 - 2\sin t + \sin^2 t)
$$

Distribuimos los signos negativos y agrupamos términos semejantes:

$$
y(t)^2 = 4 - 1 - 2\sin t - \sin^2 t - 1 + 2\sin t - \sin^2 t
$$

$$
y(t)^2 = (4 - 1 - 1) + (-2\sin t + 2\sin t) + (-\sin^2 t - \sin^2 t)
$$

$$
y(t)^2 = 2 + 0 - 2\sin^2 t
$$

$$
y(t)^2 = 2 - 2\sin^2 t
$$

Factorizamos el 2:

$$
y(t)^2 = 2(1 - \sin^2 t)
$$

Usamos la identidad trigonométrica fundamental $(\sin^2 t + \cos^2 t = 1)$, de la cual $1 - \sin^2 t = \cos^2 t$:

$$
y(t)^2 = 2\cos^2 t
$$

Tomamos la raíz cuadrada (seleccionando la raíz positiva por convención estándar):

$$
y(t) = \sqrt{2\cos^2 t}
$$

$$
y(t) = \sqrt{2} \cos t
$$

**4\. Ensamblar la Función Vectorial**

Combinamos las componentes $x(t)$, $y(t)$ y $z(t)$:

$$
\mathbf{r}(t) = (x(t), y(t), z(t))
$$

$$
\mathbf{r}(t) = (1 + \sin t, \sqrt{2} \cos t, 1 - \sin t)
$$

* * *

### Resultado final

La función vectorial que recorre la curva de intersección es:

$$
\mathbf{r}(t) = (1 + \sin t, \sqrt{2} \cos t, 1 - \sin t)
$$

* * *

### Interpretación breve del resultado

La intersección de la esfera ($r=2$) y el plano ($x+z=2$) es un **círculo**. El análisis geométrico confirma que este círculo está centrado en el punto $(1, 0, 1)$ y tiene un radio $R = \sqrt{2}$. La función vectorial $\mathbf{r}(t)$ obtenida describe la trayectoria de este círculo.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 4 inciso 1

### Enunciado del problema

Para las funciones $\mathbf{f}(t)$ y $\mathbf{v}(t)$ (definidas en un problema anterior), realice la operación $\mathbf{f}(t) + \mathbf{v}(t)$ y calcule el dominio de la función resultante.

* * *

### Datos dados

Las funciones vectoriales de referencia son:

- $\mathbf{f}(t) = (\sqrt{9 - t^2}, \ln(t - 3), \frac{2t - 3}{4})$
- $\mathbf{v}(t) = (e^{-t}, \frac{1}{t}, \frac{t}{t^2 + 1})$

* * *

### Desarrollo paso a paso

**1\. Expresión de la Suma**

La suma $\mathbf{f}(t) + \mathbf{v}(t)$ se obtiene sumando las componentes correspondientes:

$$
\mathbf{f}(t) + \mathbf{v}(t) = \left( \sqrt{9 - t^2} + e^{-t}, \ln(t - 3) + \frac{1}{t}, \frac{2t - 3}{4} + \frac{t}{t^2 + 1} \right)
$$

**2\. Cálculo del Dominio de la Suma**

El dominio de una suma de funciones vectoriales, $D_{\text{suma}}$, es la **intersección** de los dominios de las funciones individuales ($D_f$ y $D_v$).

$$
D_{\text{suma}} = D_f \cap D_v
$$

**A. Dominio de $\mathbf{f}(t)$ ($D_f$)**

El dominio $D_f$ es la intersección de los dominios de sus tres componentes:

- $f_1(t) = \sqrt{9 - t^2}$: Requiere $9 - t^2 \ge 0 \implies t^2 \le 9 \implies -3 \le t \le 3$.  
    $D_{f1} = [-3, 3]$.
- $f_2(t) = \ln(t - 3)$: Requiere $t - 3 > 0 \implies t > 3$.  
    $D_{f2} = (3, \infty)$.
- $f_3(t) = \frac{2t - 3}{4}$: Es polinómica, no tiene restricciones.  
    $D_{f3} = \mathbb{R}$.

La intersección $D_f = D_{f1} \cap D_{f2} \cap D_{f3}$ es:

$$
D_f = [-3, 3] \cap (3, \infty) \cap \mathbb{R}
$$

Las condiciones $t \le 3$ (de $D_{f1}$) y $t > 3$ (de $D_{f2}$) son mutuamente excluyentes. No existe ningún $t$ que cumpla ambas.

$$
D_f = \emptyset
$$

**B. Dominio de $\mathbf{v}(t)$ ($D_v$)**

El dominio $D_v$ es la intersección de los dominios de sus tres componentes:

- $v_1(t) = e^{-t}$: Exponencial, no tiene restricciones.  
    $D_{v1} = \mathbb{R}$.
- $v_2(t) = \frac{1}{t}$: Racional, requiere $t \ne 0$.  
    $D_{v2} = \mathbb{R} - \{0\}$.
- $v_3(t) = \frac{t}{t^2 + 1}$: Racional, $t^2 + 1$ nunca es $0$.  
    $D_{v3} = \mathbb{R}$.

La intersección $D_v = D_{v1} \cap D_{v2} \cap D_{v3}$ es:

$$
D_v = \mathbb{R} \cap (\mathbb{R} - \{0\}) \cap \mathbb{R}
$$

$$
D_v = \mathbb{R} - \{0\}
$$

**C. Dominio final (Intersección)**

Calculamos la intersección de los dominios $D_f$ y $D_v$:

$$
D_{\text{suma}} = D_f \cap D_v = \emptyset \cap (\mathbb{R} - \{0\})
$$

La intersección de cualquier conjunto con el conjunto vacío ($\emptyset$) es el conjunto vacío.

$$
D_{\text{suma}} = \emptyset
$$

* * *

### Resultado final

El dominio de la función vectorial $\mathbf{f}(t) + \mathbf{v}(t)$ es el **conjunto vacío**.

$$
D = \emptyset
$$

* * *

### Interpretación breve del resultado

Para que la suma $\mathbf{f}(t) + \mathbf{v}(t)$ esté definida, ambas funciones $\mathbf{f}(t)$ y $\mathbf{v}(t)$ deben estar definidas para el mismo valor $t$.

Sin embargo, la función $\mathbf{f}(t)$ no está definida para ningún número real (su dominio es $\emptyset$), ya que los requisitos de sus dos primeras componentes ($t \le 3$ y $t > 3$) son contradictorios.

Dado que $\mathbf{f}(t)$ nunca está definida, la suma tampoco puede estar definida.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 4 inciso 4

### Enunciado del problema

Para las funciones vectoriales $\mathbf{r}(t)$ y $\mathbf{v}(t)$, realice la operación $\mathbf{r}(t) \times \mathbf{v}(t)$ y calcule su dominio.

* * *

### Datos dados

Las funciones vectoriales son:

$$
\mathbf{r}(t) = \left(\sqrt{2t + 1}, \frac{1}{e^t - e^{-t}}, \frac{t + 4}{t - 5}\right)
$$

$$
\mathbf{v}(t) = \left(e^{-t}, \frac{1}{t}, \frac{t}{t^2 + 1}\right)
$$

* * *

### Desarrollo paso a paso

El dominio de un producto cruz $\mathbf{r}(t) \times \mathbf{v}(t)$ es la **intersección** de los dominios individuales de $\mathbf{r}(t)$ y $\mathbf{v}(t)$, ya que ambas funciones deben estar definidas para que la operación exista.

$$
D_{\text{cruz}} = D_r \cap D_v
$$

**1\. Expresión del Producto Cruz**

La operación $\mathbf{r}(t) \times \mathbf{v}(t)$ se define formalmente por el determinante:

$$
\mathbf{r}(t) \times \mathbf{v}(t) = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ r_1(t) & r_2(t) & r_3(t) \\ v_1(t) & v_2(t) & v_3(t) \end{vmatrix}
$$

Sustituyendo las funciones dadas:

$$
\mathbf{r}(t) \times \mathbf{v}(t) = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ \sqrt{2t + 1} & \frac{1}{e^t - e^{-t}} & \frac{t + 4}{t - 5} \\ e^{-t} & \frac{1}{t} & \frac{t}{t^2 + 1} \end{vmatrix}
$$

**2\. Cálculo del Dominio de $\mathbf{r}(t)$ ($D_r$)**

Analizamos las restricciones de las tres componentes de $\mathbf{r}(t)$:

- **Componente $r_1(t) = \sqrt{2t + 1}$**:  
    El radicando debe ser no negativo.  
    $2t + 1 \ge 0 \implies 2t \ge -1 \implies t \ge -1/2$.  
    $D_{r1} = [-1/2, \infty)$.
- **Componente $r_2(t) = \frac{1}{e^t - e^{-t}}$**:  
    El denominador debe ser distinto de cero.  
    $e^t - e^{-t} \ne 0 \implies e^t \ne e^{-t} \implies e^t \ne \frac{1}{e^t} \implies e^{2t} \ne 1$.  
    Aplicando logaritmo natural: $2t \ne \ln(1) \implies 2t \ne 0 \implies t \ne 0$.  
    $D_{r2} = \mathbb{R} - \{0\}$.
- **Componente $r_3(t) = \frac{t + 4}{t - 5}$**:  
    El denominador debe ser distinto de cero.  
    $t - 5 \ne 0 \implies t \ne 5$.  
    $D_{r3} = \mathbb{R} - \{5\}$.

El dominio $D_r$ es la intersección $D_{r1} \cap D_{r2} \cap D_{r3}$:  
$D_r = [-1/2, \infty) \cap (\mathbb{R} - \{0\}) \cap (\mathbb{R} - \{5\})$

$$
D_r = [-1/2, 0) \cup (0, 5) \cup (5, \infty)
$$

**3\. Cálculo del Dominio de $\mathbf{v}(t)$ ($D_v$)**

Analizamos las restricciones de las tres componentes de $\mathbf{v}(t)$:

- **Componente $v_1(t) = e^{-t}$**:  
    La función exponencial está definida para todo $t \in \mathbb{R}$. $D_{v1} = \mathbb{R}$.
- **Componente $v_2(t) = \frac{1}{t}$**:  
    El denominador debe ser distinto de cero. $t \ne 0$. $D_{v2} = \mathbb{R} - \{0\}$.
- **Componente $v_3(t) = \frac{t}{t^2 + 1}$**:  
    El denominador $t^2 + 1$ nunca es cero (su valor mínimo es 1). $D_{v3} = \mathbb{R}$.

El dominio $D_v$ es la intersección $D_{v1} \cap D_{v2} \cap D_{v3}$:

$$
D_v = \mathbb{R} \cap (\mathbb{R} - \{0\}) \cap \mathbb{R} = \mathbb{R} - \{0\}
$$

**4\. Intersección de Dominios ($D_{\text{cruz}}$)**

El dominio final es la intersección de $D_r$ y $D_v$:

$$
D_{\text{cruz}} = D_r \cap D_v
$$

$$
D_{\text{cruz}} = \left( [-1/2, 0) \cup (0, 5) \cup (5, \infty) \right) \cap \left( \mathbb{R} - \{0\} \right)
$$

El conjunto $D_r$ ya excluye $t=0$. Por lo tanto, intersecarlo con $D_v$ (que también excluye $t=0$) no añade nuevas restricciones. El dominio resultante es $D_r$.

* * *

### Resultado final

El dominio de la función vectorial $\mathbf{r}(t) \times \mathbf{v}(t)$ es:

$$
D = [-1/2, 0) \cup (0, 5) \cup (5, \infty)
$$

O, equivalentemente:

$$
D = \{ t \in \mathbb{R} \mid t \ge -1/2, t \ne 0, t \ne 5 \}
$$

* * *

### Interpretación breve del resultado

El dominio del producto cruz son todos los valores $t$ para los cuales ambas funciones $\mathbf{r}(t)$ y $\mathbf{v}(t)$ están definidas simultáneamente. El resultado excluye $t < -1/2$ (donde $r_1$ no es real), $t=0$ (donde $r_2$ y $v_2$ son indefinidos) y $t=5$ (donde $r_3$ es indefinido).

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 5 inciso 1

### Enunciado del problema

Determine el límite $\lim_{t \to a} \mathbf{f}(t)$, si es que existe.

1.  $\mathbf{f}(t) = (\sqrt{t}, t^2, \sin t)$, con $a = 2$.

* * *

### Datos dados

- Función vectorial: $\mathbf{f}(t) = (\sqrt{t}, t^2, \sin t)$
- Punto de límite: $a = 2$

* * *

### Desarrollo paso a paso

El límite de una función vectorial $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$ existe si y solo si los límites de todas sus funciones componentes existen. El límite se calcula evaluando el límite de cada componente por separado:

$$
\lim_{t \to a} \mathbf{f}(t) = \left( \lim_{t \to a} f_1(t), \lim_{t \to a} f_2(t), \lim_{t \to a} f_3(t) \right)
$$

Analizamos la continuidad de cada componente en $t=2$:

1.  **Componente $f_1(t) = \sqrt{t}$**: Su dominio es $t \ge 0$. La función es continua en $t=2$.
2.  **Componente $f_2(t) = t^2$**: Su dominio es $\mathbb{R}$. La función es continua en $t=2$.
3.  **Componente $f_3(t) = \sin t$**: Su dominio es $\mathbb{R}$. La función es continua en $t=2$.

Dado que las tres componentes son continuas en $t=2$, el límite existe y se puede calcular por sustitución directa.

- Límite de la primera componente:
    
    $$
    \lim_{t \to 2} \sqrt{t} = \sqrt{2}
    $$
    
- Límite de la segunda componente:
    
    $$
    \lim_{t \to 2} t^2 = (2)^2 = 4
    $$
    
- Límite de la tercera componente:
    
    $$
    \lim_{t \to 2} \sin t = \sin(2)
    $$
    

Se ensambla el vector límite con los resultados de cada componente.

* * *

### Resultado final

El límite de la función vectorial es el vector formado por los límites de las componentes:

$$
\lim_{t \to 2} \mathbf{f}(t) = (\sqrt{2}, 4, \sin 2)
$$

* * *

### Interpretación breve del resultado

El límite existe. Dado que las tres funciones componentes ($f_1, f_2, f_3$) son continuas en $t=2$, el límite de la función vectorial $\mathbf{f}(t)$ cuando $t$ se aproxima a $2$ es simplemente el valor de la función evaluada en ese punto, $\mathbf{f}(2)$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 5 inciso 4

### Enunciado del problema

Determine el límite $\lim_{t \to a} \mathbf{r}(t)$, si es que el límite existe.  
4\. $\mathbf{r}(t) = \left(\frac{1 - \sqrt{t}}{1 - t}, e^{-t}, \frac{2t^2 + 5t - 7}{t^3 - 1}\right)$, con $a = 1$.

* * *

### Datos dados

- Función vectorial: $\mathbf{r}(t) = \left(\frac{1 - \sqrt{t}}{1 - t}, e^{-t}, \frac{2t^2 + 5t - 7}{t^3 - 1}\right)$
- Punto de límite: $a = 1$

* * *

### Desarrollo paso a paso

El límite de una función vectorial $\mathbf{r}(t)$ existe si y solo si los límites de todas sus funciones componentes ($r_1, r_2, r_3$) existen. El límite se calcula evaluando el límite de cada componente por separado.

$$
\mathbf{L} = \lim_{t \to 1} \mathbf{r}(t) = \left( \lim_{t \to 1} r_1(t), \lim_{t \to 1} r_2(t), \lim_{t \to 1} r_3(t) \right)
$$

**1\. Límite de la Componente $r_1(t)$**

$$
L_1 = \lim_{t \to 1} \frac{1 - \sqrt{t}}{1 - t}
$$

Al evaluar $t=1$, se obtiene $\frac{1 - 1}{1 - 1} = \frac{0}{0}$, que es una indeterminación. Se resuelve racionalizando el numerador (multiplicando por su conjugado):

$$
L_1 = \lim_{t \to 1} \left[ \frac{1 - \sqrt{t}}{1 - t} \cdot \frac{1 + \sqrt{t}}{1 + \sqrt{t}} \right]
$$

$$
L_1 = \lim_{t \to 1} \frac{(1)^2 - (\sqrt{t})^2}{(1 - t)(1 + \sqrt{t})}
$$

$$
L_1 = \lim_{t \to 1} \frac{1 - t}{(1 - t)(1 + \sqrt{t})}
$$

Se cancela el factor $(1 - t)$:

$$
L_1 = \lim_{t \to 1} \frac{1}{1 + \sqrt{t}}
$$

Se evalúa por sustitución directa:

$$
L_1 = \frac{1}{1 + \sqrt{1}} = \frac{1}{1 + 1} = \frac{1}{2}
$$

**2\. Límite de la Componente $r_2(t)$**

$$
L_2 = \lim_{t \to 1} e^{-t}
$$

La función $e^{-t}$ es continua en $t=1$. Se calcula por sustitución directa:

$$
L_2 = e^{-1} = \frac{1}{e}
$$

**3\. Límite de la Componente $r_3(t)$**

$$
L_3 = \lim_{t \to 1} \frac{2t^2 + 5t - 7}{t^3 - 1}
$$

Al evaluar $t=1$, se obtiene $\frac{2(1)^2 + 5(1) - 7}{(1)^3 - 1} = \frac{0}{0}$, que es una indeterminación. Se resuelve factorizando el numerador y el denominador. Sabiendo que $t=1$ es raíz, ambos polinomios son divisibles por $(t-1)$.

- Numerador: $2t^2 + 5t - 7 = (t - 1)(2t + 7)$
- Denominador (diferencia de cubos): $t^3 - 1 = (t - 1)(t^2 + t + 1)$

Sustituimos los factores en el límite:

$$
L_3 = \lim_{t \to 1} \frac{(t - 1)(2t + 7)}{(t - 1)(t^2 + t + 1)}
$$

Se cancela el factor $(t - 1)$:

$$
L_3 = \lim_{t \to 1} \frac{2t + 7}{t^2 + t + 1}
$$

Se evalúa por sustitución directa:

$$
L_3 = \frac{2(1) + 7}{(1)^2 + (1) + 1} = \frac{9}{3} = 3
$$

* * *

### Resultado final

El límite de la función vectorial es el vector formado por los límites de las componentes:

$$
\lim_{t \to 1} \mathbf{r}(t) = \left( \frac{1}{2}, \frac{1}{e}, 3 \right)
$$

* * *

### Interpretación breve del resultado

El límite de la función vectorial $\mathbf{r}(t)$ existe, ya que los límites de sus tres funciones componentes existen y son finitos. El vector límite resultante es $(\frac{1}{2}, \frac{1}{e}, 3)$.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 6 inciso 1

### Enunciado del problema

Determine el conjunto donde la función vectorial $\mathbf{f}(t) = (\sqrt{t}, t^2, \sin t)$ es continua.

* * *

### Datos dados

La función vectorial es $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$, donde las funciones componentes son:

- $f_1(t) = \sqrt{t}$
- $f_2(t) = t^2$
- $f_3(t) = \sin t$

* * *

### Desarrollo paso a paso

Una función vectorial $\mathbf{f}(t)$ es continua en un conjunto si, y solo si, todas sus funciones componentes son continuas en ese mismo conjunto.

El conjunto de continuidad $C_f$ es la **intersección** de los conjuntos de continuidad de cada componente ($C_1, C_2, C_3$).

$$
C_f = C_1 \cap C_2 \cap C_3
$$

**1\. Continuidad de $f_1(t)$**

La función $f_1(t) = \sqrt{t}$ (raíz cuadrada) es una función elemental continua en todo su dominio. Para que $\sqrt{t}$ esté definida en los números reales ($\mathbb{R}$), el radicando debe ser no negativo:

$$
t \ge 0
$$

El conjunto de continuidad $C_1$ es:

$$
C_1 = [0, \infty)
$$

**2\. Continuidad de $f_2(t)$**

La función $f_2(t) = t^2$ es una función polinómica. Las funciones polinómicas son continuas en todo el conjunto de los números reales.

$$
C_2 = (-\infty, \infty) \text{ o } \mathbb{R}
$$

**3\. Continuidad de $f_3(t)$**

La función $f_3(t) = \sin t$ es una función trigonométrica. La función seno es continua en todo el conjunto de los números reales.

$$
C_3 = (-\infty, \infty) \text{ o } \mathbb{R}
$$

**4\. Intersección de Conjuntos de Continuidad**

Calculamos la intersección de los tres conjuntos:

$$
C_f = C_1 \cap C_2 \cap C_3
$$

$$
C_f = [0, \infty) \cap \mathbb{R} \cap \mathbb{R}
$$

$$
C_f = [0, \infty)
$$

* * *

### Resultado final

El conjunto donde la función vectorial $\mathbf{f}(t)$ es continua es:

$$
C_f = [0, \infty)
$$

* * *

### Interpretación breve del resultado

La continuidad de la función vectorial $\mathbf{f}(t)$ requiere que sus tres componentes ($\sqrt{t}$, $t^2$ y $\sin t$) sean continuas simultáneamente.

Mientras que $t^2$ y $\sin t$ son continuas para todos los números reales ($\mathbb{R}$), la componente $\sqrt{t}$ solo es continua (y está definida) para $t \ge 0$. Por lo tanto, el conjunto de continuidad de la función vectorial completa está restringido por el dominio de $\sqrt{t}$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 6 inciso 4

### Enunciado del problema

Determine el conjunto donde la función vectorial $\mathbf{r}(t) = \left(\frac{1 - \sqrt{t}}{1 - t}, e^{-t}, \frac{2t^2 + 5t - 7}{t^3 - 1}\right)$ es continua.

* * *

### Datos dados

La función vectorial es $\mathbf{r}(t) = (r_1(t), r_2(t), r_3(t))$, donde las funciones componentes son:

- $r_1(t) = \frac{1 - \sqrt{t}}{1 - t}$
- $r_2(t) = e^{-t}$
- $r_3(t) = \frac{2t^2 + 5t - 7}{t^3 - 1}$

* * *

### Desarrollo paso a paso

Una función vectorial es continua en el conjunto donde todas sus funciones componentes son continuas simultáneamente. Para funciones compuestas de funciones elementales, este conjunto coincide con la **intersección** de sus dominios.

$$
C_r = C_1 \cap C_2 \cap C_3
$$

**1\. Continuidad de $r_1(t)$**

La función $r_1(t) = \frac{1 - \sqrt{t}}{1 - t}$ tiene dos restricciones:

- La función raíz cuadrada $\sqrt{t}$ requiere que el radicando sea no negativo: $t \ge 0$.
- El denominador $1 - t$ debe ser distinto de cero: $t \ne 1$.

El conjunto de continuidad $C_1$ es:

$$
C_1 = [0, 1) \cup (1, \infty)
$$

**2\. Continuidad de $r_2(t)$**

La función $r_2(t) = e^{-t}$ es una función exponencial. Es continua en todo el conjunto de los números reales.

$$
C_2 = \mathbb{R} \quad \text{o} \quad (-\infty, \infty)
$$

**3\. Continuidad de $r_3(t)$**

La función $r_3(t) = \frac{2t^2 + 5t - 7}{t^3 - 1}$ es una función racional. Es continua siempre que el denominador no sea cero:

$$
t^3 - 1 \ne 0 \implies t^3 \ne 1 \implies t \ne 1
$$

El conjunto de continuidad $C_3$ es:

$$
C_3 = \mathbb{R} - \{1\} \quad \text{o} \quad (-\infty, 1) \cup (1, \infty)
$$

**4\. Intersección de Conjuntos de Continuidad**

El conjunto de continuidad de $\mathbf{r}(t)$ es la intersección $C_r = C_1 \cap C_2 \cap C_3$:

$$
C_r = \left( [0, 1) \cup (1, \infty) \right) \cap \left( \mathbb{R} \right) \cap \left( \mathbb{R} - \{1\} \right)
$$

La intersección de $C_1$ (que ya excluye $t=1$ y $t<0$) con $C_2$ (sin restricciones) y $C_3$ (que también excluye $t=1$) es simplemente $C_1$.

* * *

### Resultado final

El conjunto donde la función vectorial es continua es:

$$
C_r = [0, 1) \cup (1, \infty)
$$

O, equivalentemente:

$$
C_r = \{ t \in \mathbb{R} \mid t \ge 0, t \ne 1 \}
$$

* * *

### Interpretación breve del resultado

La continuidad de $\mathbf{r}(t)$ requiere que las tres componentes sean continuas. La componente $r_1(t)$ impone las restricciones $t \ge 0$ (por la raíz) y $t \ne 1$ (por el denominador). La componente $r_3(t)$ también impone $t \ne 1$. La componente $r_2(t)$ no impone restricciones. El conjunto final debe satisfacer todas las condiciones simultáneamente, resultando en $t \ge 0$ y $t \ne 1$.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 7 inciso 1

### Enunciado del problema

Calcule, usando la definición, la derivada de la siguiente función:

$$
\mathbf{f}(t) = (2t + 1, t^2, \sin t)
$$

* * *

### Datos dados

- Función vectorial: $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$
    - $f_1(t) = 2t + 1$
    - $f_2(t) = t^2$
    - $f_3(t) = \sin t$
- Método solicitado: Usar la definición formal de la derivada (límite).

La definición de la derivada de una función vectorial es:

$$
\mathbf{f}'(t) = \lim_{h \to 0} \frac{\mathbf{f}(t + h) - \mathbf{f}(t)}{h}
$$

* * *

### Desarrollo paso a paso

La derivada de la función vectorial se calcula aplicando la definición del límite a cada una de sus componentes por separado.

**1\. Derivada de $f_1(t) = 2t + 1$**

$$
f_1'(t) = \lim_{h \to 0} \frac{f_1(t+h) - f_1(t)}{h}
$$

$$
f_1'(t) = \lim_{h \to 0} \frac{[2(t+h) + 1] - [2t + 1]}{h}
$$

$$
f_1'(t) = \lim_{h \to 0} \frac{2t + 2h + 1 - 2t - 1}{h}
$$

$$
f_1'(t) = \lim_{h \to 0} \frac{2h}{h}
$$

$$
f_1'(t) = \lim_{h \to 0} 2 = 2
$$

**2\. Derivada de $f_2(t) = t^2$**

$$
f_2'(t) = \lim_{h \to 0} \frac{f_2(t+h) - f_2(t)}{h}
$$

$$
f_2'(t) = \lim_{h \to 0} \frac{(t+h)^2 - t^2}{h}
$$

$$
f_2'(t) = \lim_{h \to 0} \frac{(t^2 + 2th + h^2) - t^2}{h}
$$

$$
f_2'(t) = \lim_{h \to 0} \frac{2th + h^2}{h}
$$

$$
f_2'(t) = \lim_{h \to 0} \frac{h(2t + h)}{h}
$$

$$
f_2'(t) = \lim_{h \to 0} (2t + h) = 2t + 0 = 2t
$$

**3\. Derivada de $f_3(t) = \sin t$**

$$
f_3'(t) = \lim_{h \to 0} \frac{f_3(t+h) - f_3(t)}{h}
$$

$$
f_3'(t) = \lim_{h \to 0} \frac{\sin(t+h) - \sin t}{h}
$$

Se utiliza la identidad trigonométrica de suma de ángulos: $\sin(A+B) = \sin A \cos B + \cos A \sin B$.

$$
f_3'(t) = \lim_{h \to 0} \frac{(\sin t \cos h + \cos t \sin h) - \sin t}{h}
$$

Reagrupamos los términos:

$$
f_3'(t) = \lim_{h \to 0} \left[ \frac{\sin t (\cos h - 1)}{h} + \frac{\cos t \sin h}{h} \right]
$$

Separamos los límites (ya que $\sin t$ y $\cos t$ son constantes respecto a $h$):

$$
f_3'(t) = (\sin t) \cdot \left( \lim_{h \to 0} \frac{\cos h - 1}{h} \right) + (\cos t) \cdot \left( \lim_{h \to 0} \frac{\sin h}{h} \right)
$$

Usamos los límites trigonométricos fundamentales:  
$\lim_{h \to 0} \frac{\sin h}{h} = 1$  
$\lim_{h \to 0} \frac{\cos h - 1}{h} = 0$

Sustituimos estos valores:

$$
f_3'(t) = (\sin t) \cdot (0) + (\cos t) \cdot (1)
$$

$$
f_3'(t) = \cos t
$$

* * *

### Resultado final

Combinando las derivadas de las tres componentes:

$$
\mathbf{f}'(t) = (f_1'(t), f_2'(t), f_3'(t))
$$

$$
\mathbf{f}'(t) = (2, 2t, \cos t)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{f}'(t) = (2, 2t, \cos t)$ es la función derivada de $\mathbf{f}(t)$ y representa el vector tangente (o vector velocidad) de la curva descrita por $\mathbf{f}(t)$ en cualquier punto $t$ donde está definida.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 7 inciso 2

### Enunciado del problema

Calcule, usando la definición, la derivada de la siguiente función:

$$
\mathbf{g}(t) = (\sqrt{t}, \frac{1}{t}, \cos t)
$$

* * *

### Datos dados

- Función vectorial: $\mathbf{g}(t) = (g_1(t), g_2(t), g_3(t))$
    - $g_1(t) = \sqrt{t}$
    - $g_2(t) = \frac{1}{t}$
    - $g_3(t) = \cos t$
- Método solicitado: Usar la definición formal de la derivada (límite).

La definición de la derivada de una función vectorial es:

$$
\mathbf{g}'(t) = \lim_{h \to 0} \frac{\mathbf{g}(t + h) - \mathbf{g}(t)}{h}
$$

* * *

### Desarrollo paso a paso

La derivada de la función vectorial se calcula aplicando la definición del límite a cada una de sus componentes por separado.

**1\. Derivada de $g_1(t) = \sqrt{t}$**

$$
g_1'(t) = \lim_{h \to 0} \frac{g_1(t+h) - g_1(t)}{h} = \lim_{h \to 0} \frac{\sqrt{t+h} - \sqrt{t}}{h}
$$

Al evaluar $h=0$, se obtiene una indeterminación $\frac{0}{0}$. Se resuelve por racionalización (multiplicando por el conjugado del numerador):

$$
g_1'(t) = \lim_{h \to 0} \left[ \frac{\sqrt{t+h} - \sqrt{t}}{h} \cdot \frac{\sqrt{t+h} + \sqrt{t}}{\sqrt{t+h} + \sqrt{t}} \right]
$$

$$
g_1'(t) = \lim_{h \to 0} \frac{(t+h) - t}{h(\sqrt{t+h} + \sqrt{t})}
$$

$$
g_1'(t) = \lim_{h \to 0} \frac{h}{h(\sqrt{t+h} + \sqrt{t})}
$$

$$
g_1'(t) = \lim_{h \to 0} \frac{1}{\sqrt{t+h} + \sqrt{t}}
$$

Evaluando el límite $h \to 0$ por sustitución directa:

$$
g_1'(t) = \frac{1}{\sqrt{t} + \sqrt{t}} = \frac{1}{2\sqrt{t}}
$$

**2\. Derivada de $g_2(t) = \frac{1}{t}$**

$$
g_2'(t) = \lim_{h \to 0} \frac{g_2(t+h) - g_2(t)}{h} = \lim_{h \to 0} \frac{\frac{1}{t+h} - \frac{1}{t}}{h}
$$

Se obtiene $\frac{0}{0}$. Se resuelve buscando un común denominador en el numerador:

$$
g_2'(t) = \lim_{h \to 0} \frac{1}{h} \left[ \frac{t - (t+h)}{t(t+h)} \right]
$$

$$
g_2'(t) = \lim_{h \to 0} \frac{1}{h} \left[ \frac{-h}{t(t+h)} \right]
$$

$$
g_2'(t) = \lim_{h \to 0} \frac{-1}{t(t+h)}
$$

Evaluando el límite $h \to 0$ por sustitución directa:

$$
g_2'(t) = \frac{-1}{t(t)} = -\frac{1}{t^2}
$$

**3\. Derivada de $g_3(t) = \cos t$**

$$
g_3'(t) = \lim_{h \to 0} \frac{g_3(t+h) - g_3(t)}{h} = \lim_{h \to 0} \frac{\cos(t+h) - \cos t}{h}
$$

Se obtiene $\frac{0}{0}$. Se utiliza la identidad trigonométrica de suma de ángulos: $\cos(A+B) = \cos A \cos B - \sin A \sin B$.

$$
g_3'(t) = \lim_{h \to 0} \frac{(\cos t \cos h - \sin t \sin h) - \cos t}{h}
$$

Reagrupamos los términos:

$$
g_3'(t) = \lim_{h \to 0} \left[ \frac{\cos t (\cos h - 1)}{h} - \frac{\sin t \sin h}{h} \right]
$$

Separamos los límites (tratando $t$ como constante respectiva a $h$):

$$
g_3'(t) = (\cos t) \cdot \left( \lim_{h \to 0} \frac{\cos h - 1}{h} \right) - (\sin t) \cdot \left( \lim_{h \to 0} \frac{\sin h}{h} \right)
$$

Usamos los límites trigonométricos fundamentales:  
$\lim_{h \to 0} \frac{\sin h}{h} = 1$  
$\lim_{h \to 0} \frac{\cos h - 1}{h} = 0$

Sustituimos estos valores:

$$
g_3'(t) = (\cos t) \cdot (0) - (\sin t) \cdot (1) = -\sin t
$$

* * *

### Resultado final

Combinando las derivadas de las tres componentes:

$$
\mathbf{g}'(t) = (g_1'(t), g_2'(t), g_3'(t))
$$

$$
\mathbf{g}'(t) = \left(\frac{1}{2\sqrt{t}}, -\frac{1}{t^2}, -\sin t\right)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{g}'(t)$ es la función derivada de $\mathbf{g}(t)$ y representa el vector tangente (o vector velocidad) de la curva descrita por $\mathbf{g}(t)$ para cualquier $t$ en su dominio de derivabilidad ($t > 0$).

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 8 inciso 1

### Enunciado del problema

Calcule la derivada de la función $\mathbf{f}(t) = (6t, -7t^2, t^3)$.  
(Se asume que la derivación se realiza componente a componente, según el teorema de derivación de funciones vectoriales).

* * *

### Datos dados

La función vectorial es $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$, donde las funciones componentes son:

- $f_1(t) = 6t$
- $f_2(t) = -7t^2$
- $f_3(t) = t^3$

* * *

### Desarrollo paso a paso

El teorema de derivación de funciones vectoriales establece que la derivada $\mathbf{f}'(t)$ se obtiene derivando cada componente de forma independiente. Se aplica la regla de la potencia $\frac{d}{dt}(ct^n) = cnt^{n-1}$ a cada componente.

**1\. Derivada de la Primera Componente ($f_1(t)$)**

$$
f_1'(t) = \frac{d}{dt}(6t) = 6 \cdot 1 \cdot t^{1-1} = 6t^0 = 6
$$

**2\. Derivada de la Segunda Componente ($f_2(t)$)**

$$
f_2'(t) = \frac{d}{dt}(-7t^2) = -7 \cdot (2t^{2-1}) = -14t
$$

**3\. Derivada de la Tercera Componente ($f_3(t)$)**

$$
f_3'(t) = \frac{d}{dt}(t^3) = 3 \cdot t^{3-1} = 3t^2
$$

* * *

### Resultado final

La derivada de la función vectorial es el vector ensamblado con las derivadas de las componentes:

$$
\mathbf{f}'(t) = (f_1'(t), f_2'(t), f_3'(t))
$$

$$
\mathbf{f}'(t) = (6, -14t, 3t^2)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{f}'(t) = (6, -14t, 3t^2)$ es la función derivada (vector tangente o vector velocidad) de la curva $\mathbf{f}(t)$ en cualquier punto $t$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 8 inciso 6

### Enunciado del problema

Calcule la derivada de la función $\mathbf{r}(t) = (t \sin t, t \cos t, t^2)$.  
(Se asume que la derivación se realiza componente a componente, según el teorema de derivación).

* * *

### Datos dados

La función vectorial es $\mathbf{r}(t) = (r_1(t), r_2(t), r_3(t))$, donde las funciones componentes son:

- $r_1(t) = t \sin t$
- $r_2(t) = t \cos t$
- $r_3(t) = t^2$

* * *

### Desarrollo paso a paso

El teorema de derivación de funciones vectoriales indica que la derivada $\mathbf{r}'(t)$ se obtiene derivando cada componente de forma independiente.

**1\. Derivada de $r_1(t)$ (Regla del Producto)**

Se aplica la regla del producto $\frac{d}{dt}(uv) = u'v + uv'$:

$$
\begin{aligned}
r_1'(t) &= \frac{d}{dt}(t \sin t) \\
        &= \left(\frac{d}{dt} t\right) \sin t + t \left(\frac{d}{dt} \sin t\right) \\
        &= (1)\sin t + t(\cos t) \\
        &= \sin t + t \cos t
\end{aligned}
$$

**2\. Derivada de $r_2(t)$ (Regla del Producto)**

Se aplica nuevamente la regla del producto:

$$
\begin{aligned}
r_2'(t) &= \frac{d}{dt}(t \cos t) \\
        &= \left(\frac{d}{dt} t\right) \cos t + t \left(\frac{d}{dt} \cos t\right) \\
        &= (1)\cos t + t(-\sin t) \\
        &= \cos t - t \sin t
\end{aligned}
$$

**3\. Derivada de $r_3(t)$ (Regla de la Potencia)**

Se aplica la regla de la potencia $\frac{d}{dt}(t^n) = nt^{n-1}$:

$$
r_3'(t) = \frac{d}{dt}(t^2) = 2t
$$

* * *

### Resultado final

La derivada de la función vectorial es el vector ensamblado con las derivadas de las componentes:

$$
\mathbf{r}'(t) = (\sin t + t \cos t, \cos t - t \sin t, 2t)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{r}'(t)$ es la función derivada (vector tangente o vector velocidad) de la curva $\mathbf{r}(t)$ en cualquier punto $t$.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 9 inciso 1

### Enunciado del problema

Determine $\mathbf{f}'$ si $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$.

* * *

### Datos dados

La función vectorial es $\mathbf{f}(t) = (f_1(t), f_2(t), f_3(t))$, donde las funciones componentes son:

- $f_1(t) = t$
- $f_2(t) = t^2$
- $f_3(t) = \frac{1}{3}t^3$

* * *

### Desarrollo paso a paso

La derivada de la función vectorial $\mathbf{f}(t)$ se obtiene derivando cada una de sus componentes con respecto a $t$, aplicando el teorema de derivación componente a componente. Se utiliza la Regla de la Potencia ($\frac{d}{dt} (ct^n) = cnt^{n-1}$).

Dada la función:

$$
\mathbf{f}(t) = \left( t, t^2, \frac{1}{3}t^3 \right)
$$

1.  **Derivada de la 1ª componente:**
    
    $$
    \frac{d}{dt}(t) = 1
    $$
    
2.  **Derivada de la 2ª componente:**
    
    $$
    \frac{d}{dt}(t^2) = 2t
    $$
    
3.  **Derivada de la 3ª componente:**
    
    $$
    \frac{d}{dt}\left(\frac{1}{3}t^3\right) = \frac{1}{3} (3t^2) = t^2
    $$
    

* * *

### Resultado final

La derivada de la función vectorial es:

$$
\mathbf{f}'(t) = (1, 2t, t^2)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{f}'(t) = (1, 2t, t^2)$ es la función derivada (vector tangente o vector velocidad) de la curva descrita por $\mathbf{f}(t)$ en cualquier punto $t$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 9 inciso 3

### Enunciado del problema

Determine $\mathbf{f}''(t)$ (la segunda derivada) si $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$.

* * *

### Datos dados

La función vectorial original es:

$$
\mathbf{f}(t) = \left(t, t^2, \frac{1}{3}t^3\right)
$$

* * *

### Desarrollo paso a paso

Para encontrar la segunda derivada $\mathbf{f}''(t)$, primero calculamos la primera derivada $\mathbf{f}'(t)$ y luego volvemos a derivar ese resultado.

**1\. Cálculo de la Primera Derivada $\mathbf{f}'(t)$**

Derivamos cada componente de $\mathbf{f}(t)$ con respecto a $t$:

$$
\mathbf{f}'(t) = \frac{d}{dt} \mathbf{f}(t) = \left( \frac{d}{dt}t, \frac{d}{dt}t^2, \frac{d}{dt}\left(\frac{1}{3}t^3\right) \right)
$$

- $\frac{d}{dt}(t) = 1$
- $\frac{d}{dt}(t^2) = 2t$
- $\frac{d}{dt}\left(\frac{1}{3}t^3\right) = \frac{1}{3} (3t^2) = t^2$

Por lo tanto, la primera derivada es:

$$
\mathbf{f}'(t) = (1, 2t, t^2)
$$

**2\. Cálculo de la Segunda Derivada $\mathbf{f}''(t)$**

A continuación, derivamos la primera derivada $\mathbf{f}'(t)$ componente a componente:

$$
\mathbf{f}''(t) = \frac{d}{dt} \mathbf{f}'(t) = \left( \frac{d}{dt}1, \frac{d}{dt}(2t), \frac{d}{dt}t^2 \right)
$$

- $\frac{d}{dt}(1) = 0$ (La derivada de una constante es 0)
- $\frac{d}{dt}(2t) = 2$
- $\frac{d}{dt}(t^2) = 2t$

* * *

### Resultado final

La segunda derivada de la función vectorial es:

$$
\mathbf{f}''(t) = (0, 2, 2t)
$$

* * *

### Interpretación breve del resultado

El vector $\mathbf{f}''(t) = (0, 2, 2t)$ representa el **vector aceleración** de la curva descrita por la función de posición $\mathbf{f}(t)$ en cualquier punto $t$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 9 inciso 6

### Enunciado del problema

Determine $(\mathbf{f} + \mathbf{g})'$ dadas las funciones:

$$
\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)
$$

$$
\mathbf{g}(t) = (\cos t, \sin t, t)
$$

* * *

### Datos dados

- Función 1: $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$
- Función 2: $\mathbf{g}(t) = (\cos t, \sin t, t)$
- Operación: Calcular la derivada de la suma, $(\mathbf{f} + \mathbf{g})'(t)$.

* * *

### Desarrollo paso a paso

Se utiliza la regla de la suma para la derivación de funciones vectoriales, la cual establece que la derivada de la suma es la suma de las derivadas:

$$
(\mathbf{f} + \mathbf{g})'(t) = \mathbf{f}'(t) + \mathbf{g}'(t)
$$

**1\. Calcular la derivada $\mathbf{f}'(t)$**

Se deriva $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$ componente a componente:

- $\frac{d}{dt}(t) = 1$
- $\frac{d}{dt}(t^2) = 2t$
- $\frac{d}{dt}\left(\frac{1}{3}t^3\right) = \frac{1}{3}(3t^2) = t^2$

Por lo tanto:

$$
\mathbf{f}'(t) = (1, 2t, t^2)
$$

**2\. Calcular la derivada $\mathbf{g}'(t)$**

Se deriva $\mathbf{g}(t) = (\cos t, \sin t, t)$ componente a componente:

- $\frac{d}{dt}(\cos t) = -\sin t$
- $\frac{d}{dt}(\sin t) = \cos t$
- $\frac{d}{dt}(t) = 1$

Por lo tanto:

$$
\mathbf{g}'(t) = (-\sin t, \cos t, 1)
$$

**3\. Sumar las derivadas $\mathbf{f}'(t) + \mathbf{g}'(t)$**

$$
(\mathbf{f} + \mathbf{g})'(t) = \mathbf{f}'(t) + \mathbf{g}'(t)
$$

$$
(\mathbf{f} + \mathbf{g})'(t) = (1, 2t, t^2) + (-\sin t, \cos t, 1)
$$

Se suman las componentes correspondientes:

$$
(\mathbf{f} + \mathbf{g})'(t) = (1 - \sin t, 2t + \cos t, t^2 + 1)
$$

* * *

### Resultado final

La derivada de la suma de las funciones vectoriales es:

$$
(\mathbf{f} + \mathbf{g})'(t) = (1 - \sin t, 2t + \cos t, t^2 + 1)
$$

* * *

### Interpretación breve del resultado

El resultado se puede verificar sumando primero las funciones $\mathbf{f}(t)$ y $\mathbf{g}(t)$, y luego derivando el vector resultante.

Suma: $\mathbf{f}(t) + \mathbf{g}(t) = (t + \cos t, t^2 + \sin t, \frac{1}{3}t^3 + t)$  
Derivada de la suma: $\frac{d}{dt}(\mathbf{f} + \mathbf{g}) = (1 - \sin t, 2t + \cos t, t^2 + 1)$.  
El resultado coincide, validando el cálculo.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 9 inciso 7

### Enunciado del problema

Determine la derivada del producto punto $(\mathbf{f} \cdot \mathbf{g})'(t)$ para las funciones vectoriales dadas.

* * *

### Datos dados

- Función 1: $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$
- Función 2: $\mathbf{g}(t) = (\cos t, \sin t, t)$

* * *

### Desarrollo paso a paso

Se utiliza la regla del producto para la derivada de un producto punto, que establece:

$$
(\mathbf{f} \cdot \mathbf{g})'(t) = \mathbf{f}'(t) \cdot \mathbf{g}(t) + \mathbf{f}(t) \cdot \mathbf{g}'(t)
$$

**Paso 1: Calcular las derivadas $\mathbf{f}'(t)$ y $\mathbf{g}'(t)$**

Se derivan las funciones $\mathbf{f}(t)$ y $\mathbf{g}(t)$ componente a componente:

$$
\mathbf{f}'(t) = \left( \frac{d}{dt}t, \frac{d}{dt}t^2, \frac{d}{dt}\left(\frac{1}{3}t^3\right) \right) = (1, 2t, t^2)
$$

$$
\mathbf{g}'(t) = \left( \frac{d}{dt}\cos t, \frac{d}{dt}\sin t, \frac{d}{dt}t \right) = (-\sin t, \cos t, 1)
$$

**Paso 2: Calcular el término $\mathbf{f}'(t) \cdot \mathbf{g}(t)$**

$$
\mathbf{f}'(t) \cdot \mathbf{g}(t) = (1, 2t, t^2) \cdot (\cos t, \sin t, t)
$$

$$
\mathbf{f}'(t) \cdot \mathbf{g}(t) = (1)(\cos t) + (2t)(\sin t) + (t^2)(t)
$$

$$
\mathbf{f}'(t) \cdot \mathbf{g}(t) = \cos t + 2t \sin t + t^3
$$

**Paso 3: Calcular el término $\mathbf{f}(t) \cdot \mathbf{g}'(t)$**

$$
\mathbf{f}(t) \cdot \mathbf{g}'(t) = \left(t, t^2, \frac{1}{3}t^3\right) \cdot (-\sin t, \cos t, 1)
$$

$$
\mathbf{f}(t) \cdot \mathbf{g}'(t) = (t)(-\sin t) + (t^2)(\cos t) + \left(\frac{1}{3}t^3\right)(1)
$$

$$
\mathbf{f}(t) \cdot \mathbf{g}'(t) = -t \sin t + t^2 \cos t + \frac{1}{3}t^3
$$

**Paso 4: Sumar los resultados (Paso 2 + Paso 3)**

$$
(\mathbf{f} \cdot \mathbf{g})'(t) = (\cos t + 2t \sin t + t^3) + (-t \sin t + t^2 \cos t + \frac{1}{3}t^3)
$$

Se agrupan los términos semejantes:

- Términos $\cos t$: $\cos t + t^2 \cos t = (1 + t^2)\cos t$
- Términos $\sin t$: $2t \sin t - t \sin t = t \sin t$
- Términos $t^3$: $t^3 + \frac{1}{3}t^3 = \frac{4}{3}t^3$

$$
(\mathbf{f} \cdot \mathbf{g})'(t) = (1 + t^2)\cos t + t \sin t + \frac{4}{3}t^3
$$

* * *

**Validación (Método Alternativo)**

Se valida el resultado calculando primero el producto punto (una función escalar $h(t)$) y luego derivando esa función.

1.  Calcular $h(t) = \mathbf{f}(t) \cdot \mathbf{g}(t)$:
    
    $$
    h(t) = (t, t^2, \frac{1}{3}t^3) \cdot (\cos t, \sin t, t)
    $$
    
    $$
    h(t) = t \cos t + t^2 \sin t + \frac{1}{3}t^4
    $$
    
2.  Derivar $h(t)$ usando la regla del producto y la regla de la potencia:
    
    $$
    h'(t) = \frac{d}{dt} \left( t \cos t \right) + \frac{d}{dt} \left( t^2 \sin t \right) + \frac{d}{dt} \left( \frac{1}{3}t^4 \right)
    $$
    
    $$
    h'(t) = [(1)\cos t + (t)(-\sin t)] + [(2t)\sin t + (t^2)(\cos t)] + \left[ \frac{4}{3}t^3 \right]
    $$
    
    $$
    h'(t) = (\cos t - t \sin t) + (2t \sin t + t^2 \cos t) + \frac{4}{3}t^3
    $$
    
3.  Agrupar términos:
    
    $$
    h'(t) = (\cos t + t^2 \cos t) + (-t \sin t + 2t \sin t) + \frac{4}{3}t^3
    $$
    
    $$
    h'(t) = (1 + t^2)\cos t + t \sin t + \frac{4}{3}t^3
    $$
    

El resultado de la validación coincide con el método principal.

* * *

### Resultado final

La derivada del producto punto es:

$$
(\mathbf{f} \cdot \mathbf{g})'(t) = (1 + t^2)\cos t + t \sin t + \frac{4}{3}t^3
$$

* * *

### Interpretación breve del resultado

El resultado es una función escalar, como se espera de la derivada de un producto punto (que es una función escalar). El cálculo se verificó usando dos métodos distintos (la regla del producto para producto punto y la derivación de la función escalar resultante), ambos arrojando el mismo resultado.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 9 inciso 9

### Enunciado del problema

Determine la derivada $(\alpha \mathbf{f})'(t)$, que es la derivada del producto de la función escalar $\alpha(t)$ por la función vectorial $\mathbf{f}(t)$.

* * *

### Datos dados

- Función escalar: $\alpha(t) = e^{-at}$
- Función vectorial: $\mathbf{f}(t) = (t, t^2, \frac{1}{3}t^3)$
- Regla a utilizar (Regla del Producto):
    
    $$
    (\alpha \mathbf{f})'(t) = \alpha'(t) \mathbf{f}(t) + \alpha(t) \mathbf{f}'(t)
    $$
    

* * *

### Desarrollo paso a paso

Se utiliza la regla del producto para una función escalar $\alpha(t)$ que multiplica a una función vectorial $\mathbf{f}(t)$.

**1\. Calcular las derivadas $\alpha'(t)$ y $\mathbf{f}'(t)$**

- **Derivada Escalar (Regla de la Cadena):**
    
    $$
    \alpha'(t) = \frac{d}{dt}(e^{-at}) = e^{-at} \cdot (-a) = -a e^{-at}
    $$
    
- **Derivada Vectorial (Regla de la Potencia):**
    
    $$
    \mathbf{f}'(t) = \frac{d}{dt}\left(t, t^2, \frac{1}{3}t^3\right) = (1, 2t, t^2)
    $$
    

**2\. Calcular el término $\alpha'(t) \mathbf{f}(t)$**

Se multiplica la derivada escalar $\alpha'(t)$ por el vector $\mathbf{f}(t)$:

$$
\alpha'(t) \mathbf{f}(t) = (-a e^{-at}) \cdot \left(t, t^2, \frac{1}{3}t^3\right)
$$

$$
\alpha'(t) \mathbf{f}(t) = \left( -at e^{-at}, -at^2 e^{-at}, -\frac{a}{3}t^3 e^{-at} \right)
$$

**3\. Calcular el término $\alpha(t) \mathbf{f}'(t)$**

Se multiplica la escalar $\alpha(t)$ por el vector derivado $\mathbf{f}'(t)$:

$$
\alpha(t) \mathbf{f}'(t) = (e^{-at}) \cdot (1, 2t, t^2)
$$

$$
\alpha(t) \mathbf{f}'(t) = \left( e^{-at}, 2t e^{-at}, t^2 e^{-at} \right)
$$

**4\. Sumar los resultados (Paso 2 + Paso 3)**

$$
(\alpha \mathbf{f})'(t) = \left( -at e^{-at}, -at^2 e^{-at}, -\frac{a}{3}t^3 e^{-at} \right) + \left( e^{-at}, 2t e^{-at}, t^2 e^{-at} \right)
$$

Se suman las componentes correspondientes:

- **Comp. 1:** $e^{-at} - at e^{-at} = (1 - at)e^{-at}$
- **Comp. 2:** $2t e^{-at} - at^2 e^{-at} = (2t - at^2)e^{-at}$
- **Comp. 3:** $t^2 e^{-at} - \frac{a}{3}t^3 e^{-at} = \left(t^2 - \frac{a}{3}t^3\right)e^{-at}$

* * *

### Resultado final

El vector resultante es:

$$
(\alpha \mathbf{f})'(t) = \left( (1 - at)e^{-at}, (2t - at^2)e^{-at}, \left(t^2 - \frac{a}{3}t^3\right)e^{-at} \right)
$$

Factorizando el término común $e^{-at}$:

$$
(\alpha \mathbf{f})'(t) = e^{-at} \left( 1 - at, 2t - at^2, t^2 - \frac{a}{3}t^3 \right)
$$

* * *

### Interpretación breve del resultado

El resultado se puede validar multiplicando primero $\mathbf{h}(t) = \alpha(t) \mathbf{f}(t) = (t e^{-at}, t^2 e^{-at}, \frac{1}{3}t^3 e^{-at})$ y luego derivando $\mathbf{h}(t)$ componente a componente, usando la regla del producto para funciones escalares en cada componente.

- $h_1'(t) = (1)e^{-at} + (t)(-a e^{-at}) = (1 - at)e^{-at}$
- $h_2'(t) = (2t)e^{-at} + (t^2)(-a e^{-at}) = (2t - at^2)e^{-at}$
- $h_3'(t) = (t^2)e^{-at} + (\frac{1}{3}t^3)(-a e^{-at}) = (t^2 - \frac{a}{3}t^3)e^{-at}$

El resultado coincide, validando el cálculo.

* * *

✅ *Cálculos verificados: correctos.*

* * *

# Problema 10 inciso 1

### Enunciado del problema

Calcule la integral definida de la siguiente función vectorial:

$$
\int_{0}^{\frac{\pi}{2}} (\sin t, \cos t, \tan t) dt
$$

* * *

### Datos dados

- Función vectorial: $\mathbf{f}(t) = (\sin t, \cos t, \tan t)$
- Límites de integración: $a = 0$ (inferior) y $b = \pi/2$ (superior).

* * *

### Desarrollo paso a paso

El teorema de integración vectorial establece que la integral de una función vectorial se calcula integrando cada componente por separado. La integral vectorial $\mathbf{I}$ existe si y solo si las integrales de todas sus componentes convergen.

$$
\mathbf{I} = \left( \int_{0}^{\pi/2} \sin t \, dt, \int_{0}^{\pi/2} \cos t \, dt, \int_{0}^{\pi/2} \tan t \, dt \right)
$$

**1\. Integral de la Componente 1 ($I_1$)**

$$
I_1 = \int_{0}^{\pi/2} \sin t \, dt
$$

La antiderivada es $-\cos t$. Usando el Teorema Fundamental del Cálculo:

$$
I_1 = [-\cos t]_{0}^{\pi/2} = \left(-\cos\left(\frac{\pi}{2}\right)\right) - (-\cos(0))
$$

$$
I_1 = (0) - (-1) = 1
$$

Esta integral converge.

**2\. Integral de la Componente 2 ($I_2$)**

$$
I_2 = \int_{0}^{\pi/2} \cos t \, dt
$$

La antiderivada es $\sin t$.

$$
I_2 = [\sin t]_{0}^{\pi/2} = \sin\left(\frac{\pi}{2}\right) - \sin(0)
$$

$$
I_2 = (1) - (0) = 1
$$

Esta integral converge.

**3\. Integral de la Componente 3 ($I_3$)**

$$
I_3 = \int_{0}^{\pi/2} \tan t \, dt
$$

Esta es una **integral impropia** porque la función $\tan t$ tiene una asíntota vertical (discontinuidad infinita) en el límite superior de integración, $t = \pi/2$.

Debemos evaluarla usando un límite:

$$
I_3 = \lim_{b \to (\pi/2)^-} \int_{0}^{b} \tan t \, dt
$$

La antiderivada de $\tan t$ es $-\ln|\cos t|$:

$$
I_3 = \lim_{b \to (\pi/2)^-} [-\ln|\cos t|]_{0}^{b}
$$

$$
I_3 = \lim_{b \to (\pi/2)^-} \left( (-\ln|\cos b|) - (-\ln|\cos 0|) \right)
$$

$$
I_3 = \lim_{b \to (\pi/2)^-} \left( -\ln|\cos b| - (-\ln(1)) \right)
$$

$$
I_3 = \lim_{b \to (\pi/2)^-} (-\ln|\cos b| - 0)
$$

A medida que $b$ se acerca a $\pi/2$ por la izquierda, $\cos b$ se acerca a $0^+$. El logaritmo natural de un número que tiende a $0^+$ es $-\infty$.

$$
I_3 = \lim_{b \to (\pi/2)^-} -(-\infty) = +\infty
$$

La integral de la tercera componente diverge.

* * *

### Resultado final

La integral de la tercera componente, $\int_{0}^{\pi/2} \tan t \, dt$, diverge a $+\infty$.

Dado que al menos una de las componentes diverge, la integral de la función vectorial no existe.

**La integral no existe (o diverge).**

* * *

### Interpretación breve del resultado

Para que la integral de una función vectorial exista (converja), las integrales de todas sus funciones componentes deben converger. En este caso, aunque las integrales de $\sin t$ y $\cos t$ convergen en el intervalo $[0, \pi/2]$, la integral de $\tan t$ no lo hace debido a la asíntota vertical en $t = \pi/2$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 10 inciso 3

### Enunciado del problema

Calcule la integral definida de la siguiente función vectorial:

$$
\int_{0}^{2} (t, t e^t, -t e^t) dt
$$

* * *

### Datos dados

- Función vectorial: $\mathbf{f}(t) = (t, t e^t, -t e^t)$
- Límites de integración: $a = 0$ (inferior) y $b = 2$ (superior).

* * *

### Desarrollo paso a paso

El teorema de integración vectorial establece que la integral de una función vectorial se calcula integrando cada componente por separado.

$$
\mathbf{I} = \left( \int_{0}^{2} t \, dt, \int_{0}^{2} t e^t \, dt, \int_{0}^{2} -t e^t \, dt \right)
$$

**1\. Integral de la Componente 1 ($I_1$)**

$$
I_1 = \int_{0}^{2} t \, dt
$$

Usando la regla de la potencia para la antiderivada:

$$
I_1 = \left[ \frac{t^2}{2} \right]_{0}^{2}
$$

Evaluando con el Teorema Fundamental del Cálculo (T.F.C.):

$$
I_1 = \left( \frac{(2)^2}{2} \right) - \left( \frac{(0)^2}{2} \right) = \frac{4}{2} - 0 = 2
$$

**2\. Integral de la Componente 2 ($I_2$)**

$$
I_2 = \int_{0}^{2} t e^t \, dt
$$

Se utiliza **integración por partes**: $\int u \, dv = uv - \int v \, du$.

- Sea $u = t \implies du = dt$.
- Sea $dv = e^t \, dt \implies v = e^t$.

La antiderivada es:

$$
\int t e^t \, dt = (t)(e^t) - \int e^t \, dt = t e^t - e^t = e^t(t - 1)
$$

Evaluando con el T.F.C.:

$$
I_2 = [e^t(t - 1)]_{0}^{2}
$$

$$
I_2 = (e^2(2 - 1)) - (e^0(0 - 1))
$$

$$
I_2 = (e^2 \cdot 1) - (1 \cdot -1) = e^2 + 1
$$

**3\. Integral de la Componente 3 ($I_3$)**

$$
I_3 = \int_{0}^{2} -t e^t \, dt
$$

Usando la propiedad de linealidad de la integral:

$$
I_3 = - \int_{0}^{2} t e^t \, dt = -I_2
$$

Dado que $I_2 = e^2 + 1$:

$$
I_3 = -(e^2 + 1) = -e^2 - 1
$$

* * *

### Resultado final

El vector resultante de la integral definida es:

$$
\mathbf{I} = (2, e^2 + 1, -e^2 - 1)
$$

* * *

### Interpretación breve del resultado

La integral de la función vectorial $\mathbf{f}(t)$ en el intervalo $[0, 2]$ es el vector $(2, e^2 + 1, -e^2 - 1)$. Este resultado se obtiene al integrar cada una de las componentes ($t$, $t e^t$ y $-t e^t$) de forma independiente.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 10 inciso 6

### Enunciado del problema

Calcule la integral indefinida de la siguiente función vectorial:

$$
\int (\sin t, \cos t, e^t) dt
$$

* * *

### Datos dados

- Función vectorial a integrar (integrando): $\mathbf{f}(t) = (\sin t, \cos t, e^t)$
- Se busca la integral indefinida (antiderivada) de $\mathbf{f}(t)$.

* * *

### Desarrollo paso a paso

El teorema de integración vectorial establece que la integral indefinida de una función vectorial se calcula integrando cada componente por separado.

$$
\int \mathbf{f}(t) dt = \int (\sin t, \cos t, e^t) dt = \left( \int \sin t \, dt, \int \cos t \, dt, \int e^t \, dt \right)
$$

1.  **Integral de la Componente 1:**
    
    $$
    \int \sin t \, dt = -\cos t + C_1
    $$
    
2.  **Integral de la Componente 2:**
    
    $$
    \int \cos t \, dt = \sin t + C_2
    $$
    
3.  **Integral de la Componente 3:**
    
    $$
    \int e^t \, dt = e^t + C_3
    $$
    

* * *

### Resultado final

El vector resultante se ensambla con las antiderivadas de cada componente. Las constantes de integración escalares ($C_1, C_2, C_3$) se agrupan en un **vector constante de integración** $\mathbf{C}$.

$$
\mathbf{R}(t) = (-\cos t + C_1, \sin t + C_2, e^t + C_3)
$$

Expresado de forma compacta:

$$
\mathbf{R}(t) = (-\cos t, \sin t, e^t) + \mathbf{C}
$$

donde $\mathbf{C} = (C_1, C_2, C_3)$.

* * *

### Interpretación breve del resultado

La integral indefinida de $\mathbf{f}(t)$ es la familia de funciones vectoriales $\mathbf{R}(t)$. Se puede verificar el resultado derivando $\mathbf{R}(t)$:

$$
\mathbf{R}'(t) = \frac{d}{dt} ((-\cos t, \sin t, e^t) + \mathbf{C}) = (\sin t, \cos t, e^t)
$$

La derivada del resultado coincide con el integrando original $\mathbf{f}(t)$.

* * *

✅ *Cálculos verificados: correctos.*

# Problema 10 inciso 7

### Enunciado del problema

Calcule la integral indefinida de la siguiente función vectorial:

$$
\int (e^{-t} \sin t, e^{-t} \cos t, e^{-t}) dt
$$

* * *

### Datos dados

- Función vectorial a integrar (integrando): $\mathbf{f}(t) = (e^{-t} \sin t, e^{-t} \cos t, e^{-t})$
- Se busca la integral indefinida (antiderivada) de $\mathbf{f}(t)$.

* * *

### Desarrollo paso a paso

La integral indefinida de una función vectorial se calcula integrando cada componente por separado.

$$
\int \mathbf{f}(t) dt = \left( \int e^{-t} \sin t \, dt, \int e^{-t} \cos t \, dt, \int e^{-t} \, dt \right)
$$

**1\. Integral de la Componente 3 ($I_3$)**

Esta es la integral más directa y se resuelve primero:

$$
I_3 = \int e^{-t} \, dt = -e^{-t} + C_3
$$

**2\. Integral de las Componentes 1 y 2 ($I_1, I_2$)**

Las integrales $I_1 = \int e^{-t} \sin t \, dt$ y $I_2 = \int e^{-t} \cos t \, dt$ requieren **integración por partes** ($\int u \, dv = uv - \int v \, du$). Se pueden resolver de forma simultánea.

**Cálculo de $I_1$:**

- Sea $u = \sin t \implies du = \cos t \, dt$
- Sea $dv = e^{-t} \, dt \implies v = -e^{-t}$

$$
I_1 = (\sin t)(-e^{-t}) - \int (-e^{-t})(\cos t \, dt)
$$

$$
I_1 = -e^{-t} \sin t + \int e^{-t} \cos t \, dt
$$

Dado que $I_2 = \int e^{-t} \cos t \, dt$, tenemos la Ecuación A:

$$
I_1 = -e^{-t} \sin t + I_2 \quad (\text{Ecuación A})
$$

**Cálculo de $I_2$:**

- Sea $u = \cos t \implies du = -\sin t \, dt$
- Sea $dv = e^{-t} \, dt \implies v = -e^{-t}$

$$
I_2 = (\cos t)(-e^{-t}) - \int (-e^{-t})(-\sin t \, dt)
$$

$$
I_2 = -e^{-t} \cos t - \int e^{-t} \sin t \, dt
$$

Dado que $I_1 = \int e^{-t} \sin t \, dt$, tenemos la Ecuación B:

$$
I_2 = -e^{-t} \cos t - I_1 \quad (\text{Ecuación B})
$$

**Resolución del sistema:**  
Sustituimos (B) en (A):

$$
I_1 = -e^{-t} \sin t + (-e^{-t} \cos t - I_1)
$$

$$
2I_1 = -e^{-t} (\sin t + \cos t)
$$

$$
I_1 = -\frac{1}{2} e^{-t} (\sin t + \cos t) + C_1
$$

Sustituimos $I_1$ en (B) para hallar $I_2$:

$$
I_2 = -e^{-t} \cos t - \left[ -\frac{1}{2} e^{-t} (\sin t + \cos t) \right]
$$

$$
I_2 = -e^{-t} \cos t + \frac{1}{2} e^{-t} \sin t + \frac{1}{2} e^{-t} \cos t
$$

$$
I_2 = \frac{1}{2} e^{-t} \sin t - \frac{1}{2} e^{-t} \cos t
$$

$$
I_2 = \frac{1}{2} e^{-t} (\sin t - \cos t) + C_2
$$

* * *

### Resultado final

Se ensambla el vector con las antiderivadas de cada componente, agrupando las constantes $(C_1, C_2, C_3)$ en un vector constante $\mathbf{C}$.

$$
\mathbf{R}(t) = \left( -\frac{1}{2} e^{-t}(\sin t + \cos t), \frac{1}{2} e^{-t}(\sin t - \cos t), -e^{-t} \right) + \mathbf{C}
$$

* * *

### Interpretación breve del resultado

La integral indefinida de $\mathbf{f}(t)$ es la familia de funciones vectoriales $\mathbf{R}(t)$. Se puede verificar el resultado derivando $\mathbf{R}(t)$:

- $\frac{d}{dt} R_1(t) = \frac{d}{dt} [-\frac{1}{2} e^{-t}(\sin t + \cos t)] = e^{-t} \sin t$.
- $\frac{d}{dt} R_2(t) = \frac{d}{dt} [\frac{1}{2} e^{-t}(\sin t - \cos t)] = e^{-t} \cos t$.
- $\frac{d}{dt} R_3(t) = \frac{d}{dt} [-e^{-t}] = e^{-t}$.

La derivada del resultado coincide con el integrando original $\mathbf{f}(t)$.

* * *

✅ *Cálculos verificados: correctos.*