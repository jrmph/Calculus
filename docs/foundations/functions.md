# Functions

Functions are the fundamental building blocks of calculus. A solid understanding of functions is essential for success in calculus.

## What is a Function?

A function is a rule that assigns exactly one output to each input. We typically denote functions using letters like $f$, $g$, or $h$, and write:

$f(x) = y$

Where:
- $x$ is the input (independent variable)
- $y$ is the output (dependent variable)
- $f$ is the function (the rule that transforms $x$ into $y$)

## Function Notation

Function notation $f(x)$ is read as "f of x" and represents the output value of the function $f$ when the input is $x$.

For example, if $f(x) = x^2 + 3x + 2$, then:
- $f(1) = 1^2 + 3(1) + 2 = 1 + 3 + 2 = 6$
- $f(0) = 0^2 + 3(0) + 2 = 0 + 0 + 2 = 2$
- $f(-2) = (-2)^2 + 3(-2) + 2 = 4 - 6 + 2 = 0$

## Types of Functions

### 1. Linear Functions

A linear function has the form $f(x) = mx + b$ where $m$ is the slope and $b$ is the y-intercept.

Example: $f(x) = 3x + 4$

### 2. Polynomial Functions

Polynomial functions have the form $f(x) = a_nx^n + a_{n-1}x^{n-1} + \ldots + a_1x + a_0$

Examples:
- Quadratic: $f(x) = 2x^2 - 3x + 1$
- Cubic: $f(x) = x^3 - 4x^2 + 2$

### 3. Rational Functions

Rational functions are ratios of polynomials: $f(x) = \frac{P(x)}{Q(x)}$

Example: $f(x) = \frac{x^2 - 1}{x - 3}$

### 4. Exponential Functions

Exponential functions have the form $f(x) = a^x$ where $a > 0$ and $a \neq 1$.

Example: $f(x) = 2^x$

### 5. Logarithmic Functions

Logarithmic functions are the inverse of exponential functions: $f(x) = \log_a(x)$

Example: $f(x) = \log_{10}(x)$ or $f(x) = \ln(x)$ (natural logarithm, base $e$)

### 6. Trigonometric Functions

The six basic trigonometric functions: sine, cosine, tangent, cosecant, secant, and cotangent.

Example: $f(x) = \sin(x)$ or $f(x) = \cos(x)$

## Function Operations

Functions can be combined through several operations:

### 1. Addition and Subtraction

$(f + g)(x) = f(x) + g(x)$  
$(f - g)(x) = f(x) - g(x)$

### 2. Multiplication and Division

$(f \cdot g)(x) = f(x) \cdot g(x)$  
$(\frac{f}{g})(x) = \frac{f(x)}{g(x)}$ (where $g(x) \neq 0$)

### 3. Composition

$(f \circ g)(x) = f(g(x))$

Example: If $f(x) = x^2$ and $g(x) = x+3$, then:  
$(f \circ g)(x) = f(g(x)) = f(x+3) = (x+3)^2 = x^2 + 6x + 9$

## Function Characteristics

### 1. Domain and Range

- **Domain**: The set of all possible input values ($x$)
- **Range**: The set of all possible output values ($y$ or $f(x)$)

### 2. Even and Odd Functions

- **Even function**: $f(-x) = f(x)$ (symmetric about the y-axis)
- **Odd function**: $f(-x) = -f(x)$ (symmetric about the origin)

### 3. Increasing and Decreasing Functions

- **Increasing**: $f(a) < f(b)$ whenever $a < b$
- **Decreasing**: $f(a) > f(b)$ whenever $a < b$

### 4. One-to-One Functions

A function is one-to-one if each output corresponds to exactly one input.

### 5. Inverse Functions

If a function $f$ is one-to-one, it has an inverse function $f^{-1}$ such that:
- $f^{-1}(f(x)) = x$ for every $x$ in the domain of $f$
- $f(f^{-1}(y)) = y$ for every $y$ in the range of $f$

## Why Functions Matter in Calculus

In calculus, we study how functions change and behave. Specifically:

1. **Limits** examine the behavior of functions as inputs approach certain values
2. **Derivatives** measure the rate of change of functions
3. **Integrals** accumulate the values of functions over intervals

Understanding functions thoroughly is therefore essential before diving deeper into calculus concepts.

## Practice Problems

1. Find the domain of $f(x) = \frac{1}{x^2 - 4}$
2. Determine if $f(x) = x^3 - x$ is even, odd, or neither
3. Find $(f \circ g)(x)$ if $f(x) = 2x + 1$ and $g(x) = x^2 - 3$
4. Find the inverse of $f(x) = 3x - 5$

### Solutions

1. Domain: All real numbers except $x = \pm 2$ (where the denominator equals zero)
2. $f(-x) = (-x)^3 - (-x) = -x^3 + x = -(x^3 - x) = -f(x)$, so $f$ is an odd function
3. $(f \circ g)(x) = f(g(x)) = f(x^2 - 3) = 2(x^2 - 3) + 1 = 2x^2 - 6 + 1 = 2x^2 - 5$
4. $y = 3x - 5 \implies x = \frac{y + 5}{3} \implies f^{-1}(x) = \frac{x + 5}{3}$