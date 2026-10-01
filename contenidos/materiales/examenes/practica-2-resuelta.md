# Práctica 2: Sistemas de coordenadas — Resolución

> Basado en el *Cuadernillo de Álgebra II* (Ingeniería en Computación, UNTREF). Incluye las dos partes de la Práctica 2: **Sistemas de coordenadas** (ejercicios 1–16) y **Vectores** (ejercicios 1–30).

---

## Convenciones usadas

- **Polares** $(\rho,\theta)$: $x=\rho\cos\theta,\ y=\rho\sin\theta$.
- **Cilíndricas** $(\rho,\theta,z)$: $x=\rho\cos\theta,\ y=\rho\sin\theta,\ z=z$ ($\theta$ = ángulo azimutal, igual que en polares).
- **Esféricas** — el cuadernillo define $P=(\rho,\theta,\varphi)$ donde:
  - $\rho$: distancia al origen.
  - $\theta$: ángulo **cenital** (entre el eje $z$ y el vector posición), $0\le\theta\le\pi$.
  - $\varphi$: ángulo **azimutal** (el mismo que el $\theta$ de cilíndricas/polares), $0\le\varphi<2\pi$.

  $$x=\rho\sin\theta\cos\varphi,\qquad y=\rho\sin\theta\sin\varphi,\qquad z=\rho\cos\theta$$

  $$\rho=\sqrt{x^2+y^2+z^2},\qquad \theta=\arccos\!\left(\frac{z}{\rho}\right),\qquad \varphi=\operatorname{atan2}(y,x)$$

---

# Parte A — Sistemas de coordenadas

## Coordenadas cartesianas

### Ejercicio 1 — Representar puntos

$$(0,2)\quad (-1,\tfrac34)\quad (2,0,1)\quad (3,\tfrac16)\quad (1,\pi)\quad (-1,1,0)\quad (1,-\tfrac{\pi}{6})\quad (0,1,0)\quad (1,2,3)$$

Para graficarlos alcanza con ubicar cada uno en el plano ($\mathbb{R}^2$) o el espacio ($\mathbb{R}^3$) correspondiente:

| Punto | Espacio | Ubicación |
|---|---|---|
| $(0,2)$ | $\mathbb{R}^2$ | sobre el eje $y$, a 2 unidades del origen |
| $(-1,\tfrac34)$ | $\mathbb{R}^2$ | 2.º cuadrante ($x<0,\,y>0$) |
| $(2,0,1)$ | $\mathbb{R}^3$ | en el plano $y=0$ (plano $xz$) |
| $(3,\tfrac16)$ | $\mathbb{R}^2$ | 1.º cuadrante ($x>0,\,y>0$) |
| $(1,\pi)$ | $\mathbb{R}^2$ | 1.º cuadrante ($y=\pi\approx3.14>0$) |
| $(-1,1,0)$ | $\mathbb{R}^3$ | en el plano $z=0$ (plano $xy$), con $x<0,y>0$ |
| $(1,-\tfrac{\pi}{6})$ | $\mathbb{R}^2$ | 4.º cuadrante ($x>0,\,y<0$) |
| $(0,1,0)$ | $\mathbb{R}^3$ | sobre el eje $y$ |
| $(1,2,3)$ | $\mathbb{R}^3$ | primer octante (todas las coordenadas positivas) |

### Ejercicio 2 — Coordenadas de puntos graficados

Del gráfico (cuadrícula de $-4$ a $4$ en $x$, de $-3$ a $5$ en $y$, con divisiones menores de $0.25$):

$$A=(-2,\,3)\qquad B=(2,\,0)\qquad C=(-1,\,-1)\qquad D=(0.5,\,3)$$

### Ejercicio 3 — Nombrar los puntos graficados

Con $A=(1,2,0)$, $B=(0,0,3)$, $C=(4,0,0)$ y $D=(2,-2,-2)$, en el gráfico 3D:

- El punto que está **sobre el eje $z$** (altura 3, sin componentes $x,y$) es $B$.
- El punto que está **sobre el eje $x$** (a distancia 4, sin componentes $y,z$) es $C$.
- El punto que está **en el plano de referencia** $z=0$ (dentro de la grilla) es $A$.
- El punto que está **por debajo del plano** de referencia (con $z<0$) es $D$.

### Ejercicio 4 — Representar conjuntos en $\mathbb{R}^2$

$$A=\{(x,y)\ /\ x=1\}\qquad B=\{(x,y)\ /\ x\ge 2\}$$
$$C=\{(x,y)\ /\ y<3\}\qquad D=\{(x,y)\ /\ x=-1 \wedge y>4\}$$
$$E=\{(x,y)\ /\ y=2x-1\}\qquad F=\{(x,y)\ /\ xy=0\}$$
$$G=\{(x,y)\ /\ xy<0\}\qquad H=\{(x,y)\ /\ xy=1\}$$

Descripción geométrica de cada uno:

