# Método de la Bisección

El método de la bisección es un algoritmo numérico utilizado para encontrar una raíz de una función continua \( f(x) \) en un intervalo \([a, b]\), siempre que se cumpla que \( f(a) \cdot f(b) < 0 \) (es decir, la función cambia de signo en el intervalo, garantizando la existencia de al menos una raíz).

## Pasos del Método

1. **Definir el intervalo inicial \([a, b]\):**
   - Verifica que \( f(a) \cdot f(b) < 0 \).
   - Esto asegura que existe al menos una raíz en el intervalo (por el Teorema del Valor Intermedio).

2. **Calcular el punto medio:**
   - La fórmula del punto medio es:
     \[
     c = \frac{a + b}{2}
     \]
   - Aquí, \( c \) es el punto medio del intervalo.

3. **Evaluar la función en el punto medio:**
   - Si \( f(c) = 0 \), entonces \( c \) es la raíz exacta.
   - Si no, determina en qué subintervalo está la raíz:
     - Si \( f(a) \cdot f(c) < 0 \), entonces la raíz está en \([a, c]\).
     - Si \( f(c) \cdot f(b) < 0 \), entonces la raíz está en \([c, b]\).

4. **Actualizar el intervalo y repetir:**
   - Continúa dividiendo el intervalo y evaluando el punto medio hasta que el intervalo sea suficientemente pequeño o \( f(c) \) esté cerca de cero.

---

## Ventajas

- Es un método sencillo y fácil de implementar.
- Siempre converge si se cumple la condición inicial \( f(a) \cdot f(b) < 0 \).

## Desventajas

- La convergencia es lenta (lineal), ya que el intervalo se reduce a la mitad en cada iteración.


