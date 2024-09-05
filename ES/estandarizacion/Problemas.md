# Lista de Problemas

Este apartado contiene una lista de problemas relacionados con el tema específico. Cada problema debe estar correctamente numerado y presentado de forma clara, seguido de un índice para facilitar la navegación.

---

## Índice de Problemas
1. [Problema 1: Integración por partes](#problema-1)
2. [Problema 2: Ecuaciones diferenciales](#problema-2)
3. [Problema 3: Series de Fourier](#problema-3)
4. [Problema 4: Optimización de funciones](#problema-4)

---

# Problemas sin Resolver

Aquí se listan los problemas que el lector debe intentar resolver antes de consultar las soluciones. Los problemas pueden incluir ecuaciones, gráficos o escenarios que deben analizarse.

### Problema 1: Integración por partes {#problema-1}
Calcular la siguiente integral aplicando la técnica de integración por partes:

$$
\int x e^x \, dx
$$

### Problema 2: Ecuaciones diferenciales {#problema-2}
Resolver la siguiente ecuación diferencial de primer orden:

$$
\frac{dy}{dx} + y = e^x
$$

### Problema 3: Series de Fourier {#problema-3}
Determinar los primeros tres términos de la serie de Fourier para la función:

$$
f(x) = x^2 \quad \text{en el intervalo} \, [-\pi, \pi]
$$

### Problema 4: Optimización de funciones {#problema-4}
Hallar los puntos críticos de la función:

$$
f(x, y) = x^2 + y^2 - 4x - 6y + 13
$$

> **Nota:** Cada problema debe estar correctamente formulado y acompañado de cualquier información relevante que el lector pueda necesitar para abordarlo. Evita dejar información ambigua o incompleta.

---

# Soluciones y Desarrollos de los Problemas

A continuación, se presentan las soluciones detalladas de los problemas previamente planteados. Cada solución debe incluir una explicación paso a paso y, si es necesario, notas del autor que clarifiquen conceptos clave o justifiquen las decisiones tomadas en el desarrollo del ejercicio.

---

## Solución del Problema 1: Integración por partes
**Problema:** Calcular la siguiente integral:

$$
\int x e^x \, dx
$$

### Desarrollo:

Para resolver esta integral, utilizamos el método de **integración por partes**, donde:

- $u = x$
- $dv = e^x \, dx$

Aplicando la fórmula:

$$
\int u \, dv = u v - \int v \, du
$$

1. Derivamos $u$:  
   $$
   du = dx
   $$
2. Integramos $dv$:  
   $$
   v = e^x
   $$
3. Sustituimos en la fórmula de integración por partes:  
   $$
   \int x e^x \, dx = x e^x - \int e^x \, dx
   $$
4. Resolvemos la integral restante:  
   $$
   \int e^x \, dx = e^x
   $$
5. La solución final es:  
   $$
   \int x e^x \, dx = x e^x - e^x + C
   $$

> **Nota del autor:** La técnica de integración por partes es útil cuando tenemos un producto de funciones donde una es fácilmente integrable (como $e^x$) y la otra tiene una derivada simple (como $x$).

---

## Solución del Problema 2: Ecuaciones diferenciales
**Problema:** Resolver la ecuación diferencial:

$$
\frac{dy}{dx} + y = e^x
$$

### Desarrollo:

Esta es una **ecuación diferencial lineal de primer orden**. Utilizamos el factor integrante $\mu(x) = e^{\int 1 \, dx} = e^x$.

1. Multiplicamos toda la ecuación por $e^x$:  
   $$
   e^x \frac{dy}{dx} + e^x y = e^{2x}
   $$
2. Observamos que el lado izquierdo es la derivada de $y e^x$:  
   $$
   \frac{d}{dx} \left( y e^x \right) = e^{2x}
   $$
3. Integramos ambos lados:  
   $$
   y e^x = \int e^{2x} \, dx = \frac{e^{2x}}{2} + C
   $$
4. Finalmente, despejamos $y$:  
   $$
   y = \frac{e^x}{2} + Ce^{-x}
   $$

> **Nota del autor:** El factor integrante es una técnica estándar para resolver ecuaciones diferenciales lineales de primer orden. Es importante dominar este procedimiento para casos similares.

---

## Solución del Problema 3: Series de Fourier
**Problema:** Determinar los primeros tres términos de la serie de Fourier para la función $f(x) = x^2$ en el intervalo $[-\pi, \pi]$.

### Desarrollo:

1. Calculamos el coeficiente $a_0$:  
   $$
   a_0 = \frac{1}{\pi} \int_{-\pi}^{\pi} x^2 \, dx = \frac{2\pi^2}{3}
   $$
2. Los coeficientes $a_n$ y $b_n$ se calculan a partir de:  
   $$
   a_n = \frac{1}{\pi} \int_{-\pi}^{\pi} x^2 \cos(nx) \, dx
   $$
   $$
   b_n = \frac{1}{\pi} \int_{-\pi}^{\pi} x^2 \sin(nx) \, dx
   $$
   Los primeros tres términos resultantes de estos cálculos son:  
   $$
   f(x) \approx a_0 + a_1 \cos(x) + a_2 \cos(2x)
   $$

> **Nota del autor:** El cálculo de los coeficientes de Fourier puede ser tedioso, pero es esencial para descomponer una función periódica en términos de senos y cosenos. Recomendable verificar los límites de integración cuidadosamente.

---

## Solución del Problema 4: Optimización de funciones
**Problema:** Encontrar los puntos críticos de la función:

$$
f(x, y) = x^2 + y^2 - 4x - 6y + 13
$$

### Desarrollo:

1. Calculamos las derivadas parciales:  
   $$
   \frac{\partial f}{\partial x} = 2x - 4, \quad \frac{\partial f}{\partial y} = 2y - 6
   $$
2. Igualamos a cero para encontrar los puntos críticos:  
   $$
   2x - 4 = 0 \quad \Rightarrow \quad x = 2
   $$
   $$
   2y - 6 = 0 \quad \Rightarrow \quad y = 3
   $$
3. El punto crítico es $(2, 3)$. Evaluamos el valor de la función en ese punto:  
   $$
   f(2, 3) = 2^2 + 3^2 - 4(2) - 6(3) + 13 = -2
   $$

> **Nota del autor:** Al aplicar derivadas parciales para optimización, es importante evaluar también el tipo de punto crítico usando las segundas derivadas. En este caso, el cálculo del determinante de la matriz Hessiana puede confirmar si es un mínimo, máximo o punto de silla.

---

# Consideraciones para el Autor

- **Claridad en la exposición**: Todos los pasos de las soluciones deben explicarse de manera clara y concisa. No asumas que el lector ya sabe cómo se desarrolla cada paso.
  
- **Notas adicionales**: En las notas del autor, incluye recomendaciones, aclaraciones, y posibles errores comunes para ayudar al lector a entender mejor la solución.

- **Formato uniforme**: Asegúrate de que tanto los problemas como las soluciones sigan el mismo formato en todo el documento.

- **Referencias**: Si es necesario, añade referencias a otros temas o lecciones que puedan ayudar a resolver el problema. (pueden ser cualquier contenido de texto o multimedia de la web)