- $A$: recta vertical $x=1$.
- $B$: semiplano cerrado a la derecha de (e incluyendo) la recta $x=2$.
- $C$: semiplano abierto por debajo de la recta $y=3$.
- $D$: semirrecta abierta sobre $x=-1$, con $y>4$ (sin incluir el punto $(-1,4)$).
- $E$: recta de pendiente $2$ y ordenada al origen $-1$.
- $F$: unión de los dos ejes coordenados ($x=0$ o $y=0$).
- $G$: 2.º y 4.º cuadrantes, abiertos (sin los ejes).
- $H$: hipérbola equilátera $y=1/x$ (dos ramas, en el 1.º y 3.º cuadrante).

### Ejercicio 5 — Uniones e intersecciones (usando los conjuntos del ejercicio 4)

- $A\cup B$: la recta $x=1$ junto con el semiplano $x\ge2$.
- $A\cap B=\varnothing$ (la recta $x=1$ no tiene puntos con $x\ge2$).
- $B\cap C=\{(x,y): x\ge2 \wedge y<3\}$: cuarto de plano.
- $A\cup D$: la recta $x=1$ (completa) junto con la semirrecta $\{x=-1,y>4\}$.
- $A\cap D=\varnothing$ ($x=1$ y $x=-1$ son incompatibles).
- $B\cap D=\varnothing$ ($D$ tiene $x=-1$, que no cumple $x\ge2$).
- $E\cup B$: la recta $y=2x-1$ junto con el semiplano $x\ge2$.
- $E\cap G$: puntos de la recta $E$ con $xy<0$. Como $y=2x-1$, $xy=x(2x-1)=2x^2-x<0 \iff 0<x<\tfrac12$. Es el **segmento abierto** de la recta $E$ entre $(0,-1)$ y $(\tfrac12,0)$ (extremos excluidos).
- $A\cap H$: en $H$, $y=1/x$; con $x=1$ resulta $y=1$. Es el **punto único** $(1,1)$.

### Ejercicio 6 — Representar conjuntos en $\mathbb{R}^3$

$$A=\{(x,y,z)/x=1\}\qquad B=\{(x,y,z)/x<2 \wedge y<2\}$$
$$C=\{(x,y,z)/xz=0\}\qquad D=\{(x,y,z)/z=x \wedge y=0\}$$

- $A$: plano paralelo al plano $yz$, en $x=1$.
- $B$: prisma infinito (abierto) definido por $x<2$ e $y<2$, sin restricción en $z$.
- $C$: unión de dos planos: $x=0$ (plano $yz$) **o** $z=0$ (plano $xy$).
- $D$: intersección del plano $z=x$ con el plano $y=0$ → es una **recta**: $\{(t,0,t): t\in\mathbb{R}\}$, con vector director $(1,0,1)$.

---

## Coordenadas polares

### Ejercicio 7 — Polares a cartesianas (y polares equivalentes)

Cada punto polar $(\rho,\theta)$ admite representaciones equivalentes $(\rho,\theta+2k\pi)$ o $(-\rho,\theta+\pi+2k\pi)$, $k\in\mathbb{Z}$.

| Polar dado | Cartesiano ($x=\rho\cos\theta,\ y=\rho\sin\theta$) | Otra representación polar equivalente |
|---|---|---|
| $(2,\tfrac{\pi}{4})$ | $(\sqrt2,\sqrt2)$ | $(-2,\ \tfrac{5\pi}{4})$ |
| $(1,0)$ | $(1,0)$ | $(-1,\pi)$ |
| $(1,\tfrac{\pi}{6})$ | $\left(\tfrac{\sqrt3}{2},\tfrac12\right)$ | $(-1,\ \tfrac{7\pi}{6})$ |
| $(5,\tfrac{3\pi}{4})$ | $\left(-\tfrac{5\sqrt2}{2},\tfrac{5\sqrt2}{2}\right)$ | $(-5,\ \tfrac{7\pi}{4})$ (o $-\tfrac{\pi}{4}$) |

### Ejercicio 8 — Cartesianas a polares

$$\rho=\sqrt{x^2+y^2},\qquad \theta=\operatorname{atan2}(y,x)$$

- $(1,1)$: $\rho=\sqrt{1+1}=\sqrt2$, $\theta=\arctan(1/1)=\dfrac{\pi}{4}$ (1.º cuadrante). $\Rightarrow (\sqrt2,\ \tfrac{\pi}{4})$.
- $(\sqrt2,1)$: $\rho=\sqrt{2+1}=\sqrt3$, $\theta=\arctan\!\left(\dfrac{1}{\sqrt2}\right)\approx35.26^\circ\approx0.6155\text{ rad}$. $\Rightarrow (\sqrt3,\ \arctan(1/\sqrt2))$.

### Ejercicio 9 — Ecuación polar de un lugar geométrico

$$x^2+y^2-4x-2y+1=0$$

Completando cuadrados: $(x-2)^2+(y-1)^2=4$ → circunferencia de centro $(2,1)$ y radio $2$ (no pasa por el origen).

Sustituyendo $x=\rho\cos\theta,\ y=\rho\sin\theta$ (y usando $x^2+y^2=\rho^2$):

