# Fórmulas (machete) — Unidades 1 y 2

> Machete para practicar el **primer parcial** (Unidad 1: Matrices, sistemas y determinantes · Unidad 2: Vectores y sistemas de coordenadas).
> Cada bloque trae la fórmula y **cuándo usarla**. Al final hay una tabla "si piden X, usá Y".

:::{note} Alcance
El cronograma del Cuadernillo asigna **Unidades 1–2 al primer parcial** y **Unidades 3–4 al segundo** (rectas y planos, cónicas y cuádricas). Este machete cubre solo las Unidades 1 y 2, que es lo que figura en el temario. Los ejercicios de rectas, planos y cónicas de los parciales anteriores quedaron fuera de [los ejercicios](examenes/ejercicios-unidades-1-2.md).
:::

---

# Unidad 1 — Matrices, sistemas y determinantes

## 1. Tipos de matrices

| Tipo | Definición | Ejemplo / nota |
|---|---|---|
| Matriz $m\times n$ | $A=[a_{ij}]$, $m$ filas y $n$ columnas | $A\in\mathbb{R}^{m\times n}$ |
| Cuadrada | $m=n$ | solo ellas tienen determinante e inversa |
| Nula $N$ | todos los elementos son $0$ | $A+N=A$ |
| Identidad $I$ | $1$ en la diagonal, $0$ fuera | $AI=IA=A$ |
| Diagonal | $a_{ij}=0$ si $i\neq j$ | |
| Triangular sup./inf. | ceros debajo / encima de la diagonal | $\det$ = producto de la diagonal |
| Traspuesta $A^t$ | $(A^t)_{ij}=a_{ji}$ (filas ↔ columnas) | $A\in\mathbb{R}^{m\times n}\Rightarrow A^t\in\mathbb{R}^{n\times m}$ |
| Simétrica | $A^t=A$ | $a_{ij}=a_{ji}$ |
| Antisimétrica | $A^t=-A$ | diagonal toda en $0$; $a_{ij}=-a_{ji}$ |
| Ortogonal | $A^t=A^{-1}$ | |
| Idempotente | $A^2=A$ | |
| Nilpotente | $A^n=N$ para algún $n$ | |
| Inversible (no singular) | existe $A^{-1}$ con $AA^{-1}=A^{-1}A=I$ | $\iff\det A\neq0$ |
| Singular | no tiene inversa | $\iff\det A=0$ |
| Igualdad | $A=B\iff$ mismo tamaño y $a_{ij}=b_{ij}$ $\forall i,j$ | sirve para plantear ecuaciones con incógnitas |

**Cuándo usarlo:** cuando piden *clasificar* una matriz, demostrar que es simétrica/idempotente/etc., o igualar matrices para despejar parámetros.

## 2. Operaciones y propiedades

- **Suma / resta:** elemento a elemento; solo si tienen **el mismo tamaño**.
- **Producto por escalar:** $(\lambda A)_{ij}=\lambda a_{ij}$.
- **Producto** $A\in\mathbb{R}^{m\times n}$, $B\in\mathbb{R}^{n\times p}$: $AB\in\mathbb{R}^{m\times p}$ y
  $$(AB)_{ij}=\sum_{l=1}^{n}a_{il}\,b_{lj}\quad(\text{fila } i \text{ de } A\ \cdot\ \text{columna } j \text{ de } B)$$
  Solo se puede si **columnas de $A$ = filas de $B$**.

| Propiedad | ¿Vale? |
|---|---|
| $AB=BA$ | **No en general** (no es conmutativo) |
| $AB=N\Rightarrow A=N$ ó $B=N$ | **No** (hay divisores de cero) |
| $AB=AC\Rightarrow B=C$ | **No**, salvo que $A$ sea inversible |
| $(A+B)^2=A^2+2AB+B^2$ | **No** (solo si $AB=BA$) |
| $(A^t)^t=A$, $(A+B)^t=A^t+B^t$, $(\lambda A)^t=\lambda A^t$ | Sí |
| $(AB)^t=B^tA^t$ | Sí (**se invierte el orden**) |
| $(AB)^{-1}=B^{-1}A^{-1}$ | Sí (**se invierte el orden**) |
| $(A^{-1})^{-1}=A$, $(A^t)^{-1}=(A^{-1})^t$ | Sí |
| $A+A^t$ es simétrica; $A-A^t$ es antisimétrica; $AA^t$ es simétrica | Sí (siempre) |

