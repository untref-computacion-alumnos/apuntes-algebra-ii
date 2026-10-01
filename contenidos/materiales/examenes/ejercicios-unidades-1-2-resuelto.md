# Ejercicios de parcial — Unidades 1 y 2 (resuelto)

Ejercicios para practicar el **primer parcial** (Unidades 1 y 2), pensados para usar junto con el [machete de fórmulas](../formulas.md). Esta versión incluye **consignas y resoluciones**; para practicar sin ver las respuestas, usá [la versión de consignas](ejercicios-unidades-1-2.md).

:::{note} Cómo está armado
- **Parte A:** ejercicios de parciales y recuperatorios anteriores (2024) que entran en Unidades 1–2. Son los ejercicios 1 y 2 de cada examen.
- **Parte B:** matrices, sistemas y determinantes (Unidad 1). Ningún parcial anterior los incluye, pero están en el temario.
- **Parte C:** coordenadas y vectores (Unidad 2).
- **Parte D:** integradores, que mezclan matrices, sistemas y vectores.

En cada ejercicio, *Repasá* indica la sección del machete que conviene tener a mano.
:::

:::{important} Quedaron afuera
Los ejercicios 3 y 4 de cada examen (rectas, planos y cónicas) son de las Unidades 3–4, es decir, del **segundo parcial**. Siguen disponibles en los archivos de cada examen.
:::

---

# Parte A — Ejercicios de parciales anteriores

> Fuente: *Parciales tomados otros cuatrimestres* del Cuadernillo de Álgebra II (Ingeniería en Computación, UNTREF). Los enunciados completos están en [parcial 10/06](parcial-2024-06-10.md), [recuperatorio 24/06](recuperatorio-2024-06-24.md), [parcial 04/11](parcial-2024-11-04.md) y [recuperatorio 11/11](recuperatorio-2024-11-11.md).

## A1. Parcial 10/06/2024 — Ejercicio 1 (30 pts)

Los siguientes puntos están expresados en coordenadas cartesianas: $A=(0,4)$ y $B=(-1,1)$.

a) Expresá los dos puntos en coordenadas polares.

b) Calculá la distancia entre $A$ y $B$.

c) Hallá todos los puntos $P\in\mathbb{R}^2$ tales que $d(P,A)=d(P,B)$.

*Repasá:* secciones 6 y 7.

### Resolución

**a)** Para $A=(0,4)$: $\rho=4$, y está sobre el eje $y$ positivo, así que $\theta=\frac{\pi}{2}$.

Para $B=(-1,1)$: $\rho=\sqrt{1+1}=\sqrt2$, y está en el 2.º cuadrante con $\tan\theta=-1$, así que $\theta=\frac{3\pi}{4}$.

$$A=\left(4,\tfrac{\pi}{2}\right)\qquad B=\left(\sqrt2,\tfrac{3\pi}{4}\right)$$

**b)**
$$d(A,B)=\sqrt{(0+1)^2+(4-1)^2}=\sqrt{1+9}=\boxed{\sqrt{10}}$$

**c)** Es la mediatriz del segmento $AB$:

$$x^2+(y-4)^2=(x+1)^2+(y-1)^2$$

$$x^2+y^2-8y+16=x^2+2x+1+y^2-2y+1\ \Longrightarrow\ 2x+6y=14$$

$$\boxed{x+3y=7}$$

Son todos los puntos de esa recta.

## A2. Parcial 10/06/2024 — Ejercicio 2 (20 pts)

Sean $v=(1,2,1)$ y $w=(k,0,1)$ con $k\in\mathbb{R}$.

a) Hallá $k$ para que el ángulo entre $v$ y $w$ sea $\frac{\pi}{2}$.

b) Para $k=2$, encontrá un vector $u$ tal que:

- $u$ es ortogonal a $v$.
- $u$ es ortogonal a $w$.
- $\|u\|=2$.

*Repasá:* secciones 8 y 9.

### Resolución

**a)** El ángulo es $\frac{\pi}{2}$ si y solo si $v\cdot w=0$:

$$v\cdot w=k+0+1=0\ \Longrightarrow\ \boxed{k=-1}$$

**b)** Con $k=2$, $w=(2,0,1)$. Un vector ortogonal a ambos es el producto vectorial:

$$v\times w=(1,2,1)\times(2,0,1)=(2\cdot1-1\cdot0,\ 1\cdot2-1\cdot1,\ 1\cdot0-2\cdot2)=(2,1,-4)$$

Verificación: $v\cdot(2,1,-4)=2+2-4=0$ y $w\cdot(2,1,-4)=4-4=0$.

Su norma es $\sqrt{4+1+16}=\sqrt{21}$, entonces:

$$\boxed{u=\frac{2}{\sqrt{21}}(2,1,-4)=\left(\tfrac{4}{\sqrt{21}},\tfrac{2}{\sqrt{21}},-\tfrac{8}{\sqrt{21}}\right)}$$

(también sirve $-u$).

## A3. Recuperatorio 24/06/2024 — Ejercicio 1 (30 pts)

Sea $T$ el triángulo definido por los vértices $A=(1,0)$, $B=(5,0)$ y $C=(3,\sqrt3)$.

a) Expresá a los tres puntos en coordenadas polares.

b) Hallá el perímetro del triángulo $T$.

c) ¿Es rectángulo el triángulo $T$?

*Repasá:* secciones 6, 7 y 8.

### Resolución

**a)**

- $A=(1,0)$: $\rho=1$, $\theta=0$.
- $B=(5,0)$: $\rho=5$, $\theta=0$.
- $C=(3,\sqrt3)$: $\rho=\sqrt{9+3}=2\sqrt3$, $\tan\theta=\frac{\sqrt3}{3}$, 1.er cuadrante, entonces $\theta=\frac{\pi}{6}$.

$$A=(1,0)\qquad B=(5,0)\qquad C=\left(2\sqrt3,\tfrac{\pi}{6}\right)$$

**b)** Lados:

$$AB=4,\qquad AC=\sqrt{2^2+3}=\sqrt7,\qquad BC=\sqrt{(-2)^2+3}=\sqrt7$$

$$\boxed{\text{Perímetro}=4+2\sqrt7}$$

**c)** El lado mayor es $AB=4$. Verificamos Pitágoras:

$$AC^2+BC^2=7+7=14\neq16=AB^2$$

**No es rectángulo** (es isósceles, con $AC=BC$).

## A4. Recuperatorio 24/06/2024 — Ejercicio 2 (20 pts)

Sea $v=(1,k,k-1)$ con $k\in\mathbb{R}$.