$$\boxed{\rho^2-4\rho\cos\theta-2\rho\sin\theta+1=0}$$

Como cuadrática en $\rho$: $\rho^2-2\rho(2\cos\theta+\sin\theta)+1=0$, de donde

$$\rho=(2\cos\theta+\sin\theta)\pm\sqrt{(2\cos\theta+\sin\theta)^2-1}$$

(válida solo para los $\theta$ en que el radicando es $\ge0$, ya que el origen queda fuera de la circunferencia).

### Ejercicio 10 — Tercer vértice de un triángulo rectángulo

Puntos dados (pasados a cartesianas): $P_1=(1,0)$ y $P_2=\left(2,\tfrac{\pi}{4}\right)=(\sqrt2,\sqrt2)$.

Se interpreta que el triángulo rectángulo tiene sus **catetos paralelos a los ejes** (la construcción clásica: completar el "rectángulo" que definen los dos puntos). Los dos vértices posibles son las esquinas del rectángulo determinado por $P_1$ y $P_2$:

$$Q_1=(1,\ \sqrt2)\qquad\text{o}\qquad Q_2=(\sqrt2,\ 0)$$

En ambos casos el ángulo recto queda en el tercer vértice ($Q_1$ o $Q_2$), con catetos horizontal y vertical.

*(Nota: si no se exige que los catetos sean paralelos a los ejes, hay infinitos puntos posibles — todo el círculo de Thales de diámetro $P_1P_2$ sirve como lugar de vértices con ángulo recto allí. La respuesta de arriba es la que se obtiene con la construcción usual de estos ejercicios.)*

---

## Coordenadas cilíndricas y esféricas

### Ejercicio 11 — Cilíndricas a cartesianas y a esféricas

Puntos cilíndricos $(\rho,\theta,z)$:

**a) $(0,\tfrac{\pi}{4},10)$**
Cartesianas: $\rho=0\Rightarrow(0,0,10)$.
Esféricas: $\rho_{esf}=\sqrt{0^2+10^2}=10$; $\theta_{esf}=\arccos(10/10)=0$; $\varphi$ indefinido (el punto está sobre el eje $z$, cualquier azimut sirve). $\Rightarrow (10,\,0,\,\varphi\text{ arbitrario})$.

**b) $(1,-\tfrac{\pi}{6},0)$**
Cartesianas: $x=\cos(-\tfrac{\pi}{6})=\tfrac{\sqrt3}{2}$, $y=\sin(-\tfrac{\pi}{6})=-\tfrac12$, $z=0\Rightarrow\left(\tfrac{\sqrt3}{2},-\tfrac12,0\right)$.
Esféricas: $\rho_{esf}=\sqrt{1+0}=1$; $\theta_{esf}=\arccos(0/1)=\tfrac{\pi}{2}$; $\varphi=-\tfrac{\pi}{6}$. $\Rightarrow\left(1,\ \tfrac{\pi}{2},\ -\tfrac{\pi}{6}\right)$.

**c) $(3,\tfrac{\pi}{6},4)$**
Cartesianas: $x=3\cos(\tfrac\pi6)=\tfrac{3\sqrt3}{2}$, $y=3\sin(\tfrac\pi6)=\tfrac32$, $z=4\Rightarrow\left(\tfrac{3\sqrt3}{2},\tfrac32,4\right)$.
Esféricas: $\rho_{esf}=\sqrt{3^2+4^2}=5$; $\theta_{esf}=\arccos(4/5)\approx36.87^\circ$; $\varphi=\tfrac\pi6$. $\Rightarrow\left(5,\ \arccos\tfrac45,\ \tfrac{\pi}{6}\right)$.

**d) $(2,\tfrac{3\pi}{4},-2)$**
Cartesianas: $x=2\cos(\tfrac{3\pi}4)=-\sqrt2$, $y=2\sin(\tfrac{3\pi}4)=\sqrt2$, $z=-2\Rightarrow(-\sqrt2,\sqrt2,-2)$.
Esféricas: $\rho_{esf}=\sqrt{2^2+(-2)^2}=2\sqrt2$; $\theta_{esf}=\arccos\!\left(\tfrac{-2}{2\sqrt2}\right)=\arccos\!\left(-\tfrac{1}{\sqrt2}\right)=\tfrac{3\pi}{4}$; $\varphi=\tfrac{3\pi}{4}$. $\Rightarrow\left(2\sqrt2,\ \tfrac{3\pi}{4},\ \tfrac{3\pi}{4}\right)$.

### Ejercicio 12 — Coordenadas esféricas de puntos cartesianos

**$(1,-1,1)$:** $\rho=\sqrt{1+1+1}=\sqrt3$; $\theta=\arccos\!\left(\tfrac{1}{\sqrt3}\right)\approx54.74^\circ$; $\varphi=\operatorname{atan2}(-1,1)=-\tfrac{\pi}{4}$.
$$\Rightarrow \left(\sqrt3,\ \arccos\tfrac{1}{\sqrt3},\ -\tfrac{\pi}{4}\right)$$