**Descomposición:** toda matriz cuadrada es suma de una simétrica y una antisimétrica:
$$A=\underbrace{\tfrac12(A+A^t)}_{\text{simétrica}}+\underbrace{\tfrac12(A-A^t)}_{\text{antisimétrica}}$$

**Cuándo usarlo:** "calculá $AB$", "decidí si es V o F", "demostrá que...". Para refutar una afirmación general, **un contraejemplo con matrices $2\times2$ alcanza**.

**Digrafos:** si $A$ es la matriz de adyacencia, $(A^r)_{ij}$ = cantidad de caminos de $r$ pasos de $i$ a $j$; $(A+A^2)_{ij}$ = caminos de a lo sumo 2 pasos.

## 3. Matriz inversa

### Método de Gauss-Jordan

Armar $[\,A\mid I\,]$ y aplicar operaciones elementales por filas hasta llegar a $[\,I\mid A^{-1}\,]$. Si en el camino aparece una **fila de ceros** en el lado izquierdo, $A$ **no es inversible**.

### Con la adjunta (útil para $2\times2$ y $3\times3$)

$$A^{-1}=\frac{1}{\det A}\operatorname{adj}(A),\qquad \operatorname{adj}(A)=C^t\quad\text{con } C_{ij}=(-1)^{i+j}M_{ij}$$

donde $M_{ij}$ es el determinante que queda al **tachar la fila $i$ y la columna $j$**.