a) Hallá, si es posible, $k$ para que $v$ sea ortogonal a $u=(2,1,-1)$.

b) Para $k=1$, encontrá un vector $w$ tal que:

- $w$ es ortogonal a $u$.
- $w$ no es ortogonal a $v$.
- $\|w\|=1$.

*Repasá:* sección 8 (en particular "Construir un vector con condiciones").

### Resolución

**a)** $v\cdot u=2+k-(k-1)=3\neq0$ para todo $k$.

**No es posible**: no existe $k$ que haga a $v$ ortogonal a $u$.

**b)** Con $k=1$, $v=(1,1,0)$. Buscamos $w=(x,y,z)$ con $u\cdot w=2x+y-z=0$ y $v\cdot w=x+y\neq0$.

Por ejemplo, $w'=(1,0,2)$: $u\cdot w'=2-2=0$ ✓ y $v\cdot w'=1\neq0$ ✓. Su norma es $\sqrt5$, entonces:

$$\boxed{w=\frac{1}{\sqrt5}(1,0,2)}$$

## A5. Parcial 04/11/2024 — Ejercicio 1 (25 pts)

Los puntos $A=\left(5,\frac{\pi}{3}\right)$ y $B=\left(5,\frac{5\pi}{3}\right)$ están expresados en coordenadas polares.

a) Graficá los puntos $A$ y $B$.

b) Calculá la distancia entre los puntos $A$ y $B$.

c) Determiná las coordenadas cartesianas de un punto $C$ que cumpla las siguientes condiciones:

- i. La distancia de $C$ al punto $A$ es el doble de la distancia entre $A$ y $B$.
- ii. $C$ pertenece a la recta que pasa por $A$ y por $B$.

d) ¿Es única la ubicación de $C$? Justificá la respuesta.

*Repasá:* secciones 6 y 7.

### Resolución

**a)** Ambos puntos están a distancia $\rho=5$ del origen. $A$ está a $60^\circ$ (1.er cuadrante) y $B$ a $300^\circ$ (4.º cuadrante).

**b)** Pasando a cartesianas:

$$A=\left(5\cos\tfrac{\pi}{3},5\sin\tfrac{\pi}{3}\right)=\left(\tfrac52,\tfrac{5\sqrt3}{2}\right),\qquad B=\left(5\cos\tfrac{5\pi}{3},5\sin\tfrac{5\pi}{3}\right)=\left(\tfrac52,-\tfrac{5\sqrt3}{2}\right)$$

$$\boxed{d(A,B)=\tfrac{5\sqrt3}{2}+\tfrac{5\sqrt3}{2}=5\sqrt3}$$

**c)** $A$ y $B$ tienen la misma abscisa, así que la recta $AB$ es $x=\frac52$. Un punto de ella es $C=\left(\frac52,y\right)$ y debe cumplir:

$$d(C,A)=\left|y-\tfrac{5\sqrt3}{2}\right|=2\cdot5\sqrt3=10\sqrt3$$

$$y=\tfrac{5\sqrt3}{2}\pm10\sqrt3\ \Longrightarrow\ y=\tfrac{25\sqrt3}{2}\ \text{ o }\ y=-\tfrac{15\sqrt3}{2}$$

Por ejemplo:

$$\boxed{C=\left(\tfrac52,\tfrac{25\sqrt3}{2}\right)}$$

**d)** **No es única**: hay dos puntos sobre la recta a esa distancia de $A$, uno a cada lado:

$$C_1=\left(\tfrac52,\tfrac{25\sqrt3}{2}\right),\qquad C_2=\left(\tfrac52,-\tfrac{15\sqrt3}{2}\right)$$

## A6. Parcial 04/11/2024 — Ejercicio 2 (15 pts)

Considerá el vector $v=(4,2,-1)$. Encontrá, si es posible, dos vectores $w_1$ y $w_2$ que sean ortogonales entre sí y que también sean ortogonales a $v$.

*Repasá:* secciones 8 y 9.

### Resolución

Sí es posible. Buscamos $w_1=(a,b,c)$ con $4a+2b-c=0$; por ejemplo $w_1=(1,-2,0)$ ($4-4=0$ ✓).

Para $w_2$ tomamos el producto vectorial, que es ortogonal a ambos:

$$v\times w_1=(4,2,-1)\times(1,-2,0)=(2\cdot0-(-1)(-2),\ (-1)(1)-4\cdot0,\ 4(-2)-2\cdot1)=(-2,-1,-10)$$

Tomando el opuesto: $w_2=(2,1,10)$.

Verificación: $v\cdot w_2=8+2-10=0$ ✓ y $w_1\cdot w_2=2-2+0=0$ ✓.

$$\boxed{w_1=(1,-2,0)\qquad w_2=(2,1,10)}$$

## A7. Recuperatorio 11/11/2024 — Ejercicio 1 (20 pts)

Sea el triángulo $KLM$ con vértices en $K=(1,2)$, $L=(4,5)$ y $M=(1,5)$.

a) Determiná las coordenadas polares de los vértices del triángulo.

b) Calculá la longitud de cada lado del triángulo.

c) Verificá si el triángulo $KLM$ es un triángulo rectángulo.

*Repasá:* secciones 6, 7 y 8.

### Resolución

**a)**

- $K=(1,2)$: $\rho=\sqrt5$, $\theta=\arctan2\approx1{,}107$ rad ($63{,}43^\circ$).
- $L=(4,5)$: $\rho=\sqrt{41}$, $\theta=\arctan\frac54\approx0{,}896$ rad ($51{,}34^\circ$).
- $M=(1,5)$: $\rho=\sqrt{26}$, $\theta=\arctan5\approx1{,}373$ rad ($78{,}69^\circ$).

Los tres están en el 1.er cuadrante.

**b)**

$$KL=\sqrt{3^2+3^2}=3\sqrt2,\qquad LM=\sqrt{3^2+0^2}=3,\qquad KM=\sqrt{0^2+3^2}=3$$

**c)** El lado mayor es $KL$. Verificamos Pitágoras:

$$KM^2+LM^2=9+9=18=(3\sqrt2)^2=KL^2$$

**Sí es rectángulo**, con el ángulo recto en $M$ (además es isósceles).

## A8. Recuperatorio 11/11/2024 — Ejercicio 2 (30 pts)

Sea el vector $a=(2,k,k+3)$ con $k\in\mathbb{R}$.

a) Encontrá, si existe, un valor de $k$ tal que el vector $a$ sea ortogonal a $b=(3,-1,2)$.

b) Si $k=4$, encontrá, si es posible, un vector $c$ tal que:

- $c$ es ortogonal a $b$.
- $c$ no es ortogonal a $a$.
- $\|c\|=2$.

*Repasá:* sección 8.

### Resolución

**a)** $a\cdot b=6-k+2(k+3)=k+12=0\Rightarrow\boxed{k=-12}$.

**b)** Con $k=4$, $a=(2,4,7)$. Buscamos $c=(x,y,z)$ con $3x-y+2z=0$ y $a\cdot c\neq0$.

Por ejemplo $c'=(0,2,1)$: $b\cdot c'=-2+2=0$ ✓ y $a\cdot c'=8+7=15\neq0$ ✓. Su norma es $\sqrt5$, así que para tener norma 2:

$$\boxed{c=\frac{2}{\sqrt5}(0,2,1)=\left(0,\tfrac{4}{\sqrt5},\tfrac{2}{\sqrt5}\right)}$$

---

# Parte B — Matrices, sistemas y determinantes

## B1. Operaciones con matrices

Sean
$$A=\begin{pmatrix}1&2\\0&-1\\3&1\end{pmatrix},\qquad B=\begin{pmatrix}2&0&1\\1&-1&4\end{pmatrix},\qquad C=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}$$

a) Calculá $2C-A$.

b) Calculá $AB$ y $BA$. ¿Son iguales? ¿Por qué?

c) Verificá que $(AB)^t=B^tA^t$.

*Repasá:* sección 2.

### Resolución

**a)**
$$2C-A=\begin{pmatrix}2&0\\4&2\\-2&6\end{pmatrix}-\begin{pmatrix}1&2\\0&-1\\3&1\end{pmatrix}=\boxed{\begin{pmatrix}1&-2\\4&3\\-5&5\end{pmatrix}}$$

**b)** $A\in\mathbb{R}^{3\times2}$ y $B\in\mathbb{R}^{2\times3}$, así que $AB\in\mathbb{R}^{3\times3}$ y $BA\in\mathbb{R}^{2\times2}$.

$$AB=\begin{pmatrix}1\cdot2+2\cdot1&1\cdot0+2(-1)&1\cdot1+2\cdot4\\0\cdot2+(-1)1&0+(-1)(-1)&0+(-1)4\\3\cdot2+1\cdot1&3\cdot0+1(-1)&3\cdot1+1\cdot4\end{pmatrix}=\boxed{\begin{pmatrix}4&-2&9\\-1&1&-4\\7&-1&7\end{pmatrix}}$$

$$BA=\begin{pmatrix}2\cdot1+0\cdot0+1\cdot3&2\cdot2+0(-1)+1\cdot1\\1\cdot1+(-1)0+4\cdot3&1\cdot2+(-1)(-1)+4\cdot1\end{pmatrix}=\boxed{\begin{pmatrix}5&5\\13&7\end{pmatrix}}$$

**No son iguales**: ni siquiera tienen el mismo tamaño ($3\times3$ contra $2\times2$). El producto no es conmutativo.

**c)**
$$(AB)^t=\begin{pmatrix}4&-1&7\\-2&1&-1\\9&-4&7\end{pmatrix},\qquad B^tA^t=\begin{pmatrix}2&1\\0&-1\\1&4\end{pmatrix}\begin{pmatrix}1&0&3\\2&-1&1\end{pmatrix}=\begin{pmatrix}4&-1&7\\-2&1&-1\\9&-4&7\end{pmatrix}$$

Coinciden ✓.

## B2. Simétrica más antisimétrica

Sea
$$Q=\begin{pmatrix}1&4&-2\\0&3&6\\2&-2&5\end{pmatrix}$$

a) Hallá una matriz simétrica $S$ y una antisimétrica $K$ tales que $Q=S+K$.

b) Verificá que $S^t=S$, que $K^t=-K$ y que $S+K=Q$.

*Repasá:* secciones 1 y 2.

### Resolución

**a)** Se usa $S=\frac12(Q+Q^t)$ y $K=\frac12(Q-Q^t)$, con
$$Q^t=\begin{pmatrix}1&0&2\\4&3&-2\\-2&6&5\end{pmatrix}$$

$$S=\frac12\begin{pmatrix}2&4&0\\4&6&4\\0&4&10\end{pmatrix}=\boxed{\begin{pmatrix}1&2&0\\2&3&2\\0&2&5\end{pmatrix}}\qquad K=\frac12\begin{pmatrix}0&4&-4\\-4&0&8\\4&-8&0\end{pmatrix}=\boxed{\begin{pmatrix}0&2&-2\\-2&0&4\\2&-4&0\end{pmatrix}}$$

**b)** $S$ es simétrica (se refleja respecto de la diagonal: $s_{12}=s_{21}=2$, $s_{23}=s_{32}=2$, $s_{13}=s_{31}=0$). $K$ tiene la diagonal en cero y $k_{ij}=-k_{ji}$ (por ejemplo $k_{12}=2$ y $k_{21}=-2$), así que $K^t=-K$.

Y $S+K=\begin{pmatrix}1&4&-2\\0&3&6\\2&-2&5\end{pmatrix}=Q$ ✓.

## B3. Verdadero o falso

Decidí si cada afirmación es verdadera o falsa para $A,B,C\in\mathbb{R}^{n\times n}$. Si es falsa, dá un **contraejemplo** ($n=2$); si es verdadera, justificá.

a) $AB=AC\Rightarrow B=C$.

b) $(A+B)^2=A^2+2AB+B^2$.

c) $\det(A+B)=\det A+\det B$.

d) Si $A$ es inversible y $AB=AC$, entonces $B=C$.

e) $AA^t$ es simétrica.

*Repasá:* secciones 2, 3 y 4.

### Resolución

**a) Falsa.** Con $A=\begin{pmatrix}1&0\\0&0\end{pmatrix}$, $B=\begin{pmatrix}1&1\\0&0\end{pmatrix}$ y $C=\begin{pmatrix}1&1\\5&7\end{pmatrix}$:

$$AB=\begin{pmatrix}1&1\\0&0\end{pmatrix}=AC\qquad\text{pero }B\neq C$$

**b) Falsa.** Vale solo si $AB=BA$. Con $A=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ y $B=\begin{pmatrix}0&0\\1&0\end{pmatrix}$ se tiene $A+B=\begin{pmatrix}0&1\\1&0\end{pmatrix}$, entonces $(A+B)^2=I$. En cambio $A^2=B^2=N$ y $2AB=\begin{pmatrix}2&0\\0&0\end{pmatrix}$, así que $A^2+2AB+B^2=\begin{pmatrix}2&0\\0&0\end{pmatrix}\neq I$.