**$(0,1,0)$:** $\rho=1$; $\theta=\arccos(0/1)=\tfrac{\pi}{2}$; $\varphi=\operatorname{atan2}(1,0)=\tfrac{\pi}{2}$.
$$\Rightarrow \left(1,\ \tfrac{\pi}{2},\ \tfrac{\pi}{2}\right)$$

### Ejercicio 13 — Esféricas a cartesianas

Punto esférico $\left(3,\tfrac{\pi}{6},\tfrac{\pi}{4}\right)$ (es decir $\rho=3,\theta=\tfrac\pi6,\varphi=\tfrac\pi4$):

$$z=\rho\cos\theta=3\cos\tfrac{\pi}{6}=\frac{3\sqrt3}{2}\qquad \rho\sin\theta=3\sin\tfrac\pi6=\frac32$$
$$x=\frac32\cos\tfrac{\pi}{4}=\frac{3\sqrt2}{4}\qquad y=\frac32\sin\tfrac{\pi}{4}=\frac{3\sqrt2}{4}$$

$$\boxed{\left(\frac{3\sqrt2}{4},\ \frac{3\sqrt2}{4},\ \frac{3\sqrt3}{2}\right)}$$

### Ejercicio 14 — Significado geométrico de asociaciones en cilíndricas

- $(r,\theta,z)\to(r,\theta,-z)$: **simetría respecto del plano $z=0$** (reflejo especular horizontal).
- $(r,\theta,z)\to(r,\theta+\pi,-z)$: como $\cos(\theta+\pi)=-\cos\theta$ y $\sin(\theta+\pi)=-\sin\theta$, esto equivale a $(x,y,z)\to(-x,-y,-z)$: **simetría central respecto del origen**.
- $(r,\theta,z)\to(r,\theta-\tfrac{\pi}{4},z)$: **rotación rígida de $\tfrac{\pi}{4}$ (en sentido horario) alrededor del eje $z$**, manteniendo la altura.

### Ejercicio 15 — Tanque cilíndrico acostado

Tanque: cilindro circular recto, radio $R=3\,\text{m}$, altura (ahora longitud, al estar acostado) $L=5\,\text{m}$, con la mitad de líquido.

Se eligen coordenadas cilíndricas $(\rho,\theta,z)$ con el eje $z$ coincidiendo con el **eje del cilindro** (horizontal), $0\le z\le5$, y $\theta$ el ángulo en el plano transversal medido de modo que $\theta=\tfrac{\pi}{2}$ apunte "hacia arriba" (verticalmente).

Como el líquido ocupa exactamente la mitad del volumen y la sección transversal es un círculo, por simetría el nivel del líquido coincide con el **diámetro horizontal**: el líquido llena la mitad inferior de cada sección circular y el aire la mitad superior, para todo $z$.

$$\text{Aire}=\{(\rho,\theta,z)\ :\ 0\le\rho\le3,\ \ 0<\theta<\pi,\ \ 0\le z\le5\}$$

(la mitad "de arriba" del cilindro); el líquido es el conjunto complementario $\pi<\theta<2\pi$.

### Ejercicio 16 — Descripción de conjuntos graficados

1. **Circunferencia** centrada en el origen, radio $\tfrac52$:
   $$\{(x,y): x^2+y^2=\tfrac{25}{4}\}\qquad\text{(en polares: }\rho=\tfrac52\text{)}$$
2. **Arco de parábola "acostada"** $x=y^2$, para $-1\le y\le1$ (equivalentemente $0\le x\le1$):
   $$\{(x,y): x=y^2,\ -1\le y\le1\}$$
3. **Segmento de recta** $y=x+2$, para $-3\le x\le2$:
   $$\{(x,y): y=x+2,\ -3\le x\le2\}$$
4. **Arco de parábola** $y=x^2$, para $-1\le x\le2$:
   $$\{(x,y): y=x^2,\ -1\le x\le2\}$$
5. **Borde de un rectángulo** de vértices $(1,1),(5,1),(5,4),(1,4)$ — es la unión de los 4 lados:
   $$\{(x,y): 1\le x\le5,\ y=1\}\cup\{(x,y): 1\le x\le5,\ y=4\}\cup\{(x,y): x=1,\ 1\le y\le4\}\cup\{(x,y): x=5,\ 1\le y\le4\}$$
6. **Curva** $y=\sqrt{x+1}$, para $0\le x\le15$:
   $$\{(x,y): y=\sqrt{x+1},\ 0\le x\le15\}$$

---

# Parte B — Vectores

### Ejercicio 1 — Fuerza que contrarresta

$F_1=(1,3)$, $F_2=(5,4)$. Para anular el efecto conjunto, la tercera fuerza debe ser la opuesta de la resultante:

$$F_3=-(F_1+F_2)=-(6,7)=\boxed{(-6,-7)}$$

### Ejercicio 2 — Graficar vectores desde el origen

**a) En $\mathbb{R}^2$:**

