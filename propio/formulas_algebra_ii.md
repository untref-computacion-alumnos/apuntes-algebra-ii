# Álgebra II – Resumen de Fórmulas

---

## Unidad 1: Sistemas de Coordenadas

### En $\mathbb{R}^2$

- Punto: $P(x, y)$
- Distancia entre puntos: $d(P_1, P_2) = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$
- Ecuación de la recta: $y = mx + b$
- Pendiente: $m = \frac{y_2 - y_1}{x_2 - x_1}$

### Conversión Cartesianas ↔ Polares

- **Polares a Cartesianas:**
  - $x = \rho \cos\theta$
  - $y = \rho \sin\theta$
- **Cartesianas a Polares:**
  - $\rho = \sqrt{x^2 + y^2}$
  - $\theta = \begin{cases} \arctan\!\left(\dfrac{y}{x}\right), & x > 0,\, y \ge 0 \\[6pt] \arctan\!\left(\dfrac{y}{x}\right) + 2\pi, & x > 0,\, y < 0 \\[6pt] \arctan\!\left(\dfrac{y}{x}\right) + \pi, & x < 0 \\[6pt] \dfrac{\pi}{2}, & x = 0,\, y > 0 \\[6pt] \dfrac{3\pi}{2}, & x = 0,\, y < 0 \end{cases}$

---

### En $\mathbb{R}^3$

- Punto: $P(x, y, z)$
- Distancia entre puntos: $d(P_1, P_2) = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2}$

### Cartesianas ↔ Cilíndricas

- **Cilíndricas a Cartesianas:**
  - $x = \rho \cos\theta$
  - $y = \rho \sin\theta$
  - $z = z$
- **Cartesianas a Cilíndricas:**
  - $\rho = \sqrt{x^2 + y^2}$
  - $\theta = \arctan\!\left(\dfrac{y}{x}\right)$
  - $z = z$

### Cartesianas ↔ Esféricas

- **Esféricas a Cartesianas:**
  - $x = r \sinφ \cos\theta$
  - $y = r \sinφ \sin\theta$
  - $z = r \cosφ$
- **Cartesianas a Esféricas:**
  - $r = \sqrt{x^2 + y^2 + z^2}$
  - $\theta = \begin{cases}
      \arctan\!\left(\dfrac{y}{x}\right), & x > 0,\, y \ge 0 \\[6pt]
      \arctan\!\left(\dfrac{y}{x}\right) + 2\pi, & x > 0,\, y < 0 \\[6pt]
      \arctan\!\left(\dfrac{y}{x}\right) + \pi, & x < 0 \\[6pt]
      \dfrac{\pi}{2}, & x = 0,\, y > 0 \\[6pt]
      \dfrac{3\pi}{2}, & x = 0,\, y < 0
    \end{cases}$
  - $φ = \arccos\!\left(\dfrac{z}{r}\right)$

### Esféricas ↔ Cilíndricas

- **Esféricas a Cilíndricas:**
  - $\rho = r \sinφ$
  - $\theta = \theta$
  - $z = r \cosφ$
- **Cilíndricas a Esféricas:**
  - $r = \sqrt{\rho^2 + z^2}$
  - $\theta = \theta$
  - $φ = \begin{cases} \arccos\!\left(\dfrac{z}{r}\right), & z > 0 \\[6pt] \pi + \arccos\!\left(\dfrac{z}{r}\right), & z < 0 \end{cases}$

---

## Unidad 2: Vectores

### Componentes y Norma

- Vector: $\vec{v} = (v_x, v_y, v_z)$
- Norma: $\|\vec{v}\| = \sqrt{v_x^2 + v_y^2 + v_z^2}$
- Versor: $\hat{v} = \frac{\vec{v}}{\|\vec{v}\|}$

### Aritmética Vectorial

- Suma: $\vec{u} + \vec{v} = (u_x+v_x,\,u_y+v_y,\,u_z+v_z)$
- Resta: $\vec{u} - \vec{v} = (u_x-v_x,\,u_y-v_y,\,u_z-v_z)$
- Producto por escalar: $\lambda \vec{v} = (\lambda v_x, \lambda v_y, \lambda v_z)$