**c) Falsa.** Con $A=B=I_2$: $\det(A+B)=\det(2I)=4$, pero $\det A+\det B=2$.

**d) Verdadera.** Multiplicando a izquierda por $A^{-1}$: $A^{-1}AB=A^{-1}AC\Rightarrow IB=IC\Rightarrow B=C$.

**e) Verdadera.** $(AA^t)^t=(A^t)^tA^t=AA^t$.

## B4. Ecuación matricial

Hallá la matriz $X$ que cumple $AX+B=C$, siendo
$$A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad B=\begin{pmatrix}1&0\\3&2\end{pmatrix},\qquad C=\begin{pmatrix}5&3\\4&6\end{pmatrix}$$

*Repasá:* sección 3 (tabla de ecuaciones matriciales).

### Resolución

Despejamos: $AX=C-B\Rightarrow X=A^{-1}(C-B)$, **multiplicando por $A^{-1}$ a izquierda**.

$\det A=2\cdot1-1\cdot1=1\neq0$, así que $A$ es inversible y
$$A^{-1}=\frac11\begin{pmatrix}1&-1\\-1&2\end{pmatrix}$$

$$C-B=\begin{pmatrix}4&3\\1&4\end{pmatrix}\qquad X=\begin{pmatrix}1&-1\\-1&2\end{pmatrix}\begin{pmatrix}4&3\\1&4\end{pmatrix}=\boxed{\begin{pmatrix}3&-1\\-2&5\end{pmatrix}}$$

Verificación: $AX+B=\begin{pmatrix}4&3\\1&4\end{pmatrix}+\begin{pmatrix}1&0\\3&2\end{pmatrix}=\begin{pmatrix}5&3\\4&6\end{pmatrix}=C$ ✓.

## B5. Matriz inversa

Sea
$$M=\begin{pmatrix}1&2&0\\0&1&1\\2&0&3\end{pmatrix}$$

a) Calculá $\det M$. ¿Es inversible?

b) Hallá $M^{-1}$ por el método de Gauss-Jordan.

c) Verificá el resultado calculando $M^{-1}$ con la adjunta.

*Repasá:* secciones 3 y 4.

### Resolución

**a)** Desarrollando por la primera fila:
$$\det M=1\,(1\cdot3-1\cdot0)-2\,(0\cdot3-1\cdot2)+0=3+4=\boxed{7}\neq0$$
Es inversible.

**b)** Armamos $[\,M\mid I\,]$:

$$\left(\begin{array}{ccc|ccc}1&2&0&1&0&0\\0&1&1&0&1&0\\2&0&3&0&0&1\end{array}\right)$$

- $F_3\leftarrow F_3-2F_1$: $(0,-4,3\mid-2,0,1)$.
- $F_3\leftarrow F_3+4F_2$: $(0,0,7\mid-2,4,1)$.
- $F_3\leftarrow\frac17F_3$: $(0,0,1\mid-\frac27,\frac47,\frac17)$.
- $F_2\leftarrow F_2-F_3$: $(0,1,0\mid\frac27,\frac37,-\frac17)$.
- $F_1\leftarrow F_1-2F_2$: $(1,0,-2\mid1,-2,0)$, y luego $F_1\leftarrow F_1+2F_3$: $(1,0,0\mid\frac37,-\frac67,\frac27)$.

$$\boxed{M^{-1}=\frac17\begin{pmatrix}3&-6&2\\2&3&-1\\-2&4&1\end{pmatrix}}$$

**c)** Cofactores $C_{ij}=(-1)^{i+j}M_{ij}$:

$$C=\begin{pmatrix}3&2&-2\\-6&3&4\\2&-1&1\end{pmatrix}\qquad \operatorname{adj}(M)=C^t=\begin{pmatrix}3&-6&2\\2&3&-1\\-2&4&1\end{pmatrix}$$

$M^{-1}=\frac{1}{7}\operatorname{adj}(M)$ coincide con lo obtenido en b) ✓.

## B6. Sistema $3\times3$: Gauss-Jordan y Cramer

Resolvé
$$\begin{cases}2x+y-z=1\\x+3y+2z=13\\x+z=4\end{cases}$$

a) Por el método de Gauss-Jordan.

b) Verificá la solución con la regla de Cramer.

*Repasá:* sección 5.

### Resolución

**a)** Matriz ampliada:
$$\left(\begin{array}{ccc|c}2&1&-1&1\\1&3&2&13\\1&0&1&4\end{array}\right)$$

- $F_1\leftrightarrow F_3$: $(1,0,1\mid4)$, $(1,3,2\mid13)$, $(2,1,-1\mid1)$.
- $F_2\leftarrow F_2-F_1$: $(0,3,1\mid9)$; $F_3\leftarrow F_3-2F_1$: $(0,1,-3\mid-7)$.
- $F_2\leftrightarrow F_3$: $(0,1,-3\mid-7)$ y $(0,3,1\mid9)$.
- $F_3\leftarrow F_3-3F_2$: $(0,0,10\mid30)$, y luego $F_3\leftarrow\frac1{10}F_3$: $(0,0,1\mid3)$.
- $F_2\leftarrow F_2+3F_3$: $(0,1,0\mid2)$; $F_1\leftarrow F_1-F_3$: $(1,0,0\mid1)$.

$$\boxed{(x,y,z)=(1,2,3)}\qquad\text{(SCD: } \operatorname{rg}(A)=\operatorname{rg}(A|B)=3\text{)}$$

**b)** $\det A=2(3-0)-1(1-2)+(-1)(0-3)=6+1+3=10$.

$$x=\frac{\begin{vmatrix}1&1&-1\\13&3&2\\4&0&1\end{vmatrix}}{10}=\frac{10}{10}=1,\quad y=\frac{\begin{vmatrix}2&1&-1\\1&13&2\\1&4&1\end{vmatrix}}{10}=\frac{20}{10}=2,\quad z=\frac{\begin{vmatrix}2&1&1\\1&3&13\\1&0&4\end{vmatrix}}{10}=\frac{30}{10}=3$$

Coincide con a) ✓.

## B7. Sistema con parámetro

Sea el sistema
$$\begin{cases}x+y+z=1\\x+2y+kz=1\\x+4y+k^2z=k\end{cases}$$

a) Calculá el determinante de la matriz de coeficientes y factorizalo.

b) Discutí el sistema según $k$ (SCD, SCI o SI).

c) Resolvelo para $k=3$ y para $k=1$.

*Repasá:* secciones 4 y 5 (sistemas con parámetro).

### Resolución