| Vector | Cuadrante / eje |
|---|---|
| $v_1=(2,5)$ | 1.º cuadrante |
| $v_2=(-3,4)$ | 2.º cuadrante |
| $v_3=(-4,-2)$ | 3.º cuadrante |
| $v_4=(0,8)$ | sobre el eje $+y$ |
| $v_5=(3,0)$ | sobre el eje $+x$ |

**b) En $\mathbb{R}^3$:** $v_6=(2,0,1)$ (en el plano $xz$), $v_7=(0,0,-3)$ (sobre el eje $-z$), $v_8=(2,1,3)$ (primer octante).

Cada uno se dibuja como una flecha desde $O=(0,0,\dots)$ hasta el punto de sus coordenadas.

### Ejercicio 3 — Módulo, dirección y sentido

**a) En $\mathbb{R}^2$:** $P_1=(-2,1)$, $P_2=(2,-3)$.
$$v=P_2-P_1=(4,-4)\qquad \|v\|=\sqrt{16+16}=4\sqrt2$$
Dirección: $\theta=\operatorname{atan2}(-4,4)=-45^\circ$ (o $315^\circ$). Sentido: hacia la derecha y hacia abajo, formando $45^\circ$ por debajo del semieje $+x$.

**b) En $\mathbb{R}^3$:** $P_1=(6,3,7)$, $P_2=(8,-7,-2)$.
$$v=P_2-P_1=(2,-10,-9)\qquad \|v\|=\sqrt{4+100+81}=\sqrt{185}\approx13.60$$
Ángulos directores: $\cos\alpha=\tfrac{2}{\sqrt{185}}\Rightarrow\alpha\approx81.55^\circ$; $\cos\beta=\tfrac{-10}{\sqrt{185}}\Rightarrow\beta\approx137.34^\circ$; $\cos\gamma=\tfrac{-9}{\sqrt{185}}\Rightarrow\gamma\approx131.44^\circ$.

### Ejercicio 4 — Vector paralelo con punto final fijo

$v=(-2,4,-1)$, punto final $Q=(2,0,-7)$. ¿Es única?

**No.** Cualquier vector $\lambda v$ ($\lambda\ne0$) es paralelo a $v$, y para cada $\lambda$ existe un único punto inicial $P=Q-\lambda v$ tal que el vector "de $P$ a $Q$" es exactamente $\lambda v$:
$$P=(2+2\lambda,\ -4\lambda,\ -7+\lambda),\qquad \lambda\in\mathbb{R}\setminus\{0\}$$
Hay infinitas soluciones (todas las direcciones son la misma recta, pero cambian magnitud/sentido y punto inicial). Un ejemplo concreto con $\lambda=1$: el vector $(-2,4,-1)$ ubicado con punto inicial $P=(4,-4,-6)$ y final $Q=(2,0,-7)$.

### Ejercicio 5 — Operaciones con $u,v,w$

$u=(-2,4,-1)$, $v=(2,0,-7)$, $w=(3,-2,1)$.

**a)**
$$\text{i. } u-w=(-5,\,6,\,-2)$$
$$\text{ii. } w+v=(5,\,-2,\,-6)$$
$$\text{iii. } 2v-(u+v)=v-u=(4,\,-4,\,-6)$$

**b)** Hallar $\alpha,\beta,\gamma$ tales que $\alpha v+\beta u+\gamma w=(6,4,-2)$.

Sistema:
$$\begin{cases}2\alpha-2\beta+3\gamma=6\\ 4\beta-2\gamma=4\\ -7\alpha-\beta+\gamma=-2\end{cases}$$

De la 2.ª: $\gamma=2\beta-2$. Sustituyendo en la 3.ª: $\beta=7\alpha$. Sustituyendo ambas en la 1.ª: $30\alpha=12\Rightarrow\alpha=\tfrac25$.

$$\boxed{\alpha=\frac25,\qquad \beta=\frac{14}{5},\qquad \gamma=\frac{18}{5}}$$

(Verificación: $\tfrac25v+\tfrac{14}{5}u+\tfrac{18}{5}w=(6,4,-2)$ ✓.)

### Ejercicio 6 — Copias en tres centros

$a=(25,211,818)$ (diciembre, en miles), $b=(331,3227,1377)$ (los once meses anteriores).

$$a+b=(356,\ 3438,\ 2195)$$

Representa el **total de copias hechas en el año completo** (12 meses) por cada uno de los tres centros de copiado, en miles.

### Ejercicio 7 — Normas

$$\text{a) } v=(2,6):\ \|v\|=\sqrt{40}=2\sqrt{10}\qquad\qquad \text{c) } v=(-2,-6):\ \|v\|=\sqrt{40}=2\sqrt{10}$$
$$\text{b) } v=(-1,0,2):\ \|v\|=\sqrt{5}\qquad\qquad\qquad\ \, \text{d) } v=(4,0,0):\ \|v\|=4$$

### Ejercicio 8 — Distancias

**a)** $P_1=(2,3)$, $P_2=(-2,-3)$: $d=\sqrt{4^2+6^2}=\sqrt{52}=2\sqrt{13}$.