Para $2\times2$:
$$\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}=\frac{1}{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$$

**Cuándo usarlo:** "hallá, si existe, la inversa", "resolvé la ecuación matricial". Ecuaciones matriciales (multiplicando **del mismo lado** a ambos miembros):

| Ecuación | Despeje |
|---|---|
| $AX=B$ | $X=A^{-1}B$ |
| $XA=B$ | $X=BA^{-1}$ |
| $AX+B=C$ | $X=A^{-1}(C-B)$ |

## 4. Determinantes

**$2\times2$:** $\begin{vmatrix}a&b\\c&d\end{vmatrix}=ad-bc$.

**$3\times3$ (Sarrus):** suma de los 3 productos de diagonales "hacia abajo" menos los 3 de diagonales "hacia arriba".

**Desarrollo por cofactores** (por la fila $i$, o por columna): $\displaystyle\det A=\sum_{j}a_{ij}C_{ij}$. Conviene elegir la fila/columna con más ceros.

### Efecto de las operaciones sobre el determinante

| Operación | Efecto |
|---|---|
| Intercambiar dos filas | $\det\to-\det$ |
| Multiplicar **una** fila por $\lambda$ | $\det\to\lambda\det$ |
| Sumarle a una fila un múltiplo de otra | **no cambia** |
| Dos filas iguales o proporcionales | $\det=0$ |
| Una fila (o columna) de ceros | $\det=0$ |
| Matriz triangular | producto de la diagonal |

### Propiedades (con $A,B\in\mathbb{R}^{n\times n}$)

$$\det(AB)=\det A\cdot\det B\qquad\det(A^t)=\det A\qquad\det(A^{-1})=\frac{1}{\det A}$$
$$\det(\lambda A)=\lambda^{n}\det A\qquad\det(A^k)=(\det A)^k\qquad \det(A+B)\neq\det A+\det B\ \text{(en general)}$$

**Cuándo usarlo:**

- ¿Es inversible? ¿para qué valores del parámetro? → $\det A\neq0$.
- Dado $\det A$, piden $\det(2A)$, $\det(A^{-1})$, $\det(A^tA)$... → propiedades, **sin calcular $A$**. Cuidado con $\det(\lambda A)=\lambda^n\det A$ ($n$ = orden, no $\lambda$ a secas).
- Si dan una matriz con filas modificadas ($f_1\leftrightarrow f_3$, $2f_2$, ...) → tabla de efectos.

## 5. Sistemas de ecuaciones lineales

**Forma matricial:** $AX=B$, con $A$ matriz de coeficientes, $X$ incógnitas, $B$ términos independientes. **Matriz ampliada:** $[A\mid B]$.

### Operaciones elementales por fila

1. Intercambiar dos filas.
2. Multiplicar una fila por un escalar $\neq0$.
3. Sumarle a una fila un múltiplo de otra.

### Clasificación (Rouché–Frobenius)

Sean $n$ la cantidad de incógnitas y $r=\operatorname{rg}(A)$ (cantidad de filas no nulas de la forma escalonada):

| Condición | Tipo | Soluciones |
|---|---|---|
| $\operatorname{rg}(A)=\operatorname{rg}(A\mid B)=n$ | **SCD** (compatible determinado) | una única |
| $\operatorname{rg}(A)=\operatorname{rg}(A\mid B)=r<n$ | **SCI** (compatible indeterminado) | infinitas, con $n-r$ parámetros libres |
| $\operatorname{rg}(A)<\operatorname{rg}(A\mid B)$ | **SI** (incompatible) | ninguna (aparece una fila $0\ 0\ 0\mid c$, $c\neq0$) |

- **Homogéneo** ($B=0$): **siempre compatible** (la solución trivial $X=0$). Tiene soluciones no triviales $\iff\det A=0$ (si es cuadrado) $\iff r<n$.
- **Cuadrado** ($A\in\mathbb{R}^{n\times n}$): $\det A\neq0\Rightarrow$ **SCD** y $X=A^{-1}B$.

### Métodos de resolución

| Método | Qué hacés | Cuándo conviene |
|---|---|---|
| **Gauss** | Escalonar $[A\mid B]$ y **sustituir hacia atrás** | Siempre; es el método general (cualquier tamaño) |
| **Gauss-Jordan** | Seguir hasta la forma **escalonada reducida** (pivotes $=1$ y ceros arriba y abajo): la solución se lee directo | Siempre; menos sustitución, más operaciones |
| **Matricial** | $X=A^{-1}B$ | $A$ cuadrada inversible; si ya tenés $A^{-1}$ |
| **Cramer** | $x_i=\dfrac{\det(A_i)}{\det(A)}$, con $A_i$ = $A$ con la columna $i$ reemplazada por $B$ | Cuadrado con $\det A\neq0$, pocas incógnitas (≤3) o si piden una sola incógnita |

**Diferencia Gauss / Gauss-Jordan:** Gauss deja una matriz *escalonada* y se despeja de abajo hacia arriba; Gauss-Jordan sigue operando hasta *escalonada reducida* y no hace falta sustituir.

### Sistemas con parámetro

1. Si es cuadrado: calcular $\det A$ (en función del parámetro) y **factorizarlo**.
2. Los valores que anulan $\det A$ son los casos **críticos**; para cualquier otro valor: **SCD**.
3. Para cada valor crítico, **reemplazarlo** y escalonar $[A\mid B]$ para decidir entre SCI y SI.
4. Si no es cuadrado: escalonar con el parámetro y fijarse en la última fila.

**Cuándo usarlo:** "discutí según $k$", "¿para qué valores de $a$ tiene solución única / infinitas / ninguna?", "sistema compatible determinado".

---

# Unidad 2 — Sistemas de coordenadas y vectores

## 6. Sistemas de coordenadas

### Polares (en $\mathbb{R}^2$): $P=(\rho,\theta)$

$$x=\rho\cos\theta,\quad y=\rho\sin\theta\qquad\qquad \rho=\sqrt{x^2+y^2},\quad \tan\theta=\frac yx$$

El ángulo $\theta$ **se ubica según el cuadrante**: no alcanza con $\arctan(y/x)$.

| Posición de $(x,y)$ | $\theta$ |
|---|---|
| $x>0,\ y\geq0$ (1.º cuadrante y eje $x^+$) | $\arctan\frac yx$ |
| $x<0$ (2.º y 3.º cuadrante) | $\arctan\frac yx+\pi$ |
| $x>0,\ y<0$ (4.º cuadrante) | $\arctan\frac yx+2\pi$ (o $\arctan\frac yx<0$) |
| $x=0,\ y>0$ | $\frac\pi2$ |
| $x=0,\ y<0$ | $\frac{3\pi}2$ |

Con $\rho=0$ (origen) $\theta$ queda indeterminado. Un mismo punto tiene infinitas representaciones: $(\rho,\theta)=(\rho,\theta+2k\pi)$.

### Cilíndricas (en $\mathbb{R}^3$): $P=(\rho,\theta,z)$

$$x=\rho\cos\theta,\quad y=\rho\sin\theta,\quad z=z\qquad\qquad\rho=\sqrt{x^2+y^2},\quad\theta\text{ como en polares}$$

### Esféricas (en $\mathbb{R}^3$): $P=(\rho,\theta,\varphi)$

Convención del **Cuadernillo**: $\rho$ = distancia al origen, $\theta$ = ángulo **cenital** (con el eje $z$, $0\le\theta\le\pi$), $\varphi$ = ángulo **azimutal** (el mismo $\theta$ de polares/cilíndricas, $0\le\varphi<2\pi$).

$$x=\rho\sin\theta\cos\varphi,\quad y=\rho\sin\theta\sin\varphi,\quad z=\rho\cos\theta$$
$$\rho=\sqrt{x^2+y^2+z^2},\qquad\theta=\arccos\frac z\rho,\qquad\varphi\ \text{(azimut, según cuadrante de }(x,y))$$

**Pasajes entre sistemas**

| De → A | Fórmula |
|---|---|
| Cilíndricas → esféricas | $\rho_{esf}=\sqrt{\rho_{cil}^2+z^2}$, $\theta=\arccos\frac{z}{\rho_{esf}}$, $\varphi=\theta_{cil}$ |
| Esféricas → cilíndricas | $\rho_{cil}=\rho\sin\theta$, $\theta_{cil}=\varphi$, $z=\rho\cos\theta$ |

:::{warning} Ojo con la notación
Muchos libros (y tus apuntes en `propio/formulas.md`) llaman $\theta$ al ángulo **azimutal** y $\varphi$ al **cenital**: está invertido respecto del Cuadernillo. Antes de resolver, fijate cuál usa el enunciado/tu docente y escribí la convención al empezar.
:::

**Cuándo usarlo:** "expresá en polares / cilíndricas / esféricas", "ecuación polar de un lugar geométrico" (reemplazar $x=\rho\cos\theta$, $y=\rho\sin\theta$ y simplificar).

## 7. Vectores: componentes, norma, operaciones

- **Vector entre puntos:** $\overrightarrow{PQ}=Q-P$ (final menos inicial).
- **Operaciones** (componente a componente): $u\pm v$, $\lambda u$.
- **Norma:** $\|v\|=\sqrt{v_1^2+v_2^2+v_3^2}$. Propiedad: $\|\lambda v\|=|\lambda|\,\|v\|$.
- **Distancia entre puntos / vectores:** $d(P,Q)=\|\overrightarrow{PQ}\|=\|Q-P\|$.
- **Versor** (unitario, norma 1) en la dirección de $v$: $\hat v=\dfrac{v}{\|v\|}$.
- **Vector de norma $m$ con la dirección de $v$:** $\pm\,m\,\hat v$.
- **Paralelos:** $u\parallel v\iff u=\lambda v\iff u\times v=0$ (en $\mathbb{R}^2$: $u_1v_2-u_2v_1=0$).
- **Combinación lineal:** $w=\alpha u+\beta v+\gamma t$; hallar los coeficientes lleva a un **sistema lineal** (Unidad 1).
- **Dependencia lineal:**
  - 2 vectores son LD $\iff$ son paralelos ($u\times v=0$).
  - 3 vectores de $\mathbb{R}^3$ son LD $\iff$ son coplanares $\iff\det=0$ (producto mixto nulo).
  - Si el determinante de la matriz con los vectores como filas es $\neq0$, son **LI**.

**Cuándo usarlo:** distancia entre dos puntos, perímetros, "hallá un vector de norma $m$ en la dirección de...".

**Ángulos directores** de $v$ (con los ejes): $\cos\alpha=\frac{v_1}{\|v\|}$, $\cos\beta=\frac{v_2}{\|v\|}$, $\cos\gamma=\frac{v_3}{\|v\|}$, con $\cos^2\alpha+\cos^2\beta+\cos^2\gamma=1$.

## 8. Producto escalar

$$u\cdot v=u_1v_1+u_2v_2+u_3v_3=\|u\|\,\|v\|\cos\theta\ \in\mathbb{R}\qquad\Rightarrow\qquad\cos\theta=\frac{u\cdot v}{\|u\|\,\|v\|},\ \ \theta\in[0,\pi]$$

| Condición | Significado |
|---|---|
| $u\cdot v=0$ | $u\perp v$ (**ortogonales**) — $\theta=\frac\pi2$ |
| $u\cdot v>0$ | ángulo **agudo** |
| $u\cdot v<0$ | ángulo **obtuso** |
| $u\cdot v=\pm\|u\|\|v\|$ | paralelos |

**Propiedades:** conmutativo, distributivo ($u\cdot(v+w)=u\cdot v+u\cdot w$), $(\lambda u)\cdot v=\lambda(u\cdot v)$, $u\cdot u=\|u\|^2$.

**Identidades útiles:**

- $\|u+v\|^2=\|u\|^2+2\,u\cdot v+\|v\|^2$ (y con $-$ para la resta). Si $u\perp v$: Pitágoras.
- Cauchy–Schwarz: $|u\cdot v|\le\|u\|\|v\|$. Desigualdad triangular: $\|u+v\|\le\|u\|+\|v\|$.

**Cuándo usarlo:** ortogonalidad, ángulo entre vectores o entre lados de un triángulo, "hallá $k$ para que...", triángulo rectángulo (producto escalar nulo entre dos lados, o Pitágoras).

**Vectores sin sentido:** $u\cdot(v\cdot w)$ y $(u\cdot v)+w$ no están definidos (escalar por vector y escalar más vector). Escalar $\cdot$ escalar no es producto escalar.

### Proyección ortogonal

$$\operatorname{proy}_v(u)=\frac{u\cdot v}{\|v\|^2}\,v\qquad\text{(vector, paralelo a }v)$$
$$\operatorname{comp}_v(u)=\frac{u\cdot v}{\|v\|}\qquad\text{(escalar, con signo)}$$
$$u=\underbrace{\operatorname{proy}_v(u)}_{\parallel v}+\underbrace{(u-\operatorname{proy}_v(u))}_{\perp v}$$

**Cuándo usarlo:** "descomponé $u$ en una parte paralela y otra perpendicular a $v$", "la sombra de $u$ sobre $v$", altura de un triángulo.

### Construir un vector con condiciones

| Pedido | Procedimiento |
|---|---|
| Ortogonal a $v$ en $\mathbb{R}^2$ | $(-v_2,v_1)$ |
| Ortogonal a $v$ en $\mathbb{R}^3$ | Plantear $v\cdot x=0$ y **elegir valores simples** (hay infinitos) |
| Ortogonal a $u$ **y** a $v$ | $u\times v$ (o resolver el sistema homogéneo $\begin{cases}u\cdot x=0\\v\cdot x=0\end{cases}$) |
| "…y de norma $m$" | dividir por la norma y multiplicar por $m$: $\ m\,\frac{x}{\|x\|}$ |
| "…que **no** sea ortogonal a $a$" | construir $x$ y **verificar** $a\cdot x\neq0$; si da $0$, cambiar la elección |
| Ángulo $\theta$ con parámetro | $\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}$, despejar y **verificar el signo** antes de elevar al cuadrado |