**a)** Es un determinante tipo Vandermonde:
$$\det A=\begin{vmatrix}1&1&1\\1&2&k\\1&4&k^2\end{vmatrix}=1(2k^2-4k)-1(k^2-k)+1(4-2)=k^2-3k+2=\boxed{(k-1)(k-2)}$$

**b)**

- **$k\neq1$ y $k\neq2$:** $\det A\neq0\Rightarrow$ **SCD**.
- **$k=1$:** el sistema es $x+y+z=1,\ x+2y+z=1,\ x+4y+z=1$. Restando, $y=0$ y $x+z=1$. Las matrices $A$ y $[A|B]$ tienen rango $2<3$: **SCI** (1 parámetro).
- **$k=2$:** $x+y+z=1,\ x+2y+2z=1,\ x+4y+4z=2$. De las dos primeras, $y+z=0$ y $x=1$. La tercera pide $4(y+z)=1$, o sea $0=1$: $\operatorname{rg}(A)=2<\operatorname{rg}(A|B)=3$: **SI**.

**c)**

- Para $k=3$: $x+y+z=1,\ x+2y+3z=1,\ x+4y+9z=3$. Restando, $y+2z=0$ y $3y+8z=2$, de donde $z=1$, $y=-2$, $x=2$:
$$\boxed{(x,y,z)=(2,-2,1)}$$
- Para $k=1$: con $y=0$ y $x+z=1$, llamando $z=t$:
$$\boxed{(x,y,z)=(1-t,\,0,\,t),\quad t\in\mathbb{R}}$$

## B8. Sistema homogéneo con parámetro

Hallá los valores de $a\in\mathbb{R}$ para los cuales el sistema
$$\begin{cases}x+y+az=0\\x+ay+z=0\\ax+y+z=0\end{cases}$$
tiene soluciones **no triviales**, y encontralas.

*Repasá:* sección 5 (homogéneos).

### Resolución

Un sistema homogéneo cuadrado tiene soluciones no triviales $\iff\det A=0$.

$$\det A=\begin{vmatrix}1&1&a\\1&a&1\\a&1&1\end{vmatrix}=-(a-1)^2(a+2)$$

Entonces $\det A=0\iff a=1$ ó $a=-2$.

- **$a=1$:** las tres ecuaciones son $x+y+z=0$. Rango $1$, SCI con 2 parámetros:
$$(x,y,z)=(-s-t,\ s,\ t),\quad s,t\in\mathbb{R}$$
(un plano que pasa por el origen).
- **$a=-2$:** $x+y-2z=0$, $x-2y+z=0$, $-2x+y+z=0$. Restando las dos primeras, $3y-3z=0\Rightarrow y=z$ y entonces $x=z$. Rango $2$, SCI con 1 parámetro:
$$(x,y,z)=t(1,1,1),\quad t\in\mathbb{R}$$
- **Cualquier otro $a$:** $\det A\neq0\Rightarrow$ solo la solución trivial.

## B9. Propiedades del determinante

Sea $A\in\mathbb{R}^{3\times3}$ con $\det A=4$. Calculá, sin conocer $A$:

a) $\det(2A)$

b) $\det(A^{-1})$

c) $\det(A^tA)$

d) $\det(-A)$

e) $\det(2A^{-1})$

f) $\det B$, donde $B$ se obtiene de $A$ intercambiando las filas $1$ y $3$ y multiplicando la fila $2$ por $3$.

*Repasá:* sección 4.

### Resolución

Como $n=3$:

a) $\det(2A)=2^3\det A=\boxed{32}$

b) $\det(A^{-1})=\dfrac1{\det A}=\boxed{\dfrac14}$

c) $\det(A^tA)=\det(A^t)\det A=(\det A)^2=\boxed{16}$

d) $\det(-A)=(-1)^3\det A=\boxed{-4}$

e) $\det(2A^{-1})=2^3\det(A^{-1})=8\cdot\frac14=\boxed{2}$

f) Intercambiar dos filas multiplica por $-1$, y multiplicar una fila por $3$ multiplica por $3$: $\det B=(-1)\cdot3\cdot4=\boxed{-12}$

---

# Parte C — Coordenadas y vectores

## C1. De cilíndricas a cartesianas y esféricas

El punto $P$ tiene coordenadas cilíndricas $\left(2,\frac{3\pi}{4},-2\right)$. Expresalo en coordenadas cartesianas y en coordenadas esféricas (convención del Cuadernillo: $\rho$, $\theta$ cenital, $\varphi$ azimutal).

*Repasá:* sección 6.

### Resolución

**Cartesianas:**
$$x=2\cos\tfrac{3\pi}{4}=-\sqrt2,\qquad y=2\sin\tfrac{3\pi}{4}=\sqrt2,\qquad z=-2\quad\Rightarrow\quad\boxed{P=(-\sqrt2,\ \sqrt2,\ -2)}$$

**Esféricas:**
$$\rho=\sqrt{x^2+y^2+z^2}=\sqrt{2+2+4}=2\sqrt2$$
$$\theta=\arccos\frac z\rho=\arccos\left(-\frac{2}{2\sqrt2}\right)=\arccos\left(-\frac{\sqrt2}{2}\right)=\frac{3\pi}{4}$$
$$\varphi=\frac{3\pi}{4}\quad(\text{el mismo ángulo azimutal que en cilíndricas})$$

$$\boxed{P=\left(2\sqrt2,\ \tfrac{3\pi}{4},\ \tfrac{3\pi}{4}\right)}$$

## C2. De cartesianas a esféricas y cilíndricas

Dado $Q=(1,-1,\sqrt2)$, hallá sus coordenadas esféricas y cilíndricas. Comprobá el resultado volviendo a cartesianas.

*Repasá:* sección 6.

### Resolución

**Esféricas:**
$$\rho=\sqrt{1+1+2}=2,\qquad\theta=\arccos\frac{\sqrt2}{2}=\frac\pi4$$
$(x,y)=(1,-1)$ está en el 4.º cuadrante, por lo que $\varphi=\frac{7\pi}{4}$.

$$\boxed{Q=\left(2,\ \tfrac\pi4,\ \tfrac{7\pi}4\right)_{esf}}$$

**Cilíndricas:** $\rho_{cil}=\sqrt{1+1}=\sqrt2$, mismo azimut y misma altura:

$$\boxed{Q=\left(\sqrt2,\ \tfrac{7\pi}4,\ \sqrt2\right)_{cil}}$$