**Propiedades básicas:**

- Conmutativa: $\vec{u} + \vec{v} = \vec{v} + \vec{u}$
- Asociativa: $(\vec{u} + \vec{v}) + \vec{w} = \vec{u} + (\vec{v} + \vec{w})$
- Elemento neutro: $\vec{v} + \vec{0} = \vec{v}$
- Inverso aditivo: $\vec{v} + (-\vec{v}) = \vec{0}$
- Distributiva: $\lambda(\vec{u} + \vec{v}) = \lambda\vec{u} + \lambda\vec{v}$

---

### Distancia y Ángulo

- Distancia entre vectores: $d = \|\vec{u} - \vec{v}\|$
- Producto escalar: $\vec{u}\cdot\vec{v} = u_x v_x + u_y v_y + u_z v_z = \|\vec{u}\|\|\vec{v}\|\cos\theta$
- Ángulo: $\theta = \arccos\frac{\vec{u}\cdot\vec{v}}{\|\vec{u}\|\|\vec{v}\|}$
- Ortogonalidad: $\vec{u}\cdot\vec{v} = 0$

---

### Proyección Ortogonal

$\operatorname{proj}_{\vec{v}}(\vec{u}) = \frac{\vec{u}\cdot\vec{v}}{\|\vec{v}\|^2}\vec{v}$, "sombra" de ${\vec{u}}$ sobre ${\vec{v}}$

---

### Producto Vectorial

$\vec{u}\times\vec{v} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ u_x & u_y & u_z \\ v_x & v_y & v_z \end{vmatrix}$

| Componente | Fórmula               |
| ---------- | --------------------- |
| $(x)$      | $(u_y v_z - u_z v_y)$ |
| $(y)$      | $(u_z v_x - u_x v_z)$ |
| $(z)$      | $(u_x v_y - u_y v_x)$ |

- Magnitud/Norma: $\|\vec{u}\times\vec{v}\| = \|\vec{u}\|\|\vec{v}\|\sin\theta$

**Propiedades:**

- Anticonmutativo: $\vec{u}\times\vec{v} = -(\vec{v}\times\vec{u})$
- Distributivo: $\vec{u}\times(\vec{v}+\vec{w}) = \vec{u}\times\vec{v} + \vec{u}\times\vec{w}$
- $\vec{u}\times\vec{v} = \vec{0} \iff \vec{u} \parallel \vec{v}$

---

## Unidad 3: Rectas y Planos

### Rectas en $\mathbb{R}^2$

| Forma       | Ecuación                                  | Parámetros                          |
| ----------- | ----------------------------------------- | ----------------------------------- |
| Vectorial   | $(x, y) = (x_0, y_0) + \lambda(a, b)$     | $(x_0, y_0)$, $(a, b)$              |
| Paramétrica | $x = x_0 + a\lambda, y = y_0 + b\lambda$  | $(x_0, y_0)$, $(a, b)$              |
| Simétrica   | $\dfrac{x - x_0}{a} = \dfrac{y - y_0}{b}$ | $(x_0, y_0)$, $(a, b)$              |
| Explícita   | $y = mx + b$                              | $m = \dfrac{b}{a}, b = y_0 - m x_0$ |
| Implícita   | $Ax + By + C = 0$                         | $A, B, C$                           |
| Segmentaria | $\dfrac{x}{a} + \dfrac{y}{b} = 1$         | $a, b$: interceptos                 |

---

### Rectas en $\mathbb{R}^3$

