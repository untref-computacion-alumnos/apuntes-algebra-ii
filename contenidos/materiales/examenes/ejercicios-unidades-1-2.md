# Ejercicios de parcial — Unidades 1 y 2

Ejercicios para practicar el **primer parcial** (Unidades 1 y 2), pensados para usar junto con el [machete de fórmulas](../formulas.md). Esta versión trae **solo las consignas**; las respuestas están en [la versión resuelta](ejercicios-unidades-1-2-resuelto.md).

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

## A2. Parcial 10/06/2024 — Ejercicio 2 (20 pts)

Sean $v=(1,2,1)$ y $w=(k,0,1)$ con $k\in\mathbb{R}$.

a) Hallá $k$ para que el ángulo entre $v$ y $w$ sea $\frac{\pi}{2}$.

b) Para $k=2$, encontrá un vector $u$ tal que:

- $u$ es ortogonal a $v$.
- $u$ es ortogonal a $w$.
- $\|u\|=2$.

*Repasá:* secciones 8 y 9.

## A3. Recuperatorio 24/06/2024 — Ejercicio 1 (30 pts)

Sea $T$ el triángulo definido por los vértices $A=(1,0)$, $B=(5,0)$ y $C=(3,\sqrt3)$.

a) Expresá a los tres puntos en coordenadas polares.

b) Hallá el perímetro del triángulo $T$.

c) ¿Es rectángulo el triángulo $T$?

*Repasá:* secciones 6, 7 y 8.

## A4. Recuperatorio 24/06/2024 — Ejercicio 2 (20 pts)

Sea $v=(1,k,k-1)$ con $k\in\mathbb{R}$.

a) Hallá, si es posible, $k$ para que $v$ sea ortogonal a $u=(2,1,-1)$.

b) Para $k=1$, encontrá un vector $w$ tal que:

- $w$ es ortogonal a $u$.
- $w$ no es ortogonal a $v$.
- $\|w\|=1$.

*Repasá:* sección 8 (en particular "Construir un vector con condiciones").

## A5. Parcial 04/11/2024 — Ejercicio 1 (25 pts)

Los puntos $A=\left(5,\frac{\pi}{3}\right)$ y $B=\left(5,\frac{5\pi}{3}\right)$ están expresados en coordenadas polares.

a) Graficá los puntos $A$ y $B$.

b) Calculá la distancia entre los puntos $A$ y $B$.

c) Determiná las coordenadas cartesianas de un punto $C$ que cumpla las siguientes condiciones:

- i. La distancia de $C$ al punto $A$ es el doble de la distancia entre $A$ y $B$.
- ii. $C$ pertenece a la recta que pasa por $A$ y por $B$.

d) ¿Es única la ubicación de $C$? Justificá la respuesta.

*Repasá:* secciones 6 y 7.

## A6. Parcial 04/11/2024 — Ejercicio 2 (15 pts)

Considerá el vector $v=(4,2,-1)$. Encontrá, si es posible, dos vectores $w_1$ y $w_2$ que sean ortogonales entre sí y que también sean ortogonales a $v$.

*Repasá:* secciones 8 y 9.

## A7. Recuperatorio 11/11/2024 — Ejercicio 1 (20 pts)

Sea el triángulo $KLM$ con vértices en $K=(1,2)$, $L=(4,5)$ y $M=(1,5)$.

a) Determiná las coordenadas polares de los vértices del triángulo.

b) Calculá la longitud de cada lado del triángulo.

c) Verificá si el triángulo $KLM$ es un triángulo rectángulo.

*Repasá:* secciones 6, 7 y 8.

## A8. Recuperatorio 11/11/2024 — Ejercicio 2 (30 pts)

Sea el vector $a=(2,k,k+3)$ con $k\in\mathbb{R}$.

a) Encontrá, si existe, un valor de $k$ tal que el vector $a$ sea ortogonal a $b=(3,-1,2)$.

b) Si $k=4$, encontrá, si es posible, un vector $c$ tal que:

- $c$ es ortogonal a $b$.
- $c$ no es ortogonal a $a$.
- $\|c\|=2$.

*Repasá:* sección 8.

---

# Parte B — Matrices, sistemas y determinantes

## B1. Operaciones con matrices

Sean
$$A=\begin{pmatrix}1&2\\0&-1\\3&1\end{pmatrix},\qquad B=\begin{pmatrix}2&0&1\\1&-1&4\end{pmatrix},\qquad C=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}$$

a) Calculá $2C-A$.

b) Calculá $AB$ y $BA$. ¿Son iguales? ¿Por qué?

c) Verificá que $(AB)^t=B^tA^t$.

*Repasá:* sección 2.

## B2. Simétrica más antisimétrica

Sea
$$Q=\begin{pmatrix}1&4&-2\\0&3&6\\2&-2&5\end{pmatrix}$$