**Comprobación:**
$$x=2\sin\tfrac\pi4\cos\tfrac{7\pi}4=2\cdot\tfrac{\sqrt2}2\cdot\tfrac{\sqrt2}2=1,\quad y=2\cdot\tfrac{\sqrt2}2\cdot\left(-\tfrac{\sqrt2}2\right)=-1,\quad z=2\cos\tfrac\pi4=\sqrt2\ ✓$$

## C3. Ecuaciones en polares

Escribí en coordenadas polares las siguientes ecuaciones dadas en cartesianas:

a) $x^2+y^2=4y$

b) $x+y=2$

*Repasá:* sección 6.

### Resolución

Se reemplaza $x=\rho\cos\theta$, $y=\rho\sin\theta$ y $x^2+y^2=\rho^2$.

**a)**
$$\rho^2=4\rho\sin\theta\ \Longrightarrow\ \boxed{\rho=4\sin\theta}$$
(se simplificó $\rho\neq0$; el origen se recupera con $\theta=0$). Es la circunferencia de centro $(0,2)$ y radio $2$.

**b)**
$$\rho\cos\theta+\rho\sin\theta=2\ \Longrightarrow\ \boxed{\rho=\frac{2}{\cos\theta+\sin\theta}}$$

## C4. Proyección ortogonal y descomposición

Sean $u=(3,1,2)$ y $v=(1,-2,2)$.

a) Calculá $\operatorname{proy}_v(u)$ y $\operatorname{comp}_v(u)$.

b) Descomponé $u=u_\parallel+u_\perp$ con $u_\parallel\parallel v$ y $u_\perp\perp v$.

c) Verificá que $u_\perp\cdot v=0$.

*Repasá:* sección 8 (proyección ortogonal).

### Resolución

$u\cdot v=3-2+4=5$ y $\|v\|^2=1+4+4=9$.

**a)**
$$\operatorname{proy}_v(u)=\frac{5}{9}(1,-2,2)=\boxed{\left(\tfrac59,-\tfrac{10}9,\tfrac{10}9\right)}\qquad\operatorname{comp}_v(u)=\frac{u\cdot v}{\|v\|}=\boxed{\tfrac53}$$

**b)**
$$u_\parallel=\left(\tfrac59,-\tfrac{10}9,\tfrac{10}9\right)\qquad u_\perp=u-u_\parallel=\left(3-\tfrac59,\ 1+\tfrac{10}9,\ 2-\tfrac{10}9\right)=\boxed{\left(\tfrac{22}9,\tfrac{19}9,\tfrac89\right)}$$

**c)**
$$u_\perp\cdot v=\tfrac{22}9-\tfrac{38}9+\tfrac{16}9=0\ ✓$$

## C5. Ángulo con un parámetro

Sean $v=(1,1,0)$ y $w=(1,k,1)$ con $k\in\mathbb{R}$. Hallá todos los valores de $k$ para los que el ángulo entre $v$ y $w$ es $\frac\pi3$.

*Repasá:* sección 8 (ángulo y última fila de "Construir un vector con condiciones").

### Resolución

$$\cos\frac\pi3=\frac12=\frac{v\cdot w}{\|v\|\,\|w\|}=\frac{1+k}{\sqrt2\,\sqrt{k^2+2}}$$

Elevando al cuadrado ($4(1+k)^2=2(k^2+2)$):
$$4k^2+8k+4=2k^2+4\ \Longrightarrow\ 2k^2+8k=0\ \Longrightarrow\ k=0\ \text{ ó }\ k=-4$$

**Hay que verificar el signo**, porque al elevar al cuadrado aparece una solución espuria. Debe ser $v\cdot w=1+k>0$:

- $k=0$: $\cos\theta=\frac{1}{\sqrt2\sqrt2}=\frac12$ ✓.
- $k=-4$: $\cos\theta=\frac{-3}{\sqrt2\sqrt{18}}=-\frac12$, es decir $\theta=\frac{2\pi}3$ ✗.

$$\boxed{k=0}$$

## C6. Norma a partir de condiciones geométricas

Sean $u,v\in\mathbb{R}^n$ tales que el ángulo entre ellos es $\frac\pi3$, $\|v\|=4$ y $(u-v)\perp u$. Calculá $\|u\|$.

*Repasá:* sección 8 (propiedades del producto escalar).

### Resolución

$(u-v)\perp u\Rightarrow(u-v)\cdot u=0\Rightarrow\|u\|^2=u\cdot v$.

Y $u\cdot v=\|u\|\,\|v\|\cos\frac\pi3=\|u\|\cdot4\cdot\frac12=2\|u\|$.

Entonces $\|u\|^2=2\|u\|$. Como $u\neq0$ (el ángulo está definido):
$$\boxed{\|u\|=2}$$

## C7. Triángulo en el espacio

Sea el triángulo de vértices $A=(1,0,2)$, $B=(3,1,0)$ y $C=(2,3,1)$.

a) Calculá la longitud de los lados y el perímetro.

b) ¿Es un triángulo rectángulo? Justificá.

c) Calculá el área.

d) Calculá el ángulo en el vértice $A$.

*Repasá:* secciones 7, 8 y 9.

### Resolución

$\overrightarrow{AB}=(2,1,-2)$, $\overrightarrow{AC}=(1,3,-1)$, $\overrightarrow{BC}=(-1,2,1)$.

**a)**
$$AB=\sqrt{4+1+4}=3,\qquad AC=\sqrt{1+9+1}=\sqrt{11},\qquad BC=\sqrt{1+4+1}=\sqrt6$$
$$\boxed{\text{Perímetro}=3+\sqrt{11}+\sqrt6}$$

**b)** Los productos escalares entre pares de lados que salen de cada vértice:

- En $A$: $\overrightarrow{AB}\cdot\overrightarrow{AC}=2+3+2=7\neq0$.
- En $B$: $\overrightarrow{BA}\cdot\overrightarrow{BC}=(-2,-1,2)\cdot(-1,2,1)=2-2+2=2\neq0$.
- En $C$: $\overrightarrow{CA}\cdot\overrightarrow{CB}=(-1,-3,1)\cdot(1,-2,-1)=-1+6-1=4\neq0$.

Ninguno es cero: **no es rectángulo**. (Con Pitágoras: lado mayor $\sqrt{11}$, $3^2+(\sqrt6)^2=15\neq11$.) Como los tres productos son positivos, los tres ángulos son **agudos**.

**c)**
$$\overrightarrow{AB}\times\overrightarrow{AC}=(1\cdot(-1)-(-2)\cdot3,\ (-2)\cdot1-2\cdot(-1),\ 2\cdot3-1\cdot1)=(5,0,5)$$
$$\boxed{\text{Área}=\tfrac12\|(5,0,5)\|=\tfrac12\cdot5\sqrt2=\tfrac{5\sqrt2}2}$$