| Forma                      | Ecuación                                                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------ |
| **Vectorial**              | $(x, y, z) = (x_0, y_0, z_0) + \lambda(a, b, c)$                                           |
| **Paramétrica**            | $\begin{cases} x = x_0 + a\lambda, \ y = y_0 + b\lambda, \ z = z_0 + c\lambda \end{cases}$ |
| **Simétrica**              | $\dfrac{x - x_0}{a} = \dfrac{y - y_0}{b} = \dfrac{z - z_0}{c}$                             |
| **Continua**               | $\dfrac{x - x_0}{a} = \dfrac{y - y_0}{b} = \dfrac{z - z_0}{c} = \lambda$                   |
| **Intersección de planos** | $\begin{cases} A_1x + B_1y + C_1z + D_1 = 0, \ A_2x + B_2y + C_2z + D_2 = 0 \end{cases}$   |
| **Segmentaria**            | $\dfrac{x}{a} = \dfrac{y}{b} = \dfrac{z}{c}$                                               |

| Parámetros / Interpretación                          |
| ---------------------------------------------------- |
| Punto $(x_0, y_0, z_0)$, vector director $(a, b, c)$ |
| Misma información que la vectorial                   |
| Solo válida si $a, b, c \neq 0$                      |
| Forma alternativa de la paramétrica                  |
| Recta = intersección de dos planos                   |
| Recta que pasa por el origen y corta ejes en $a,b,c$ |

---

### Planos en $\mathbb{R}^3$

- Vectorial: $\vec{r} = \vec{r_0} + \alpha\vec{u} + \beta\vec{v}$
- Implícita: $Ax + By + Cz + D = 0$
- Ecuación segmentaria: $\frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1$
- Vector normal: $\vec{n} = (A, B, C)$
- Distancia punto–plano: $d = \frac{|Ax_0 + By_0 + Cz_0 + D|}{\sqrt{A^2 + B^2 + C^2}}$

---

### Intersecciones y Distancias

- **Recta–plano:**
  Sustituir las ecuaciones paramétricas de la recta en la del plano → resolver $\lambda$.
- **Paralelismo:**
  - Recta ∥ plano ⇔ $\vec{d}\cdot\vec{n} = 0$
  - Planos paralelos ⇔ $\vec{n_1} \parallel \vec{n_2}$
- **Distancia entre planos paralelos:**
  $d = \frac{|D_2 - D_1|}{\sqrt{A^2 + B^2 + C^2}}$
- **Distancia entre rectas alabeadas:**
  $d = \frac{|(\vec{r_2} - \vec{r_1}) \cdot (\vec{d_1} \times \vec{d_2})|}{\|\vec{d_1} \times \vec{d_2}\|}$

### Intersección entre **dos planos**

Sean los planos:

$\Pi_1 : A_1x + B_1y + C_1z + D_1 = 0,\quad$

$\Pi_2 : A_2x + B_2y + C_2z + D_2 = 0$

**Vectores normales:** $\vec{n_1} = (A_1, B_1, C_1)$, $\vec{n_2} = (A_2, B_2, C_2)$

| Caso                       | Condición                                                                                                                                        | Resultado / Interpretación        |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- |
| **Paralelos distintos**    | $\vec{n_1} \parallel \vec{n_2}$ y $\dfrac{D_1}{\parallel\vec{n_1}\parallel}\ne\dfrac{D_2}{\parallel\vec{n_2}\parallel}$                          | No se cortan                      |
| **Paralelos distintos2**   | $\vec{n_1} \parallel \vec{n_2}$ y **no coincidentes** → no existe una constante $k$ tal que $A_1=kA_2,\ B_1=kB_2,\ C_1=kC_2,\ D_1=kD_2$          | Planos distintos que no se cortan |
| **Coincidentes (iguales)** | $\vec{n_1} \parallel \vec{n_2}$ y proporcionales los 4 coeficientes: $\dfrac{A_1}{A_2} = \dfrac{B_1}{B_2} = \dfrac{C_1}{C_2} = \dfrac{D_1}{D_2}$ | Mismo plano                       |
| **Secantes**               | $\vec{n_1} \times \vec{n_2} \ne \vec{0}$                                                                                                         | Se cortan en una **recta**        |

**Recta de intersección (si secantes):**

$\begin{cases} A_1x + B_1y + C_1z + D_1 = 0 \\ A_2x + B_2y + C_2z + D_2 = 0 \end{cases}$