## 9. Producto vectorial (solo en $\mathbb{R}^3$)

$$u\times v=\begin{vmatrix}\mathbf{i}&\mathbf{j}&\mathbf{k}\\u_1&u_2&u_3\\v_1&v_2&v_3\end{vmatrix}=(u_2v_3-u_3v_2,\ u_3v_1-u_1v_3,\ u_1v_2-u_2v_1)$$

- **Resultado:** un **vector** ortogonal a $u$ y a $v$ (sentido: regla de la mano derecha).
- **Norma:** $\|u\times v\|=\|u\|\|v\|\sin\theta$. Identidad de Lagrange: $\|u\times v\|^2=\|u\|^2\|v\|^2-(u\cdot v)^2$.
- **Propiedades:** anticonmutativo ($u\times v=-v\times u$), distributivo, $(\lambda u)\times v=\lambda(u\times v)$, $u\times u=0$, **no es asociativo**.
- $u\times v=0\iff u\parallel v$ (o alguno es nulo).

**Interpretación geométrica**

$$\text{Área del paralelogramo}=\|u\times v\|\qquad\text{Área del triángulo}=\tfrac12\|u\times v\|$$

**Cuándo usarlo:** vector ortogonal a otros dos, área de triángulo/paralelogramo dados los vértices, ver si dos vectores son paralelos, resolver $u\times y=v$ (existe solución solo si $u\perp v$).