a) Hallá una matriz simétrica $S$ y una antisimétrica $K$ tales que $Q=S+K$.

b) Verificá que $S^t=S$, que $K^t=-K$ y que $S+K=Q$.

*Repasá:* secciones 1 y 2.

## B3. Verdadero o falso

Decidí si cada afirmación es verdadera o falsa para $A,B,C\in\mathbb{R}^{n\times n}$. Si es falsa, dá un **contraejemplo** ($n=2$); si es verdadera, justificá.

a) $AB=AC\Rightarrow B=C$.

b) $(A+B)^2=A^2+2AB+B^2$.

c) $\det(A+B)=\det A+\det B$.

d) Si $A$ es inversible y $AB=AC$, entonces $B=C$.

e) $AA^t$ es simétrica.

*Repasá:* secciones 2, 3 y 4.

## B4. Ecuación matricial

Hallá la matriz $X$ que cumple $AX+B=C$, siendo
$$A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad B=\begin{pmatrix}1&0\\3&2\end{pmatrix},\qquad C=\begin{pmatrix}5&3\\4&6\end{pmatrix}$$

*Repasá:* sección 3 (tabla de ecuaciones matriciales).

## B5. Matriz inversa

Sea
$$M=\begin{pmatrix}1&2&0\\0&1&1\\2&0&3\end{pmatrix}$$

a) Calculá $\det M$. ¿Es inversible?

b) Hallá $M^{-1}$ por el método de Gauss-Jordan.

c) Verificá el resultado calculando $M^{-1}$ con la adjunta.

*Repasá:* secciones 3 y 4.

## B6. Sistema $3\times3$: Gauss-Jordan y Cramer

Resolvé
$$\begin{cases}2x+y-z=1\\x+3y+2z=13\\x+z=4\end{cases}$$

a) Por el método de Gauss-Jordan.

b) Verificá la solución con la regla de Cramer.

*Repasá:* sección 5.

## B7. Sistema con parámetro

Sea el sistema
$$\begin{cases}x+y+z=1\\x+2y+kz=1\\x+4y+k^2z=k\end{cases}$$

a) Calculá el determinante de la matriz de coeficientes y factorizalo.

b) Discutí el sistema según $k$ (SCD, SCI o SI).

c) Resolvelo para $k=3$ y para $k=1$.

*Repasá:* secciones 4 y 5 (sistemas con parámetro).

## B8. Sistema homogéneo con parámetro

Hallá los valores de $a\in\mathbb{R}$ para los cuales el sistema
$$\begin{cases}x+y+az=0\\x+ay+z=0\\ax+y+z=0\end{cases}$$
tiene soluciones **no triviales**, y encontralas.

*Repasá:* sección 5 (homogéneos).

## B9. Propiedades del determinante

Sea $A\in\mathbb{R}^{3\times3}$ con $\det A=4$. Calculá, sin conocer $A$:

a) $\det(2A)$

b) $\det(A^{-1})$

c) $\det(A^tA)$

d) $\det(-A)$

e) $\det(2A^{-1})$

f) $\det B$, donde $B$ se obtiene de $A$ intercambiando las filas $1$ y $3$ y multiplicando la fila $2$ por $3$.

*Repasá:* sección 4.

---

# Parte C — Coordenadas y vectores

## C1. De cilíndricas a cartesianas y esféricas

El punto $P$ tiene coordenadas cilíndricas $\left(2,\frac{3\pi}{4},-2\right)$. Expresalo en coordenadas cartesianas y en coordenadas esféricas (convención del Cuadernillo: $\rho$, $\theta$ cenital, $\varphi$ azimutal).

*Repasá:* sección 6.

## C2. De cartesianas a esféricas y cilíndricas

Dado $Q=(1,-1,\sqrt2)$, hallá sus coordenadas esféricas y cilíndricas. Comprobá el resultado volviendo a cartesianas.

*Repasá:* sección 6.

## C3. Ecuaciones en polares

Escribí en coordenadas polares las siguientes ecuaciones dadas en cartesianas:

a) $x^2+y^2=4y$

b) $x+y=2$

*Repasá:* sección 6.

## C4. Proyección ortogonal y descomposición

Sean $u=(3,1,2)$ y $v=(1,-2,2)$.

a) Calculá $\operatorname{proy}_v(u)$ y $\operatorname{comp}_v(u)$.

b) Descomponé $u=u_\parallel+u_\perp$ con $u_\parallel\parallel v$ y $u_\perp\perp v$.

c) Verificá que $u_\perp\cdot v=0$.

*Repasá:* sección 8 (proyección ortogonal).

## C5. Ángulo con un parámetro

Sean $v=(1,1,0)$ y $w=(1,k,1)$ con $k\in\mathbb{R}$. Hallá todos los valores de $k$ para los que el ángulo entre $v$ y $w$ es $\frac\pi3$.