- **Vector director:** $\vec{d} = \vec{n_1} \times \vec{n_2}$
- **Punto de la recta:** se halla imponiendo un valor fijo (por ej. $x=0$) y resolviendo el sistema.

---

### Distancia entre **dos planos paralelos**

Si los planos son paralelos:

$A_1x + B_1y + C_1z + D_1 = 0,\quad A_1x + B_1y + C_1z + D_2 = 0$

$d = \frac{|D_2 - D_1|}{\sqrt{A_1^2 + B_1^2 + C_1^2}}$

- Si $D_2 = D_1$: **planos coincidentes** → $d = 0$

---

### Intersección entre **recta y plano**

Recta:

$$
\vec{r} = \vec{r_0} + \lambda \vec{d} \Rightarrow
\begin{cases}
x = x_0 + a\lambda \\
y = y_0 + b\lambda \\
z = z_0 + c\lambda
\end{cases}
$$

Plano:

$$Ax + By + Cz + D = 0$$

Sustituyendo:

$$
A(x_0 + a\lambda) + B(y_0 + b\lambda) + C(z_0 + c\lambda) + D = 0
\Rightarrow
\lambda = -\frac{A x_0 + B y_0 + C z_0 + D}{A a + B b + C c}
$$

| Caso                      | Condición                                                 | Resultado                                          |
| ------------------------- | --------------------------------------------------------- | -------------------------------------------------- |
| **Secante**               | $A a + B b + C c \ne 0$                                   | Se cortan en **un punto** (reemplazando (\lambda)) |
| **Paralela al plano**     | $A a + B b + C c = 0$ y $A x_0 + B y_0 + C z_0 + D \ne 0$ | No hay intersección                                |
| **Contenida en el plano** | $A a + B b + C c = 0$ y $A x_0 + B y_0 + C z_0 + D = 0$   | Todos los puntos de la recta pertenecen al plano   |

---

### Distancia entre **recta y plano**

Recta: $\vec{r} = \vec{r_0} + \lambda\vec{d}$,
Plano: $Ax + By + Cz + D = 0$

- Si **recta no es paralela**, corta al plano → (d = 0).
- Si **recta ∥ plano**, la distancia entre ambos es:

$$
d = \frac{|A x_0 + B y_0 + C z_0 + D|}{\sqrt{A^2 + B^2 + C^2}}
$$

(donde ($x_0, y_0, z_0$) es un punto de la recta).

---

### Intersección entre **dos rectas en $\mathbb{R}^3$**

Rectas:

$$
\vec{r_1} = \vec{r_{01}} + \lambda \vec{d_1}, \quad
\vec{r_2} = \vec{r_{02}} + \mu \vec{d_2}
$$

Resolver el sistema:

$$
\vec{r_{01}} + \lambda \vec{d_1} = \vec{r_{02}} + \mu \vec{d_2}
$$

| Caso                     | Condición                                                             | Resultado                         |
| ------------------------ | --------------------------------------------------------------------- | --------------------------------- |
| **Secantes**             | existe solución única ($\lambda, \mu$)                                | Se cortan en un **punto**         |
| **Paralelas**            | $\vec{d_1} \parallel \vec{d_2}$ y distintos puntos                    | No se cortan                      |
| **Coincidentes**         | $\vec{d_1} \parallel \vec{d_2}$ y un punto de una pertenece a la otra | Son la **misma recta**            |
| **Alabeadas (reversas)** | $\vec{d_1}$ y $\vec{d_2}$ no son paralelos y no hay intersección      | No se cortan y no son coplanarias |

---

### Distancia entre **dos rectas**

Sean:

$$
\vec{r_1} = \vec{r_{01}} + \lambda\vec{d_1}, \quad
\vec{r_2} = \vec{r_{02}} + \mu\vec{d_2}
$$

#### Rectas alabeadas o paralelas

$$
d = \frac{|(\vec{r_{02}} - \vec{r_{01}}) \cdot (\vec{d_1} \times \vec{d_2})|}{|\vec{d_1} \times \vec{d_2}|}
$$