**b)** $P_1=(8,-4,2)$, $P_2=(-6,-1,0)$: $d=\sqrt{14^2+(-3)^2+2^2}=\sqrt{196+9+4}=\sqrt{209}$.

### Ejercicio 9 — Existencia de $b$

$u=(4,3)$, $v=(-1,b)$. $u\cdot v=-4+3b=2\Rightarrow b=2$. **Sí existe**, $b=2$.

### Ejercicio 10 — Ángulos de un triángulo

Vértices $A=(9,5)$, $B=(7,3)$, $C=(4,5)$.

$$\vec{AB}=(-2,-2),\quad \vec{AC}=(-5,0),\quad \vec{BC}=(-3,2)$$

- Ángulo en $A$: $\cos A=\dfrac{\vec{AB}\cdot\vec{AC}}{\|\vec{AB}\|\|\vec{AC}\|}=\dfrac{10}{2\sqrt2\cdot5}=\dfrac{1}{\sqrt2}\Rightarrow A=45^\circ$.
- Ángulo en $B$: $\vec{BA}=(2,2)$, $\vec{BC}=(-3,2)$. $\cos B=\dfrac{-2}{2\sqrt2\sqrt{13}}=\dfrac{-1}{\sqrt{26}}\Rightarrow B=\arccos\!\left(-\tfrac{1}{\sqrt{26}}\right)\approx101.31^\circ$.
- Ángulo en $C$: $\vec{CA}=(5,0)$, $\vec{CB}=(3,-2)$. $\cos C=\dfrac{15}{5\sqrt{13}}=\dfrac{3}{\sqrt{13}}\Rightarrow C=\arccos\!\left(\tfrac{3}{\sqrt{13}}\right)\approx33.69^\circ$.

(Suma $\approx180^\circ$ ✓.)

### Ejercicio 11 — Cálculos con $u,v,w$

$u=(-2,4,-1)$, $v=(2,0,-7)$, $w=(3,-2,1)$.

**a)** $u+v=(0,4,-8)\Rightarrow \|u+v\|=\sqrt{80}=4\sqrt5$.

**b)** $\|u\|=\sqrt{21}$, $\|v\|=\sqrt{53}\Rightarrow \|u\|+\|v\|=\sqrt{21}+\sqrt{53}\ (\approx11.86)$.

**c)** $\|w\|=\sqrt{9+4+1}=\sqrt{14}$. $\dfrac{1}{\|w\|}w=\left(\dfrac{3}{\sqrt{14}},\dfrac{-2}{\sqrt{14}},\dfrac{1}{\sqrt{14}}\right)$ (el versor de $w$).

**d)** $\left\|\dfrac{1}{\|w\|}w\right\|=1$ (todo versor tiene norma $1$).

### Ejercicio 12 — Efecto de escalar en la norma

Para cualquier $v\ne0$, $\|\lambda v\|=|\lambda|\,\|v\|$. Por lo tanto (tomando p. ej. $v=(1,2)$ como ejemplo, aunque el resultado es general):

- **a)** $\|\lambda v\|>\|v\| \iff |\lambda|>1$ (es decir $\lambda>1$ o $\lambda<-1$).
- **b)** $\|\lambda v\|<\|v\| \iff |\lambda|<1$ (es decir $-1<\lambda<1$).
- **c)** $\|\lambda v\|=\|v\| \iff |\lambda|=1$ (es decir $\lambda=1$ o $\lambda=-1$).

### Ejercicio 13 — Hallar $k$

$v=(-1,2,4)$, $\|v\|=\sqrt{21}$. $\|kv\|=|k|\sqrt{21}=2\Rightarrow |k|=\dfrac{2}{\sqrt{21}}$.

$$\boxed{k=\pm\frac{2\sqrt{21}}{21}}$$

### Ejercicio 14 — Ángulos directores

$v=\left(\tfrac12,\tfrac{\sqrt2}{2}\right)$: $\|v\|=\sqrt{\tfrac14+\tfrac12}=\tfrac{\sqrt3}{2}$.
$$\cos\alpha=\frac{1/2}{\sqrt3/2}=\frac{1}{\sqrt3}\Rightarrow\alpha\approx54.74^\circ\qquad \cos\beta=\frac{\sqrt2/2}{\sqrt3/2}=\sqrt{\frac23}\Rightarrow\beta\approx35.26^\circ$$

$w=\left(-\tfrac{\sqrt3}{2},\tfrac12\right)$: $\|w\|=\sqrt{\tfrac34+\tfrac14}=1$ (versor).
$$\cos\alpha=-\frac{\sqrt3}{2}\Rightarrow\alpha=150^\circ\qquad \cos\beta=\frac12\Rightarrow\beta=60^\circ$$

### Ejercicio 15 — Producto escalar y ángulo

| $u$ | $v$ | $u\cdot v$ | $\theta$ |
|---|---|---|---|
| $(3,0)$ | $(1,1)$ | $3$ | $\arccos\!\left(\tfrac{1}{\sqrt2}\right)=45^\circ$ |
| $(-5,0)$ | $(0,18)$ | $0$ | $90^\circ$ |
| $(1,1,1)$ | $(-2,-1,1)$ | $-2$ | $\arccos\!\left(-\tfrac{\sqrt2}{3}\right)\approx118.13^\circ$ |
| $(2,1,-2)$ | $(1,-3,2)$ | $-5$ | $\arccos\!\left(-\tfrac{5}{\sqrt{126}}\right)\approx116.45^\circ$ |

