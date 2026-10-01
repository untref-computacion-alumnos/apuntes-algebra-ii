# Examen parcial — 04/11/2024 (resuelto)

> Tomado de *Parciales tomados otros cuatrimestres* del Cuadernillo de Álgebra II (Ingeniería en Computación, UNTREF).

## Enunciado

**1. (25 pts)** Los puntos $A=\left(5,\frac{\pi}{3}\right)$ y $B=\left(5,\frac{5\pi}{3}\right)$ están expresados en coordenadas polares.

a) Graficar los puntos $A$ y $B$.

b) Calcular la distancia entre los puntos $A$ y $B$.

c) Determinar las coordenadas cartesianas de un punto $C$ que cumpla las siguientes condiciones:

- i. La distancia de $C$ al punto $A$ es el doble de la distancia entre $A$ y $B$.
- ii. $C$ pertenece a la recta que pasa por $A$ y por $B$.

d) ¿Es única la ubicación de $C$? Justificar la respuesta.

**2. (15 pts)** Considerá el vector $v=(4,2,-1)$. Encontrar, si es posible, dos vectores $w_1$ y $w_2$ que sean ortogonales entre sí y que también sean ortogonales a $v$.

**3. (40 pts)** Sea $r$ la recta definida por la ecuación vectorial

$$r:(x,y,z)=(1,-2,3)+\lambda(2,1,-1),$$

y sean $\pi_1$ y $\pi_2$ dos planos definidos por las ecuaciones:

$$\pi_1: x+y+z=4\qquad\qquad \pi_2: 2x-y+3z=6$$

a) Determinar si la recta $r$ es paralela a alguno de los planos $\pi_1$ o $\pi_2$. Justificar la respuesta.

b) Calcular el punto de intersección de $r$ con cada uno de los planos, si existe.

c) Encontrar las coordenadas de un punto $P$ en el plano $\pi_2$ que esté a distancia 5 del plano $\pi_1$.

d) ¿Existe un plano $\pi_3$ que contenga a la recta $r$ y sea perpendicular al plano $\pi_1$?

**4. (20 pts)** Clasificar y encontrar los elementos principales de la cónica definida por la siguiente ecuación:

$$4x^2-9y^2-24x-36y-36=0$$

---

## Resolución

### Ejercicio 1

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

### Ejercicio 2

Sí es posible. Buscamos $w_1=(a,b,c)$ con $4a+2b-c=0$; por ejemplo $w_1=(1,-2,0)$ ($4-4=0$ ✓).

Para $w_2$ tomamos el producto vectorial, que es ortogonal a ambos:

$$v\times w_1=(4,2,-1)\times(1,-2,0)=(2\cdot0-(-1)(-2),\ (-1)(1)-4\cdot0,\ 4(-2)-2\cdot1)=(-2,-1,-10)$$

Tomando el opuesto: $w_2=(2,1,10)$.

Verificación: $v\cdot w_2=8+2-10=0$ ✓ y $w_1\cdot w_2=2-2+0=0$ ✓.

$$\boxed{w_1=(1,-2,0)\qquad w_2=(2,1,10)}$$

### Ejercicio 3

Dirección de $r$: $d=(2,1,-1)$. Normales: $n_1=(1,1,1)$ y $n_2=(2,-1,3)$.

**a)**

- $d\cdot n_1=2+1-1=2\neq0$: $r$ **no** es paralela a $\pi_1$.
- $d\cdot n_2=4-1-3=0$: $r$ **es paralela** a $\pi_2$. Como el punto $(1,-2,3)\in r$ no cumple $\pi_2$ ($2+2+9=13\neq6$), $r$ no está contenida en $\pi_2$: es paralela estricta.

**b)**

- Con $\pi_1$: $(1+2\lambda)+(-2+\lambda)+(3-\lambda)=2+2\lambda=4\Rightarrow\lambda=1$. Entonces $r\cap\pi_1=\{(3,-1,2)\}$.
- Con $\pi_2$: por ser paralela estricta, $r\cap\pi_2=\varnothing$.

**c)** La distancia de $P=(x,y,z)$ a $\pi_1$ es $\frac{|x+y+z-4|}{\sqrt3}=5$, o sea $x+y+z=4\pm5\sqrt3$. Elegimos $x+y+z=4+5\sqrt3$ junto con $2x-y+3z=6$ y fijamos $z=0$:

$$x+y=4+5\sqrt3,\qquad 2x-y=6\ \Longrightarrow\ x=\tfrac{10+5\sqrt3}{3},\quad y=\tfrac{2+10\sqrt3}{3}$$

$$\boxed{P=\left(\tfrac{10+5\sqrt3}{3},\ \tfrac{2+10\sqrt3}{3},\ 0\right)}$$

Verificación: $2x-y=\frac{20+10\sqrt3-2-10\sqrt3}{3}=6$ ✓.

**d)** Sí existe. Debe contener la dirección $d$ y la normal $n_1$ (para ser perpendicular a $\pi_1$), que no son paralelas, así que su normal es:

$$n_3=d\times n_1=(2,1,-1)\times(1,1,1)=(2,-3,1)$$

Pasa por $(1,-2,3)$:

$$2(x-1)-3(y+2)+(z-3)=0\ \Longrightarrow\ \boxed{\pi_3:\ 2x-3y+z=11}$$

### Ejercicio 4

$$4(x^2-6x)-9(y^2+4y)=36\ \Rightarrow\ 4(x-3)^2-36-9(y+2)^2+36=36$$

$$4(x-3)^2-9(y+2)^2=36\ \Longrightarrow\ \frac{(x-3)^2}{9}-\frac{(y+2)^2}{4}=1$$

**Hipérbola** con eje focal horizontal ($y=-2$).

- Centro: $(3,-2)$.
- $a=3$, $b=2$, $c=\sqrt{13}$.
- Vértices: $(0,-2)$ y $(6,-2)$.
- Focos: $(3\pm\sqrt{13},-2)$.
- Excentricidad: $e=\frac{\sqrt{13}}{3}$.
- Asíntotas: $y+2=\pm\frac23(x-3)$.
