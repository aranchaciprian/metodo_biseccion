Método de la Bisección
El método de la bisección es un algoritmo numérico utilizado para encontrar una raíz de una función continua 𝑓(𝑥) en un intervalo [𝑎,𝑏], siempre que se cumpla que 𝑓(𝑎)⋅𝑓(𝑏)<0
(es decir, la función cambia de signo en el intervalo, garantizando la existencia de al menos una raíz).

Pasos del Método:
1. Definir el intervalo inicial [𝑎,𝑏]:
    - Verifica que 𝑓(𝑎) y 𝑓(𝑏) tengan signos opuestos 𝑓(𝑎)⋅𝑓(𝑏)<0.
Esto asegura que existe al menos una raíz en el intervalo (por el Teorema del Valor Intermedio).
Calcular el punto medio:

𝑐
=
𝑎
+
𝑏
2
c= 
2
a+b
​
 , donde 
𝑐
c es el punto medio del intervalo.
Evaluar la función en el punto medio:

Si 
𝑓
(
𝑐
)
=
0
f(c)=0, 
𝑐
c es la raíz exacta.
Si no, determina en qué subintervalo 
[
𝑎
,
𝑐
]
[a,c] o 
[
𝑐
,
𝑏
]
[c,b] se encuentra la raíz:
Si 
𝑓
(
𝑐
)
⋅
𝑓
(
𝑎
)
<
0
f(c)⋅f(a)<0, la raíz está en 
[
𝑎
,
𝑐
]
[a,c].
Si 
𝑓
(
𝑐
)
⋅
𝑓
(
𝑏
)
<
0
f(c)⋅f(b)<0, la raíz está en 
[
𝑐
,
𝑏
]
[c,b].
Actualizar el intervalo:

Sustituye 
𝑎
a o 
𝑏
b con 
𝑐
c según el paso anterior y repite el proceso.
Detenerse:

El algoritmo se detiene cuando el intervalo es suficientemente pequeño (según una tolerancia predefinida) o cuando 
𝑓
(
𝑐
)
f(c) está cerca de cero.
Ventajas:
Es un método sencillo de implementar.
Siempre converge si se cumplen las condiciones iniciales.
Desventajas:
Convergencia lenta (reduce el intervalo a la mitad en cada iteración).