### Ejercicio 16 — ¿Ortogonales?

- **a)** $u=(4,0),v=(1,1)$: $u\cdot v=4\ne0$ → **no** ortogonales.
- **b)** $u=(2,18),v=\left(\tfrac32,-\tfrac16\right)$: $u\cdot v=3-3=0$ → **sí**, ortogonales.
- **c)** $u=(-6,12,6),v=(1,-2,-1)$: $u\cdot v=-6-24-6=-36\ne0$ → **no** ortogonales.

### Ejercicio 17 — Vectores ortogonales con restricción

$v=(-1,3,2)$. Buscar $x=(x_1,x_2,x_3)$ con $x\perp v$ y $x_2=4$:

$$x\cdot v=-x_1+3(4)+2x_3=0 \Rightarrow x_1=12+2x_3$$

$$\boxed{x=(12+2t,\ 4,\ t),\quad t\in\mathbb{R}}$$

### Ejercicio 18 — Hallar $\|u\|$

Ángulo entre $u,v$ es $\tfrac{\pi}{3}$, $\|v\|=4$, $(u-v)\perp u$.

$(u-v)\cdot u=0 \Rightarrow \|u\|^2=u\cdot v=\|u\|\|v\|\cos\tfrac\pi3=4\|u\|\cdot\tfrac12=2\|u\|$

$$\|u\|^2-2\|u\|=0\Rightarrow \|u\|(\|u\|-2)=0\Rightarrow \boxed{\|u\|=2}\ (\text{descartando }\|u\|=0)$$

### Ejercicio 19 — $u=(1,1,1)$, $v=(1,-1,-1)$

**a)** Vectores no nulos $\perp$ a ambos: cualquier múltiplo no nulo de $u\times v$.
$$u\times v=(0,2,-2)\ \sim\ (0,1,-1)\qquad\Rightarrow\ \lambda(0,1,-1),\ \lambda\ne0$$

**b)** Dos vectores unitarios: normalizando $(0,1,-1)$ (norma $\sqrt2$):
$$\pm\left(0,\ \frac{\sqrt2}{2},\ -\frac{\sqrt2}{2}\right)$$

**c)** Ángulo entre $u$ y $v$: $u\cdot v=1-1-1=-1$, $\|u\|=\|v\|=\sqrt3$.
$$\theta=\arccos\!\left(-\frac13\right)\approx109.47^\circ$$

### Ejercicio 20 — Agudo, obtuso o recto

- **a)** $u=(6,1,3),v=(4,0,-6)$: $u\cdot v=24+0-18=6>0$ → **agudo**.
- **b)** $u=(1,1,1),v=(-1,0,0)$: $u\cdot v=-1<0$ → **obtuso**.
- **c)** $u=(4,1,6),v=(-3,6,-9)$: $u\cdot v=-12+6-54=-60<0$ → **obtuso**.

### Ejercicio 21 — Vectores a $55°$ de $u=(5,3)$

Existen exactamente **dos direcciones** (rectas por el origen, rotando $u$ en $+55^\circ$ y en $-55^\circ$) que forman ese ángulo con $u$; sobre cada una hay infinitos vectores posibles (cualquier múltiplo positivo). En total: **infinitos vectores**, agrupados en dos semirrectas.

### Ejercicio 22 — Proyección ortogonal

**a)** $u=(2,6)$, $v=(9,3)$: $u\cdot v=36$, $\|v\|^2=90$.
$$\operatorname{Pr}_v(u)=\frac{36}{90}(9,3)=\left(\frac{18}{5},\frac{6}{5}\right)$$

**b)** $u=(-7,3,1)$, $v=(5,0,1)$: $u\cdot v=-34$, $\|v\|^2=26$.
$$\operatorname{Pr}_v(u)=\frac{-34}{26}(5,0,1)=\left(-\frac{85}{13},\ 0,\ -\frac{17}{13}\right)$$

### Ejercicio 23 — Dos versores ortogonales a $v=(3,-2)$

Un vector ortogonal a $(3,-2)$ es $(2,3)$ (se intercambian las componentes y se cambia un signo). $\|(2,3)\|=\sqrt{13}$.

$$\boxed{\pm\left(\frac{2}{\sqrt{13}},\ \frac{3}{\sqrt{13}}\right)}$$

### Ejercicio 24 — Tres versores ortogonales a $v=(3,-2)$

**No es posible.** En $\mathbb{R}^2$, el conjunto de vectores ortogonales a un $v\ne0$ es un subespacio de dimensión $1$ (una recta), que contiene exactamente **dos** vectores de norma $1$ (opuestos entre sí: los del ejercicio 23). No puede existir un tercero.

### Ejercicio 25 — Paralelismo con parámetro