## 10. Producto mixto

$$[u,v,w]=u\cdot(v\times w)=\begin{vmatrix}u_1&u_2&u_3\\v_1&v_2&v_3\\w_1&w_2&w_3\end{vmatrix}\in\mathbb{R}$$

$$\text{Volumen del paralelepípedo}=\big|[u,v,w]\big|\qquad\text{Volumen del tetraedro}=\tfrac16\big|[u,v,w]\big|$$

- $[u,v,w]=0\iff u,v,w$ **coplanares** (LD).
- Intercambiar dos vectores cambia el signo; permutar circularmente no lo cambia.
- Altura de un tetraedro sobre la cara de $u,v$: $h=\dfrac{|[u,v,w]|}{\|u\times v\|}$.

**Cuándo usarlo:** volumen, coplanaridad de 4 puntos ($A,B,C,D$ coplanares $\iff[\overrightarrow{AB},\overrightarrow{AC},\overrightarrow{AD}]=0$), independencia lineal de tres vectores, y también para decidir si una matriz $3\times3$ con esos vectores es inversible.

---

# ¿Qué me piden? → ¿Qué uso?

| Si el enunciado dice... | Usá... | Sección |
|---|---|---|
| "calculá $AB$", "$A^2$", "$A^t$", "$2A-3B$" | operaciones de matrices (cuidado con tamaños y orden) | 2 |
| "decidí si es V o F" (matrices) | propiedades; **contraejemplo $2\times2$** para refutar | 2 |
| "hallá la inversa" | Gauss-Jordan $[A\mid I]$ o adjunta/$\det$ | 3 |
| "despejá $X$" en una ecuación matricial | $A^{-1}$ multiplicando **del mismo lado** | 3 |
| "¿es inversible?" / "¿para qué $k$ es singular?" | $\det A\neq0$ / $\det A=0$ | 4 |
| dan $\det A$ y piden $\det(2A)$, $\det(A^{-1})$... | propiedades de $\det$ | 4 |
| "resolvé el sistema" | Gauss / Gauss-Jordan | 5 |
| "clasificá el sistema (SCD, SCI, SI)" | rangos (Rouché–Frobenius) | 5 |
| "discutí según $k$" / "¿para qué $k$ hay solución única?" | $\det A(k)$ y casos críticos | 5 |
| "solución única de un sistema $n\times n$" con $\det\neq0$ | Cramer o $A^{-1}B$ | 5 |
| "solución no trivial" de un homogéneo | $\det A=0$ ($r<n$) | 5 |
| "expresá en polares / cilíndricas / esféricas" | fórmulas de pasaje + **cuadrante** | 6 |
| "distancia entre $P$ y $Q$" | $\|Q-P\|$ | 7 |
| "vector unitario" / "de norma $m$" | $\frac{v}{\|v\|}$, luego $\times m$ | 7 |
| "¿son paralelos?" | $u=\lambda v$ o $u\times v=0$ | 7, 9 |
| "ángulo entre..." | $\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}$ | 8 |
| "ortogonal / perpendicular" | $u\cdot v=0$ | 8 |
| "triángulo rectángulo" | $u\cdot v=0$ entre dos lados, o Pitágoras con el lado mayor | 8 |
| "proyección", "descomponé", "componente" | $\frac{u\cdot v}{\|v\|^2}v$ | 8 |
| "ortogonal a dos vectores" | $u\times v$ | 9 |
| "área del triángulo / paralelogramo" | $\frac12\|u\times v\|$ / $\|u\times v\|$ | 9 |
| "volumen", "coplanares", "LI de 3 vectores" | producto mixto / $\det$ | 10 |
| "escribí $w$ como combinación de $u,v,t$" | sistema lineal $\alpha u+\beta v+\gamma t=w$ | 5, 7 |

# Errores típicos

- Multiplicar matrices con tamaños incompatibles o **conmutar** el producto.
- Olvidar invertir el orden en $(AB)^t$ y $(AB)^{-1}$.
- Usar $\det(\lambda A)=\lambda\det A$ (es $\lambda^n$).
- Calcular $\arctan(y/x)$ sin revisar el cuadrante.
- Cambiar sin querer la convención de esféricas ($\theta$ cenital vs. azimutal).
- Dejar el vector **sin normalizar** cuando piden norma $1$ (o $m$).
- Al despejar $k$ en una ecuación con $\cos\theta$, no **verificar el signo** tras elevar al cuadrado.
- Concluir "$\operatorname{rg}(A)<n\Rightarrow$ SCI" sin comparar con $\operatorname{rg}(A\mid B)$ (puede ser SI).
- Aplicar Cramer cuando $\det A=0$.