**d)**
$$\cos\hat A=\frac{\overrightarrow{AB}\cdot\overrightarrow{AC}}{\|\overrightarrow{AB}\|\,\|\overrightarrow{AC}\|}=\frac{7}{3\sqrt{11}}\ \Longrightarrow\ \boxed{\hat A=\arccos\frac{7}{3\sqrt{11}}\approx45{,}3^\circ}$$

## C8. Tetraedro y coplanaridad

Con los puntos $A=(1,0,2)$, $B=(3,1,0)$, $C=(2,3,1)$ del ejercicio anterior y $D=(1,1,5)$:

a) Calculá el volumen del tetraedro $ABCD$.

b) Calculá la altura del tetraedro trazada desde $D$ sobre la cara $ABC$.

c) Hallá $z$ para que el punto $D'=(1,1,z)$ sea **coplanar** con $A$, $B$ y $C$.

*Repasá:* secciones 9 y 10.

### Resolución

$\overrightarrow{AB}=(2,1,-2)$, $\overrightarrow{AC}=(1,3,-1)$, $\overrightarrow{AD}=(0,1,3)$.

**a)**
$$[\overrightarrow{AB},\overrightarrow{AC},\overrightarrow{AD}]=\begin{vmatrix}2&1&-2\\1&3&-1\\0&1&3\end{vmatrix}=2(9+1)-1(3-0)+(-2)(1-0)=20-3-2=15$$
$$\boxed{V=\tfrac16\cdot15=\tfrac52}$$

**b)** Con $\overrightarrow{AB}\times\overrightarrow{AC}=(5,0,5)$ y $\|\overrightarrow{AB}\times\overrightarrow{AC}\|=5\sqrt2$:
$$h=\frac{|[\overrightarrow{AB},\overrightarrow{AC},\overrightarrow{AD}]|}{\|\overrightarrow{AB}\times\overrightarrow{AC}\|}=\frac{15}{5\sqrt2}=\boxed{\frac{3\sqrt2}2}$$

(Control: $V=\frac13\cdot\text{área base}\cdot h=\frac13\cdot\frac{5\sqrt2}2\cdot\frac{3\sqrt2}2=\frac52$ ✓.)

**c)** $\overrightarrow{AD'}=(0,1,z-2)$. Coplanares $\iff[\overrightarrow{AB},\overrightarrow{AC},\overrightarrow{AD'}]=0$:
$$\begin{vmatrix}2&1&-2\\1&3&-1\\0&1&z-2\end{vmatrix}=2\big(3(z-2)+1\big)-1(z-2)-2=5z-10=0\ \Longrightarrow\ \boxed{z=2}$$
(Con $z=5$ da $15$, como en a) ✓.)

---

# Parte D — Integradores

## D1. Matrices, determinantes y vectores (25 pts)

Sean $u=(1,2,0)$, $v=(0,1,k)$ y $w=(k,0,1)$ con $k\in\mathbb{R}$, y $M$ la matriz cuyas filas son $u$, $v$ y $w$.

a) (7 pts) Calculá $\det M$ en función de $k$.

b) (6 pts) ¿Para qué valores de $k$ son $u$, $v$, $w$ linealmente dependientes (coplanares)? ¿Para qué $k$ es $M$ inversible?

c) (5 pts) Para $k=1$, calculá el volumen del paralelepípedo determinado por $u$, $v$, $w$.

d) (7 pts) Para $k=1$, escribí $b=(3,3,0)$ como combinación lineal $\alpha u+\beta v+\gamma w$.

*Repasá:* secciones 4, 5, 7 y 10.

### Resolución

**a)** Desarrollando por la primera fila:
$$\det M=\begin{vmatrix}1&2&0\\0&1&k\\k&0&1\end{vmatrix}=1(1-0)-2(0-k^2)+0=\boxed{2k^2+1}$$
(coincide con el producto mixto $u\cdot(v\times w)$).

**b)** $\det M=2k^2+1\geq1>0$ para todo $k\in\mathbb{R}$. Por lo tanto **no existe ningún $k$** que los haga LD o coplanares: son **siempre linealmente independientes** y $M$ es **inversible para todo $k$**.

**c)** Con $k=1$: $\det M=3$, entonces
$$V=|[u,v,w]|=\boxed{3}$$

**d)** Con $k=1$: $u=(1,2,0)$, $v=(0,1,1)$, $w=(1,0,1)$. El sistema $\alpha u+\beta v+\gamma w=b$ queda
$$\begin{cases}\alpha+\gamma=3\\2\alpha+\beta=3\\\beta+\gamma=0\end{cases}$$

El determinante de los coeficientes es $3\neq0$ (SCD). De la tercera, $\gamma=-\beta$; de la primera, $\alpha=3+\beta$; en la segunda, $6+2\beta+\beta=3\Rightarrow\beta=-1$. Entonces
$$\boxed{\alpha=2,\quad\beta=-1,\quad\gamma=1}$$
Verificación: $2(1,2,0)-(0,1,1)+(1,0,1)=(3,3,0)$ ✓.

## D2. Sistemas y producto vectorial (25 pts)

Sean $u=(1,2,-1)$ y $v=(2,1,1)$.

a) (8 pts) Planteá y resolvé por Gauss el sistema homogéneo cuyas soluciones son **todos** los vectores $x=(x_1,x_2,x_3)$ ortogonales a $u$ y a $v$. Clasificalo.

b) (5 pts) Verificá que el resultado de a) es paralelo a $u\times v$.

c) (7 pts) Hallá dos vectores de norma $1$ ortogonales a $u$ y a $v$.

d) (5 pts) Hallá el área del paralelogramo determinado por $u$ y $v$.

*Repasá:* secciones 5, 8 y 9.

### Resolución

**a)** $x\perp u$ y $x\perp v$ equivale a
$$\begin{cases}x_1+2x_2-x_3=0\\2x_1+x_2+x_3=0\end{cases}\quad\left(\begin{array}{ccc|c}1&2&-1&0\\2&1&1&0\end{array}\right)$$

$F_2\leftarrow F_2-2F_1$: $(0,-3,3\mid0)\Rightarrow x_2=x_3$. Reemplazando en la primera: $x_1=-2x_2+x_3=-x_3$.

$$\boxed{x=t(-1,1,1),\quad t\in\mathbb{R}}$$