$v=(1-a,\,a+2)$, $w=(2,-b)$. Paralelismo $\iff$ determinante nulo:
$$(1-a)(-b)-(a+2)(2)=0 \Rightarrow -b(1-a)=2a+4 \Rightarrow b=\frac{2(a+2)}{a-1}\quad (a\ne1)$$

Si $a=1$: $v=(0,3)$, que nunca es paralelo a $w=(2,-b)$ (pues $w$ siempre tiene componente $x=2\ne0$). **No hay solución** en ese caso.

*(Representación gráfica: para cada valor de $a\ne1$, $v$ y $b\cdot$ correspondiente dan dos vectores sobre la misma recta por el origen.)*

### Ejercicio 26 — Operaciones con $u,v,w$

$u=(1,2)$, $v=(4,-2)$, $w=(6,0)$.

**a)** $7v+w=(34,-14)$; $\ u\cdot(7v+w)=34-28=6$.

**b)** $u\cdot v=4-4=0\Rightarrow (u\cdot v)w=\vec0 \Rightarrow \|(u\cdot v)w\|=0$.

**c)** $\|u\|=\sqrt5$; $v\cdot w=24+0=24$; $\ \|u\|\,(v\cdot w)=24\sqrt5$.

### Ejercicio 27 — Expresiones sin significado

**a)** $u\cdot(v\cdot w)$: $v\cdot w$ es un **escalar**; el producto escalar necesita dos vectores, no un vector y un número. **Sin sentido.**

**b)** $(u\cdot v)+w$: $u\cdot v$ es un escalar y $w$ es un vector; no se puede sumar un número con un vector. **Sin sentido.**

**c)** $\alpha\cdot(u+v)$, con $\alpha\in\mathbb{R}$: a diferencia de las anteriores, **esta expresión sí tiene sentido**: es el escalar $\alpha$ multiplicando al vector $u+v$, y da como resultado un vector. (Es la excepción entre las tres: multiplicación escalar-vector siempre está bien definida.)

### Ejercicio 28 — Producto vectorial

$u=(2,-1,3)$, $v=(0,1,7)$, $w=(1,4,5)$.

**a)** $v\times w=(1\cdot5-7\cdot4,\ 7\cdot1-0\cdot5,\ 0\cdot4-1\cdot1)=(-23,\,7,\,-1)$.

**b)** $u\times(v\times w)$. Usando $a\times(b\times c)=b(a\cdot c)-c(a\cdot b)$:
$u\cdot w=13$, $u\cdot v=20$.
$$u\times(v\times w)=13v-20w=(0,13,91)-(20,80,100)=(-20,\,-67,\,-9)$$

**c)** $(u\times v)\times w$. Primero $u\times v=(-10,-14,2)$. Usando $(a\times b)\times c=b(a\cdot c)-a(b\cdot c)$:
$u\cdot w=13$, $v\cdot w=39$.
$$(u\times v)\times w=13v-39u=(0,13,91)-(78,-39,117)=(-78,\,52,\,-26)$$

**d)** $u\times(v-2w)$. $v-2w=(-2,-7,-3)$.
$$u\times(v-2w)=\big((-1)(-3)-3(-7),\ 3(-2)-2(-3),\ 2(-7)-(-1)(-2)\big)=(24,\,0,\,-16)$$

### Ejercicio 29 — Vector ortogonal a dos dados

$u=(-7,3,1)$, $v=(2,0,4)$. Un vector ortogonal a ambos es $u\times v$:
$$u\times v=(3\cdot4-1\cdot0,\ 1\cdot2-(-7)\cdot4,\ (-7)\cdot0-3\cdot2)=(12,\,30,\,-6)$$

$$\boxed{w=(12,30,-6)\ \sim\ (2,5,-1)}$$

### Ejercicio 30 — Resolver $u\times y=v$

$u=(-1,3,2)$, $v=(1,1,-1)$.

Condición de compatibilidad: $u\cdot v=-1+3-2=0$ ✓ (necesaria, ya que $u\times y$ siempre es $\perp u$).

Una solución particular ortogonal a $u$ es $y_0=\dfrac{v\times u}{\|u\|^2}$ (se verifica que $u\times y_0=v$ usando $u\times(v\times u)=v\|u\|^2-u(u\cdot v)=v\|u\|^2$).

$$v\times u=(1\cdot2-(-1)\cdot3,\ (-1)(-1)-1\cdot2,\ 1\cdot3-1\cdot(-1))=(5,\,-1,\,4)\qquad \|u\|^2=1+9+4=14$$

$$y_0=\left(\frac{5}{14},\ -\frac{1}{14},\ \frac{2}{7}\right)$$

La solución general se obtiene sumando cualquier múltiplo de $u$ (que está en el núcleo de $y\mapsto u\times y$):

$$\boxed{y=\left(\frac{5}{14}-t,\ -\frac{1}{14}+3t,\ \frac{2}{7}+2t\right),\quad t\in\mathbb{R}}$$

(Verificación con $t=0$: $u\times y_0=(1,1,-1)=v$ ✓.)
