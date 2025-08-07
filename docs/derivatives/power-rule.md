# Power Rule

The Power Rule is one of the most fundamental differentiation rules in calculus. It provides a straightforward way to find the derivative of any function that can be expressed as a power of the variable.

## The Rule

For any real number $n$, the derivative of $x^n$ with respect to $x$ is:

$$\frac{d}{dx}(x^n) = nx^{n-1}$$

This rule states that to differentiate $x^n$:
1. Multiply by the exponent $n$
2. Reduce the exponent by 1

## Proof of the Power Rule

### For Integer Powers

We can prove the power rule for positive integers using the definition of the derivative:

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

Let $f(x) = x^n$ where $n$ is a positive integer.

$$f'(x) = \lim_{h \to 0} \frac{(x+h)^n - x^n}{h}$$

Using the binomial theorem, we can expand $(x+h)^n$:

$$(x+h)^n = x^n + nx^{n-1}h + \frac{n(n-1)}{2}x^{n-2}h^2 + \ldots + h^n$$

Substituting this into our derivative expression:

$$f'(x) = \lim_{h \to 0} \frac{x^n + nx^{n-1}h + \frac{n(n-1)}{2}x^{n-2}h^2 + \ldots + h^n - x^n}{h}$$

$$f'(x) = \lim_{h \to 0} \frac{nx^{n-1}h + \frac{n(n-1)}{2}x^{n-2}h^2 + \ldots + h^n}{h}$$

$$f'(x) = \lim_{h \to 0} \left(nx^{n-1} + \frac{n(n-1)}{2}x^{n-2}h + \ldots + h^{n-1}\right)$$

As $h \to 0$, all terms with $h$ approach zero, leaving:

$$f'(x) = nx^{n-1}$$

### For Rational Powers

For rational powers (like $x^{1/2}$ or $x^{-3/4}$), the proof requires more advanced techniques using the chain rule, but the result is the same.

## Examples

### Example 1: Basic Powers

Find the derivatives of:
- $f(x) = x^3$
- $g(x) = x^7$
- $h(x) = x$

Solutions:
- $f'(x) = 3x^2$
- $g'(x) = 7x^6$
- $h'(x) = 1x^0 = 1$

### Example 2: Negative Powers

Find the derivatives of:
- $f(x) = x^{-1}$
- $g(x) = x^{-4}$

Solutions:
- $f'(x) = -1x^{-2} = -\frac{1}{x^2}$
- $g'(x) = -4x^{-5} = -\frac{4}{x^5}$

### Example 3: Fractional Powers

Find the derivatives of:
- $f(x) = x^{1/2}$ (or $\sqrt{x}$)
- $g(x) = x^{3/2}$ (or $x\sqrt{x}$)
- $h(x) = x^{-1/2}$ (or $\frac{1}{\sqrt{x}}$)

Solutions:
- $f'(x) = \frac{1}{2}x^{-1/2} = \frac{1}{2\sqrt{x}}$
- $g'(x) = \frac{3}{2}x^{1/2} = \frac{3\sqrt{x}}{2}$
- $h'(x) = -\frac{1}{2}x^{-3/2} = -\frac{1}{2x^{3/2}} = -\frac{1}{2x\sqrt{x}}$

### Example 4: Power Rule with Coefficients

Find the derivatives of:
- $f(x) = 5x^3$
- $g(x) = -2x^{-3}$

Solutions:
- $f'(x) = 5 \cdot 3x^2 = 15x^2$
- $g'(x) = -2 \cdot (-3)x^{-4} = 6x^{-4} = \frac{6}{x^4}$

## Power Rule with the Chain Rule

When dealing with composite functions of the form $[g(x)]^n$, we need to combine the power rule with the chain rule:

$$\frac{d}{dx}[g(x)]^n = n[g(x)]^{n-1} \cdot g'(x)$$

### Example 5: Power Rule with Chain Rule

Find the derivatives of:
- $f(x) = (3x+2)^4$
- $g(x) = (x^2+1)^{1/2}$ (or $\sqrt{x^2+1}$)

Solutions:
- $f'(x) = 4(3x+2)^3 \cdot 3 = 12(3x+2)^3$
- $g'(x) = \frac{1}{2}(x^2+1)^{-1/2} \cdot 2x = \frac{x}{\sqrt{x^2+1}}$

## Common Functions Using the Power Rule

Many common functions can be differentiated using the power rule:

1. Constant function: $\frac{d}{dx}(c) = \frac{d}{dx}(cx^0) = c \cdot 0 \cdot x^{-1} = 0$

2. Identity function: $\frac{d}{dx}(x) = \frac{d}{dx}(x^1) = 1 \cdot x^0 = 1$

3. Reciprocal function: $\frac{d}{dx}(\frac{1}{x}) = \frac{d}{dx}(x^{-1}) = -1 \cdot x^{-2} = -\frac{1}{x^2}$

## Applications

### Finding Equations of Tangent Lines

The power rule is often used to find the equation of the tangent line to a curve at a specific point.

Example: Find the equation of the tangent line to the curve $f(x) = x^3$ at the point $(2, 8)$.

1. Calculate $f'(x) = 3x^2$
2. Evaluate $f'(2) = 3(2)^2 = 12$
3. Use point-slope form: $y - 8 = 12(x - 2)$
4. Simplify to slope-intercept form: $y = 12x - 16$

### Velocity and Acceleration

The power rule is useful in physics for analyzing motion.

Example: If an object's position function is $s(t) = t^3 - 6t^2 + 9t$, find its velocity and acceleration functions.

1. Velocity is the derivative of position: $v(t) = s'(t) = 3t^2 - 12t + 9$
2. Acceleration is the derivative of velocity: $a(t) = v'(t) = 6t - 12$

### Optimization Problems

The power rule helps solve optimization problems by finding critical points.

Example: Find the dimensions of a rectangle with perimeter 100 that has maximum area.

1. Let $x$ and $y$ be the length and width
2. The perimeter equation gives: $2x + 2y = 100$, so $y = 50 - x$
3. The area is $A = xy = x(50-x) = 50x - x^2$
4. Find $\frac{dA}{dx} = 50 - 2x$
5. Set $\frac{dA}{dx} = 0 \implies 50 - 2x = 0 \implies x = 25$
6. Thus $y = 25$ as well, so the rectangle is a square with sides of length 25

## Practice Problems

1. Find the derivative of $f(x) = x^4 - 3x^2 + 5$
2. Differentiate $g(x) = \frac{2}{x^3}$
3. Find the derivative of $h(x) = (2x+1)^5$
4. Calculate the derivative of $j(x) = \sqrt[3]{x}$
5. Find $\frac{d}{dx}[\sqrt{4x^2+9}]$

### Solutions

1. $f'(x) = 4x^3 - 6x$
2. $g'(x) = \frac{d}{dx}(2x^{-3}) = -6x^{-4} = -\frac{6}{x^4}$
3. $h'(x) = 5(2x+1)^4 \cdot 2 = 10(2x+1)^4$
4. $j'(x) = \frac{d}{dx}(x^{1/3}) = \frac{1}{3}x^{-2/3} = \frac{1}{3x^{2/3}} = \frac{1}{3\sqrt[3]{x^2}}$
5. $\frac{d}{dx}[\sqrt{4x^2+9}] = \frac{d}{dx}[(4x^2+9)^{1/2}] = \frac{1}{2}(4x^2+9)^{-1/2} \cdot 8x = \frac{4x}{\sqrt{4x^2+9}}$