*Repasá:* sección 8 (ángulo y última fila de "Construir un vector con condiciones").

## C6. Norma a partir de condiciones geométricas

Sean $u,v\in\mathbb{R}^n$ tales que el ángulo entre ellos es $\frac\pi3$, $\|v\|=4$ y $(u-v)\perp u$. Calculá $\|u\|$.

*Repasá:* sección 8 (propiedades del producto escalar).

## C7. Triángulo en el espacio

Sea el triángulo de vértices $A=(1,0,2)$, $B=(3,1,0)$ y $C=(2,3,1)$.

a) Calculá la longitud de los lados y el perímetro.

b) ¿Es un triángulo rectángulo? Justificá.

c) Calculá el área.

d) Calculá el ángulo en el vértice $A$.

*Repasá:* secciones 7, 8 y 9.

## C8. Tetraedro y coplanaridad

Con los puntos $A=(1,0,2)$, $B=(3,1,0)$, $C=(2,3,1)$ del ejercicio anterior y $D=(1,1,5)$:

a) Calculá el volumen del tetraedro $ABCD$.

b) Calculá la altura del tetraedro trazada desde $D$ sobre la cara $ABC$.

c) Hallá $z$ para que el punto $D'=(1,1,z)$ sea **coplanar** con $A$, $B$ y $C$.

*Repasá:* secciones 9 y 10.

---

# Parte D — Integradores

## D1. Matrices, determinantes y vectores (25 pts)

Sean $u=(1,2,0)$, $v=(0,1,k)$ y $w=(k,0,1)$ con $k\in\mathbb{R}$, y $M$ la matriz cuyas filas son $u$, $v$ y $w$.

a) (7 pts) Calculá $\det M$ en función de $k$.

b) (6 pts) ¿Para qué valores de $k$ son $u$, $v$, $w$ linealmente dependientes (coplanares)? ¿Para qué $k$ es $M$ inversible?

c) (5 pts) Para $k=1$, calculá el volumen del paralelepípedo determinado por $u$, $v$, $w$.

d) (7 pts) Para $k=1$, escribí $b=(3,3,0)$ como combinación lineal $\alpha u+\beta v+\gamma w$.

*Repasá:* secciones 4, 5, 7 y 10.

## D2. Sistemas y producto vectorial (25 pts)

Sean $u=(1,2,-1)$ y $v=(2,1,1)$.

a) (8 pts) Planteá y resolvé por Gauss el sistema homogéneo cuyas soluciones son **todos** los vectores $x=(x_1,x_2,x_3)$ ortogonales a $u$ y a $v$. Clasificalo.

b) (5 pts) Verificá que el resultado de a) es paralelo a $u\times v$.

c) (7 pts) Hallá dos vectores de norma $1$ ortogonales a $u$ y a $v$.

d) (5 pts) Hallá el área del paralelogramo determinado por $u$ y $v$.

*Repasá:* secciones 5, 8 y 9.

## D3. Rotación: matrices y coordenadas polares (25 pts)

La matriz $R(\alpha)=\begin{pmatrix}\cos\alpha&-\sin\alpha\\\sin\alpha&\cos\alpha\end{pmatrix}$ rota un punto del plano un ángulo $\alpha$ alrededor del origen (antihorario). Sea $P$ el punto de coordenadas polares $\left(4,\frac\pi3\right)$.

a) (5 pts) Expresá $P$ en cartesianas.

b) (7 pts) Calculá $R\!\left(\frac\pi3\right)\cdot P$ (con $P$ como vector columna) y expresá el resultado en polares. ¿Qué observás?

c) (7 pts) Calculá $\det R\!\left(\frac\pi3\right)$ y $R\!\left(\frac\pi3\right)^{-1}$. Verificá que $R^{-1}=R^t$.

d) (6 pts) Sin hacer el producto, justificá que $R\!\left(\frac\pi3\right)^6=I$.

*Repasá:* secciones 2, 3, 4 y 6.

## D4. Modelado con sistemas (25 pts)

La empresa "Computadoras S.A." fabrica tres modelos de computadoras personales: $M_1$, $M_2$ y $M_3$. Para armar una $M_1$ necesita $12$ horas de ensamblado, $2{,}5$ horas de prueba y $2$ horas de instalación de programas. Para una $M_2$: $10$, $2$ y $2$ horas, respectivamente. Para una $M_3$: $6$, $1{,}5$ y $1{,}5$ horas. Por mes dispone de $556$ horas de ensamblado, $120$ de pruebas y $103$ de instalación.

a) (8 pts) Planteá el sistema en forma matricial $AX=B$ indicando qué representa cada incógnita.

b) (10 pts) ¿Cuántas computadoras de cada modelo se pueden fabricar por mes, aprovechando todas las horas? Resolvelo por Gauss.

c) (7 pts) Clasificá el sistema y justificá por qué el resultado es único.

*Repasá:* sección 5.

