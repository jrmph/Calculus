# Introduction to Integration

Integration is the second fundamental concept of calculus (alongside differentiation). While differentiation deals with rates of change, integration deals with accumulation and is often used to find areas, volumes, and solutions to differential equations.

## The Problem of Area

One of the motivating problems for integration is finding the area under a curve. For simple shapes like rectangles and triangles, area formulas are well-known. But how do we find the area under an arbitrary curve?

The key idea is to approximate the area using simple shapes (like rectangles) and then take the limit as the approximation becomes increasingly accurate.

## Riemann Sums

A Riemann sum is a way to approximate the area under a curve by dividing the interval into subintervals and constructing rectangles.

Given a function $f(x)$ on an interval $[a, b]$, we:
1. Divide the interval into $n$ equal subintervals, each of width $\Delta x = \frac{b-a}{n}$
2. For each subinterval, choose a point $x_i^*$ and calculate the value $f(x_i^*)$
3. Construct a rectangle with height $f(x_i^*)$ and width $\Delta x$
4. Sum the areas of all rectangles: $\sum_{i=1}^{n} f(x_i^*) \Delta x$

As $n$ approaches infinity (or equivalently, as $\Delta x$ approaches 0), this sum approaches the definite integral.

### Types of Riemann Sums

1. **Left Riemann Sum**: $x_i^*$ is the left endpoint of each subinterval
2. **Right Riemann Sum**: $x_i^*$ is the right endpoint of each subinterval
3. **Midpoint Riemann Sum**: $x_i^*$ is the midpoint of each subinterval

## The Definite Integral

The definite integral of $f(x)$ from $a$ to $b$ is defined as the limit of the Riemann sum as the number of subintervals approaches infinity:

$$\int_a^b f(x) \, dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*) \Delta x$$

This is denoted as $\int_a^b f(x) \, dx$ and is read as "the integral of $f(x)$ from $a$ to $b$ with respect to $x$."

### Properties of the Definite Integral

1. $\int_a^b c \cdot f(x) \, dx = c \cdot \int_a^b f(x) \, dx$ (Constant Multiple Rule)
2. $\int_a^b [f(x) + g(x)] \, dx = \int_a^b f(x) \, dx + \int_a^b g(x) \, dx$ (Sum Rule)
3. $\int_a^b [f(x) - g(x)] \, dx = \int_a^b f(x) \, dx - \int_a^b g(x) \, dx$ (Difference Rule)
4. $\int_a^b f(x) \, dx = -\int_b^a f(x) \, dx$ (Reversal of Limits)
5. $\int_a^a f(x) \, dx = 0$ (Zero Width)
6. $\int_a^c f(x) \, dx + \int_c^b f(x) \, dx = \int_a^b f(x) \, dx$ (Additivity)

### Interpretations of the Definite Integral

1. **Area under a curve**: When $f(x) \geq 0$ over $[a, b]$, the integral gives the area under the curve
2. **Signed area**: When $f(x)$ changes sign over $[a, b]$, the integral gives the net area (positive areas minus negative areas)
3. **Accumulation**: The integral represents the accumulation of a quantity whose rate of change is given by $f(x)$
4. **Average value**: The average value of $f(x)$ over $[a, b]$ is $\frac{1}{b-a} \int_a^b f(x) \, dx$

## The Fundamental Theorem of Calculus

The Fundamental Theorem of Calculus is a profound result that connects differentiation and integration, showing that they are inverse operations.

### Part 1: Differentiation of an Integral

If we define a function $F(x) = \int_a^x f(t) \, dt$, where $f$ is continuous on $[a, b]$ and $x$ is in $[a, b]$, then $F$ is differentiable on $(a, b)$ and $F'(x) = f(x)$.

In other words, the derivative of the integral of a function gives back the original function.

### Part 2: Integration as Antidifferentiation

If $f$ is continuous on $[a, b]$ and $F$ is any antiderivative of $f$ on $[a, b]$ (i.e., $F'(x) = f(x)$ for all $x$ in $[a, b]$), then:

$$\int_a^b f(x) \, dx = F(b) - F(a)$$

This is often written as $\int_a^b f(x) \, dx = [F(x)]_a^b$ where $[F(x)]_a^b = F(b) - F(a)$.

## The Indefinite Integral

An indefinite integral, denoted $\int f(x) \, dx$, represents the family of all antiderivatives of $f$.

If $F(x)$ is an antiderivative of $f(x)$, then:

$$\int f(x) \, dx = F(x) + C$$

where $C$ is an arbitrary constant (the "constant of integration").

For example, $\int x^2 \, dx = \frac{x^3}{3} + C$.

## Basic Integration Rules

1. $\int x^n \, dx = \frac{x^{n+1}}{n+1} + C$ for $n \neq -1$
2. $\int e^x \, dx = e^x + C$
3. $\int \frac{1}{x} \, dx = \ln|x| + C$
4. $\int \sin(x) \, dx = -\cos(x) + C$
5. $\int \cos(x) \, dx = \sin(x) + C$
6. $\int \sec^2(x) \, dx = \tan(x) + C$

## Integration Techniques

While the basic rules cover many simple functions, more complex integrations require specialized techniques:

1. **Substitution Method** (also called u-substitution): Used when an integral has a function and its derivative
2. **Integration by Parts**: A technique based on the product rule for differentiation
3. **Partial Fractions**: Used for rational functions (ratios of polynomials)
4. **Trigonometric Substitutions**: Useful for certain expressions involving square roots
5. **Numerical Integration**: Approximation methods like the Trapezoidal Rule and Simpson's Rule

These techniques will be covered in depth in subsequent sections.

## Example: Finding a Definite Integral

Let's evaluate $\int_0^3 x^2 \, dx$.

Solution:

1. Find an antiderivative: $\int x^2 \, dx = \frac{x^3}{3} + C$
2. Apply the Fundamental Theorem of Calculus:
   $\int_0^3 x^2 \, dx = [\frac{x^3}{3}]_0^3 = \frac{3^3}{3} - \frac{0^3}{3} = 9 - 0 = 9$

So, $\int_0^3 x^2 \, dx = 9$, which also represents the area under the curve $f(x) = x^2$ from $x = 0$ to $x = 3$.

## Practice Problems

1. Evaluate $\int_1^4 (2x + 3) \, dx$
2. Find the indefinite integral $\int \sin(3x) \, dx$
3. Calculate the average value of $f(x) = x^3$ over the interval $[0, 2]$
4. Find the area between the curve $y = x^2$ and the x-axis over the interval $[0, 3]$

### Solutions

1. $\int_1^4 (2x + 3) \, dx = [x^2 + 3x]_1^4 = (16 + 12) - (1 + 3) = 28 - 4 = 24$

2. $\int \sin(3x) \, dx = -\frac{1}{3}\cos(3x) + C$
   (Using substitution with $u = 3x$)

3. Average value = $\frac{1}{2-0} \int_0^2 x^3 \, dx = \frac{1}{2} \cdot [\frac{x^4}{4}]_0^2 = \frac{1}{2} \cdot \frac{16}{4} = 2$

4. Area = $\int_0^3 x^2 \, dx = [\frac{x^3}{3}]_0^3 = \frac{27}{3} - 0 = 9$ square units