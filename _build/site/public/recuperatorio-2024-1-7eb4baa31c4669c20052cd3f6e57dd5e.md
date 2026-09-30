# Examen recuperatorio — 11/11/2024

> Tomado de *Parciales tomados otros cuatrimestres* del Cuadernillo de Álgebra II (Ingeniería en Computación, UNTREF).

## Enunciado

**1. (20 pts)** Sea el triángulo $KLM$ con vértices en $K=(1,2)$, $L=(4,5)$ y $M=(1,5)$.

a) Determinar las coordenadas polares de los vértices del triángulo.

b) Calcular la longitud de cada lado del triángulo.

c) Verificar si el triángulo $KLM$ es un triángulo rectángulo.

**2. (30 pts)** Sea el vector $a=(2,k,k+3)$ con $k\in\mathbb{R}$.

a) Encontrar, si existe, un valor de $k$ tal que el vector $a$ sea ortogonal a $b=(3,-1,2)$.

b) Si $k=4$, encontrar, si es posible, un vector $c$ tal que:

- $c$ es ortogonal a $b$.
- $c$ no es ortogonal a $a$.
- $\|c\|=2$.

**3. (30 pts)** Sea $r$ la recta definida por $r:\lambda(3,b,2)+(1,0,3)$, el plano $\Pi$ dado por $\Pi: x+2y-z=0$ y el punto $R=(1,-1,2)$.

a) Encontrar una recta que pase por $R$ y que sea alabeada con respecto a $r$.

b) Para $b=2$, hallar la distancia del punto $R$ al plano $\Pi$.

c) Calcular la intersección de $r$ con $\Pi$ para cualquier valor de $b\in\mathbb{R}$.

> El enunciado original dice "$N$ con $\Pi$"; se interpreta como la recta $r$.

**4. (20 pts)** Clasificar y encontrar los elementos principales de la cónica representada por la ecuación:

$$4x^2+9y^2-8x+18y=20$$

---

## Resolución

### Ejercicio 1

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

### Ejercicio 2

**a)** $a\cdot b=6-k+2(k+3)=k+12=0\Rightarrow\boxed{k=-12}$.

**b)** Con $k=4$, $a=(2,4,7)$. Buscamos $c=(x,y,z)$ con $3x-y+2z=0$ y $a\cdot c\neq0$.

Por ejemplo $c'=(0,2,1)$: $b\cdot c'=-2+2=0$ ✓ y $a\cdot c'=8+7=15\neq0$ ✓. Su norma es $\sqrt5$, así que para tener norma 2:

$$\boxed{c=\frac{2}{\sqrt5}(0,2,1)=\left(0,\tfrac{4}{\sqrt5},\tfrac{2}{\sqrt5}\right)}$$

### Ejercicio 3

**a)** Tomamos la dirección $(0,0,1)$, que no es paralela a $(3,b,2)$ para ningún $b$:

$$s:\ (x,y,z)=(1,-1,2)+\mu(0,0,1)=(1,-1,2+\mu)$$

Para cortar a $r$ haría falta $1+3\lambda=1\Rightarrow\lambda=0$, y entonces $y=b\lambda=0\neq-1$. No se cortan y no son paralelas, así que $s$ y $r$ son alabeadas para todo $b$.

**b)** $$d(R,\Pi)=\frac{|1-2-2|}{\sqrt6}=\frac{3}{\sqrt6}=\boxed{\frac{\sqrt6}{2}}$$

(no depende de $b$).

**c)** Reemplazando $(1+3\lambda,\ b\lambda,\ 3+2\lambda)$ en $x+2y-z=0$:

$$(1+3\lambda)+2b\lambda-(3+2\lambda)=0\ \Longrightarrow\ \lambda(1+2b)=2$$

- Si $b\neq-\frac12$: $\lambda=\frac{2}{1+2b}$ y
$$r\cap\Pi=\left\{\left(1+\tfrac{6}{1+2b},\ \tfrac{2b}{1+2b},\ 3+\tfrac{4}{1+2b}\right)\right\}$$
- Si $b=-\frac12$: queda $0=2$, sin solución. La recta es paralela al plano ($d\cdot n=1+2b=0$) y $r\cap\Pi=\varnothing$.

### Ejercicio 4

$$4(x^2-2x)+9(y^2+2y)=20\ \Rightarrow\ 4(x-1)^2-4+9(y+1)^2-9=20$$

$$4(x-1)^2+9(y+1)^2=33\ \Longrightarrow\ \frac{(x-1)^2}{33/4}+\frac{(y+1)^2}{11/3}=1$$

**Elipse** con eje focal horizontal ($y=-1$).

- Centro: $(1,-1)$.
- $a^2=\frac{33}{4}$ (semieje mayor $a=\frac{\sqrt{33}}{2}$), $b^2=\frac{11}{3}$ (semieje menor $b=\frac{\sqrt{33}}{3}$).
- $c^2=a^2-b^2=\frac{55}{12}$, $c=\frac{\sqrt{165}}{6}$.
- Vértices: $\left(1\pm\frac{\sqrt{33}}{2},-1\right)$.
- Vértices secundarios: $\left(1,-1\pm\frac{\sqrt{33}}{3}\right)$.
- Focos: $\left(1\pm\frac{\sqrt{165}}{6},-1\right)$.
- Excentricidad: $e=\frac ca=\frac{\sqrt5}{3}$.
