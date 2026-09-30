# Examen recuperatorio — 11/11/2024

> Tomado de *Parciales tomados otros cuatrimestres* del Cuadernillo de Álgebra II (Ingeniería en Computación, UNTREF).

## Consignas

**1. (20 pts)** Sea el triángulo $KLM$ con vértices en $K=(1,2)$, $L=(4,5)$ y $M=(1,5)$.

a) Determinar las coordenadas polares de los vértices del triángulo.

b) Calcular la longitud de cada lado del triángulo.

c) Verificar si el triángulo $KLM$ es un triángulo rectángulo.

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 2** (Vectores y sistemas de coordenadas) — Práctica 2.

**Qué tener en cuenta**

- Pasaje cartesianas ↔ polares: $\rho=\sqrt{x^2+y^2}$, $x=\rho\cos\theta$, $y=\rho\sin\theta$; el ángulo $\theta$ hay que ubicarlo según el cuadrante (no alcanza con $\arctan$).
- Distancia entre puntos: $d(P,Q)=\|\overrightarrow{PQ}\|$.
- Triángulo rectángulo: Pitágoras con el lado mayor como hipotenusa.

**Cómo encararlo**

1. Pasar cada vértice a polares.
2. Calcular los tres lados.
3. Verificar Pitágoras e identificar dónde está el ángulo recto.
:::

**2. (30 pts)** Sea el vector $a=(2,k,k+3)$ con $k\in\mathbb{R}$.

a) Encontrar, si existe, un valor de $k$ tal que el vector $a$ sea ortogonal a $b=(3,-1,2)$.

b) Si $k=4$, encontrar, si es posible, un vector $c$ tal que:

- $c$ es ortogonal a $b$.
- $c$ no es ortogonal a $a$.
- $\|c\|=2$.

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 2** (Vectores y sistemas de coordenadas) — Práctica 2.

**Qué tener en cuenta**

- Ortogonalidad con un parámetro: el producto escalar da una ecuación en $k$.
- Construcción de un vector con condiciones (ortogonal a uno, no ortogonal a otro, norma dada).

**Cómo encararlo**

1. En a, plantear $a\cdot b=0$ y despejar $k$.
2. En b, reemplazar $k=4$, plantear $b\cdot c=0$ y elegir una solución simple.
3. Comprobar $a\cdot c\neq0$ y normalizar a la norma pedida.
:::

**3. (30 pts)** Sea $r$ la recta definida por $r:\lambda(3,b,2)+(1,0,3)$, el plano $\Pi$ dado por $\Pi: x+2y-z=0$ y el punto $R=(1,-1,2)$.

a) Encontrar una recta que pase por $R$ y que sea alabeada con respecto a $r$.

b) Para $b=2$, hallar la distancia del punto $R$ al plano $\Pi$.

c) Calcular la intersección de $r$ con $\Pi$ para cualquier valor de $b\in\mathbb{R}$.

> El enunciado original dice "$N$ con $\Pi$"; se interpreta como la recta $r$.

:::{tip} Qué tener en cuenta y cómo encararlo
**Unidad 3** (Rectas y planos en el espacio) — Práctica 3.

**Qué tener en cuenta**

- Recta alabeada: ni paralela ni secante.
- Distancia punto–plano (no depende de $b$).
- Intersección recta–plano con parámetro $b$: discutir el caso en que se anula el coeficiente de $\lambda$ (recta paralela al plano).
- El enunciado dice "$N$"; se interpreta como la recta $r$.

**Cómo encararlo**

1. En a, elegir una dirección no paralela a $(3,b,2)$ para ningún $b$ y ver que no se corta.
2. En b, aplicar la fórmula.
3. En c, reemplazar la paramétrica en el plano, despejar $\lambda$ y separar el caso sin solución.
:::

**4. (20 pts)** Clasificar y encontrar los elementos principales de la cónica representada por la ecuación:

$$4x^2+9y^2-8x+18y=20$$

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