Es un sistema **homogéneo SCI**: $\operatorname{rg}=2<3$ incógnitas, con $3-2=1$ parámetro libre. Geométricamente: los vectores ortogonales a dos vectores no paralelos de $\mathbb{R}^3$ forman una recta por el origen.

**b)**
$$u\times v=(2\cdot1-(-1)\cdot1,\ (-1)\cdot2-1\cdot1,\ 1\cdot1-2\cdot2)=(3,-3,-3)=-3\,(-1,1,1)$$
Es paralelo a la solución de a) ✓.

**c)** Con $t$ tal que $\|x\|=1$: $\|(-1,1,1)\|=\sqrt3$, entonces
$$\boxed{\pm\frac{1}{\sqrt3}(-1,1,1)=\pm\left(-\tfrac{\sqrt3}3,\tfrac{\sqrt3}3,\tfrac{\sqrt3}3\right)}$$

**d)**
$$\text{Área}=\|u\times v\|=\|(3,-3,-3)\|=\boxed{3\sqrt3}$$

## D3. Rotación: matrices y coordenadas polares (25 pts)

La matriz $R(\alpha)=\begin{pmatrix}\cos\alpha&-\sin\alpha\\\sin\alpha&\cos\alpha\end{pmatrix}$ rota un punto del plano un ángulo $\alpha$ alrededor del origen (antihorario). Sea $P$ el punto de coordenadas polares $\left(4,\frac\pi3\right)$.

a) (5 pts) Expresá $P$ en cartesianas.

b) (7 pts) Calculá $R\!\left(\frac\pi3\right)\cdot P$ (con $P$ como vector columna) y expresá el resultado en polares. ¿Qué observás?

c) (7 pts) Calculá $\det R\!\left(\frac\pi3\right)$ y $R\!\left(\frac\pi3\right)^{-1}$. Verificá que $R^{-1}=R^t$.

d) (6 pts) Sin hacer el producto, justificá que $R\!\left(\frac\pi3\right)^6=I$.

*Repasá:* secciones 2, 3, 4 y 6.

### Resolución

**a)** $P=\left(4\cos\frac\pi3,\ 4\sin\frac\pi3\right)=\boxed{(2,\ 2\sqrt3)}$.

**b)** $R\!\left(\frac\pi3\right)=\begin{pmatrix}\frac12&-\frac{\sqrt3}2\\\frac{\sqrt3}2&\frac12\end{pmatrix}$.

$$R\!\left(\tfrac\pi3\right)\begin{pmatrix}2\\2\sqrt3\end{pmatrix}=\begin{pmatrix}1-3\\\sqrt3+\sqrt3\end{pmatrix}=\begin{pmatrix}-2\\2\sqrt3\end{pmatrix}$$

En polares: $\rho=\sqrt{4+12}=4$ y, en el 2.º cuadrante, $\tan\theta=-\sqrt3\Rightarrow\theta=\frac{2\pi}3$:

$$\boxed{\left(4,\tfrac{2\pi}3\right)}$$

**Observación:** el módulo $\rho$ no cambió y el ángulo aumentó en $\frac\pi3$; la matriz rota el punto.

**c)**
$$\det R=\cos^2\alpha+\sin^2\alpha=\boxed{1}$$
$$R^{-1}=\frac{1}{1}\begin{pmatrix}\frac12&\frac{\sqrt3}2\\-\frac{\sqrt3}2&\frac12\end{pmatrix}=\boxed{\begin{pmatrix}\frac12&\frac{\sqrt3}2\\-\frac{\sqrt3}2&\frac12\end{pmatrix}}$$

Y $R^t$ es exactamente esa matriz, por lo tanto $R^{-1}=R^t$: $R$ es una **matriz ortogonal**. (Además $R^{-1}=R(-\frac\pi3)$.)

**d)** Aplicar $R\!\left(\frac\pi3\right)$ seis veces rota $6\cdot\frac\pi3=2\pi$, una vuelta completa: cada punto vuelve a su lugar, por lo que $R^6=I$.

## D4. Modelado con sistemas (25 pts)

La empresa "Computadoras S.A." fabrica tres modelos de computadoras personales: $M_1$, $M_2$ y $M_3$. Para armar una $M_1$ necesita $12$ horas de ensamblado, $2{,}5$ horas de prueba y $2$ horas de instalación de programas. Para una $M_2$: $10$, $2$ y $2$ horas, respectivamente. Para una $M_3$: $6$, $1{,}5$ y $1{,}5$ horas. Por mes dispone de $556$ horas de ensamblado, $120$ de pruebas y $103$ de instalación.

a) (8 pts) Planteá el sistema en forma matricial $AX=B$ indicando qué representa cada incógnita.

b) (10 pts) ¿Cuántas computadoras de cada modelo se pueden fabricar por mes, aprovechando todas las horas? Resolvelo por Gauss.

c) (7 pts) Clasificá el sistema y justificá por qué el resultado es único.

*Repasá:* sección 5.

### Resolución

**a)** Sean $a$, $b$, $c$ la cantidad de computadoras $M_1$, $M_2$, $M_3$ por mes.

$$\begin{cases}12a+10b+6c=556\\2{,}5a+2b+1{,}5c=120\\2a+2b+1{,}5c=103\end{cases}\qquad A=\begin{pmatrix}12&10&6\\2{,}5&2&1{,}5\\2&2&1{,}5\end{pmatrix},\ X=\begin{pmatrix}a\\b\\c\end{pmatrix},\ B=\begin{pmatrix}556\\120\\103\end{pmatrix}$$

**b)** Se simplifica: la 1.ª ecuación $/2$ y las otras dos $\times2$:
$$\begin{cases}6a+5b+3c=278\\5a+4b+3c=240\\4a+4b+3c=206\end{cases}$$

- $E_2-E_3$: $a=34$.
- Reemplazando en $E_2$: $4b+3c=240-170=70$.
- Reemplazando en $E_1$: $5b+3c=278-204=74$.
- Restando: $b=4$, y entonces $3c=70-16=54\Rightarrow c=18$.

$$\boxed{a=34,\quad b=4,\quad c=18}$$

Verificación en el sistema original: $12\cdot34+10\cdot4+6\cdot18=408+40+108=556$ ✓; $2{,}5\cdot34+2\cdot4+1{,}5\cdot18=85+8+27=120$ ✓; $2\cdot34+2\cdot4+1{,}5\cdot18=68+8+27=103$ ✓.

**c)** Es un **SCD**: $\operatorname{rg}(A)=\operatorname{rg}(A|B)=3$ (igual al número de incógnitas), por lo que la solución es única. Además las cantidades obtenidas son enteros no negativos, así que tiene sentido en el contexto.