#### Si son paralelas

$\vec{d_1} \times \vec{d_2} = \vec{0}$, entonces:

$$
d = \frac{|(\vec{r_{02}} - \vec{r_{01}})\cdot \vec{n}|}{|\vec{n}|}
$$

donde $\vec{n}$ es un vector **normal** a las rectas (por ejemplo, igual a $\vec{d_1}$).

#### Si se cortan o coinciden

$$d = 0$$

---

## Unidad 4: Cónicas

### Ecuación general

$Ax^2 + Bxy + Cy^2 + Dx + Ey + F = 0$

### Clasificación

| Condición       | Tipo de cónica                            |
| --------------- | ----------------------------------------- |
| $B^2 - 4AC < 0$ | Elipse (o circunferencia si $A = C, B=0$) |
| $B^2 - 4AC = 0$ | Parábola                                  |
| $B^2 - 4AC > 0$ | Hipérbola                                 |

---

### Circunferencia

$(x - h)^2 + (y - k)^2 = r^2$

- Centro: $C(h, k)$
- Radio: $r$
- Ecuación general: $x^2 + y^2 + Dx + Ey + F = 0$

---

### Elipse

Eje mayor horizontal: $\frac{(x - h)^2}{a^2} + \frac{(y - k)^2}{b^2} = 1, \quad a > b$

Eje mayor vertical: $\frac{(x - h)^2}{b^2} + \frac{(y - k)^2}{a^2} = 1$

- Centro: $(h, k)$
- Vértices: $(h \pm a, k)$ ó $(h, k \pm a)$
- Focos: $(h \pm c, k)$ ó $(h, k \pm c)$
- $c^2 = a^2 - b^2$
- Excentricidad: $e = \frac{c}{a}$

---

### Parábola

Eje horizontal: $(y - k)^2 = 4p(x - h)$

Eje vertical: $(x - h)^2 = 4p(y - k)$

- Vértice: $(h, k)$
- Foco: $(h + p, k)$ ó $(h, k + p)$
- Directriz: $x = h - p$ ó $y = k - p$
- Eje focal: recta que pasa por el foco y vértice.

---

### Hipérbola

Eje transverso horizontal: $\frac{(x - h)^2}{a^2} - \frac{(y - k)^2}{b^2} = 1$
Eje transverso vertical: $\frac{(y - k)^2}{a^2} - \frac{(x - h)^2}{b^2} = 1$

- Focos: $(h \pm c, k)$ ó $(h, k \pm c)$
- $c^2 = a^2 + b^2$
- Asíntotas: $y - k = \pm \frac{b}{a}(x - h)$
- Excentricidad: $e = \frac{c}{a}$

---

### Elementos comunes

| Elemento  | Circunferencia | Elipse | Parábola | Hipérbola |
| --------- | -------------- | ------ | -------- | --------- |
| Centro    | ✓              | ✓      | ✗        | ✓         |
| Focos     | ✗              | ✓      | ✓        | ✓         |
| Directriz | ✗              | ✗      | ✓        | ✗         |
| Asíntotas | ✗              | ✗      | ✗        | ✓         |

---

### Tipos de cónica según la ecuación

| Tipo de Cónica | Condición en los Términos Cuadráticos ($x^2$ y $y^2$)                    |
| -------------- | ------------------------------------------------------------------------ |
| Elipse         | $x^2$ y $y^2$ tienen coeficientes con el mismo signo.                    |
| Círculo        | Un caso especial de elipse: $x^2$ y $y^2$ tienen coeficientes idénticos. |
| Hipérbola      | $x^2$ y $y^2$ tienen coeficientes con signos opuestos.                   |
| Parábola       | Solo una de las variables está elevada al cuadrado.                      |

---

### Ecuación de una cónica trasladada

Si el centro o vértice está en $(h, k)$: $x \to (x - h), \quad y \to (y - k)$

---

> **Referencia:** Cuadernillo de Álgebra II – Ingeniería en Computación (UNGS, 2025)
