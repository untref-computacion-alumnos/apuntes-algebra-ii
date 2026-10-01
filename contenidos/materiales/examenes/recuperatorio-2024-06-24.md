# Examen recuperatorio — 24/06/2024

> Tomado de *Parciales tomados otros cuatrimestres* del Cuadernillo de Álgebra II (Ingeniería en Computación, UNTREF).

## Consignas

**1. (30 pts)** Sea $T$ el triángulo definido por los vértices $A=(1,0)$, $B=(5,0)$ y $C=(3,\sqrt3)$.

a) Expresá a los tres puntos en coordenadas polares.

b) Hallá el perímetro del triángulo $T$.

c) ¿Es rectángulo el triángulo $T$?

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 2** (Vectores y sistemas de coordenadas) — Práctica 2.

**Qué tener en cuenta**

- Pasaje cartesianas ↔ polares: $\rho=\sqrt{x^2+y^2}$, $x=\rho\cos\theta$, $y=\rho\sin\theta$; el ángulo $\theta$ hay que ubicarlo según el cuadrante (no alcanza con $\arctan$).
- Distancia entre puntos: $d(P,Q)=\|\overrightarrow{PQ}\|$.
- Perímetro = suma de las longitudes de los tres lados.
- Triángulo rectángulo: se cumple Pitágoras con el lado mayor como hipotenusa (o dos lados con producto escalar cero).

**Cómo encararlo**

1. Pasar cada vértice a polares.
2. Calcular los tres lados con la fórmula de distancia y sumarlos.
3. Comparar el cuadrado del lado mayor con la suma de los cuadrados de los otros dos.
:::

**2. (20 pts)** Sea $v=(1,k,k-1)$ con $k\in\mathbb{R}$.

a) Hallá, si es posible, $k$ para que $v$ sea ortogonal a $u=(2,1,-1)$.

b) Para $k=1$, encontrá un vector $w$ tal que:

- $w$ es ortogonal a $u$.
- $w$ no es ortogonal a $v$.
- $\|w\|=1$.

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 2** (Vectores y sistemas de coordenadas) — Práctica 2.

**Qué tener en cuenta**

- Ortogonalidad: $v\cdot u=0$. Si la expresión no depende de $k$, puede que no haya solución (y hay que decirlo).
- Para construir un vector con condiciones, se busca uno que cumpla la ortogonalidad, se verifica la condición de *no* ortogonalidad y se ajusta la norma.

**Cómo encararlo**

1. En a, calcular $v\cdot u$ y ver si se puede anular.
2. En b, reemplazar $k$ y plantear la ecuación $u\cdot w=0$ con incógnitas $(x,y,z)$.
3. Elegir valores simples que la cumplan, comprobar $v\cdot w\neq0$ y normalizar.
:::

**3. (30 pts)** Sean $L$ la recta definida por $L:\lambda(1,a,1)+(1,0,1)$, $\Pi$ el plano definido por $\Pi: 2x+y-z=1$ y $P$ el punto $P=(0,1,1)$.

a) Hallá una recta que pase por $P$ y sea alabeada con $L$.

b) Para $a=0$, hallá la distancia de $P$ a $\Pi$.

c) Calculá $L\cap\Pi$ para cada $a\in\mathbb{R}$.

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 3** (Rectas y planos en el espacio) — Práctica 3.

**Qué tener en cuenta**

- Recta **alabeada** con otra: no es paralela y no se corta. Hay que verificar ambas cosas.
- Distancia punto–plano: $d(P,\Pi)=\frac{|ax_0+by_0+cz_0+d|}{\sqrt{a^2+b^2+c^2}}$.
- Intersección recta–plano con parámetro: discutir cuando el coeficiente de $\lambda$ se anula.

**Cómo encararlo**

1. En a, elegir una dirección que no sea paralela a la de $L$ para ningún $a$, y comprobar que no hay punto en común (plantear el sistema y ver que es incompatible).
2. En b, reemplazar $a$ y aplicar la fórmula.
3. En c, reemplazar la paramétrica en el plano, obtener una ecuación en $\lambda$ y separar casos.
:::

**4. (20 pts)** Clasificá y hallá los elementos principales de la cónica definida por la siguiente ecuación:

$$16x^2-9y^2-32x-36y=164$$

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 4** (Cónicas y cuádricas) — Práctica 4.

**Qué tener en cuenta**

- Ecuación general $Ax^2+By^2+Cx+Dy=E$ sin término $xy$: se clasifica por los signos de $A$ y $B$ (mismo signo ⇒ elipse o circunferencia; signos opuestos ⇒ hipérbola; uno solo ⇒ parábola).
- Forma canónica de cada cónica y sus elementos: centro, semiejes $a$ y $b$, $c$ (elipse: $c^2=a^2-b^2$; hipérbola: $c^2=a^2+b^2$), excentricidad $e=c/a$, focos, vértices (y asíntotas en la hipérbola).
- En la elipse $a$ es el semieje **mayor** (el mayor denominador); en la hipérbola $a^2$ va con el término positivo.

**Cómo encararlo**

1. Agrupar los términos en $x$ y en $y$ y **completar cuadrados**.
2. Pasar el término constante al otro miembro y dividir para que quede $=1$.
3. Clasificar y leer el centro $(\alpha,\beta)$ y $a$, $b$.
4. Calcular $c$ y $e$; escribir vértices, focos (y asíntotas) sobre el eje focal, que es el del término con mayor denominador (elipse) o el del término positivo (hipérbola).
:::

