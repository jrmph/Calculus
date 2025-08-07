# Product Rule

The product rule is a formula used to find the derivative of a product of two differentiable functions. It is one of the fundamental differentiation rules in calculus.

## The Rule

If $f(x)$ and $g(x)$ are both differentiable functions, then the derivative of their product is:

$$\frac{d}{dx}[f(x) \cdot g(x)] = f(x) \cdot \frac{d}{dx}[g(x)] + g(x) \cdot \frac{d}{dx}[f(x)]$$

In Leibniz notation:

$$\frac{d}{dx}(uv) = u\frac{dv}{dx} + v\frac{du}{dx}$$

where $u = f(x)$ and $v = g(x)$.

## Intuitive Understanding

The product rule can be understood intuitively by thinking about how the product changes:

1. When $f(x)$ changes (while $g(x)$ stays fixed)
2. When $g(x)$ changes (while $f(x)$ stays fixed)

The total change is the sum of these two effects.

## Proof of the Product Rule

We can derive the product rule using the definition of the derivative:

$$\frac{d}{dx}[f(x)g(x)] = \lim_{h \to 0} \frac{f(x+h)g(x+h) - f(x)g(x)}{h}$$

To manipulate this expression, we'll add and subtract $f(x+h)g(x)$ in the numerator:

$$\frac{d}{dx}[f(x)g(x)] = \lim_{h \to 0} \frac{f(x+h)g(x+h) - f(x+h)g(x) + f(x+h)g(x) - f(x)g(x)}{h}$$

Rearranging the terms:

$$\frac{d}{dx}[f(x)g(x)] = \lim_{h \to 0} \left[ \frac{f(x+h)[g(x+h) - g(x)]}{h} + \frac{g(x)[f(x+h) - f(x)]}{h} \right]$$

As $h \to 0$, we know that $f(x+h) \to f(x)$ (by the continuity of $f$), so:

$$\frac{d}{dx}[f(x)g(x)] = f(x) \cdot \lim_{h \to 0} \frac{g(x+h) - g(x)}{h} + g(x) \cdot \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

These limits are precisely the definitions of the derivatives of $g$ and $f$:

$$\frac{d}{dx}[f(x)g(x)] = f(x) \cdot \frac{d}{dx}[g(x)] + g(x) \cdot \frac{d}{dx}[f(x)]$$

## Mnemonic Device

A popular mnemonic for remembering the product rule is:
- "The derivative of a product is the first function times the derivative of the second, plus the second function times the derivative of the first."

Alternatively: "First times the derivative of second, plus second times the derivative of first."

## Examples

### Example 1: Basic Product Rule

Find the derivative of $f(x) = x^3 \sin(x)$.

Solution:
Let $u = x^3$ and $v = \sin(x)$
$u' = 3x^2$ and $v' = \cos(x)$

Using the product rule:
$f'(x) = u \cdot v' + v \cdot u'$
$f'(x) = x^3 \cdot \cos(x) + \sin(x) \cdot 3x^2$
$f'(x) = x^3\cos(x) + 3x^2\sin(x)$
$f'(x) = x^2(x\cos(x) + 3\sin(x))$

### Example 2: Products with Exponentials

Find the derivative of $g(x) = xe^x$.

Solution:
Let $u = x$ and $v = e^x$
$u' = 1$ and $v' = e^x$

Using the product rule:
$g'(x) = u \cdot v' + v \cdot u'$
$g'(x) = x \cdot e^x + e^x \cdot 1$
$g'(x) = xe^x + e^x$
$g'(x) = e^x(x + 1)$

### Example 3: Products with Logarithms

Find the derivative of $h(x) = x^2\ln(x)$, for $x > 0$.

Solution:
Let $u = x^2$ and $v = \ln(x)$
$u' = 2x$ and $v' = \frac{1}{x}$

Using the product rule:
$h'(x) = u \cdot v' + v \cdot u'$
$h'(x) = x^2 \cdot \frac{1}{x} + \ln(x) \cdot 2x$
$h'(x) = x + 2x\ln(x)$
$h'(x) = x(1 + 2\ln(x))$

### Example 4: Product of Three Functions

For the product of three functions, we can apply the product rule twice:

Find the derivative of $f(x) = x^2 \sin(x) \ln(x)$.

Solution:
We can view this as the product of $x^2\sin(x)$ and $\ln(x)$.

First, let's find the derivative of $x^2\sin(x)$ using the product rule:
Let $u = x^2$ and $v = \sin(x)$
$u' = 2x$ and $v' = \cos(x)$

$\frac{d}{dx}[x^2\sin(x)] = x^2\cos(x) + \sin(x) \cdot 2x = x^2\cos(x) + 2x\sin(x)$

Now, let's use the product rule again with $p(x) = x^2\sin(x)$ and $q(x) = \ln(x)$:
$p'(x) = x^2\cos(x) + 2x\sin(x)$ and $q'(x) = \frac{1}{x}$

$f'(x) = p(x) \cdot q'(x) + q(x) \cdot p'(x)$
$f'(x) = x^2\sin(x) \cdot \frac{1}{x} + \ln(x) \cdot (x^2\cos(x) + 2x\sin(x))$
$f'(x) = x\sin(x) + \ln(x)x^2\cos(x) + 2x\ln(x)\sin(x)$
$f'(x) = x\sin(x) + x\ln(x)(x\cos(x) + 2\sin(x))$

## Common Mistakes

1. **Forgetting a term**: The most common mistake is to forget one of the terms in the product rule formula.

2. **Incorrect differentiation**: Make sure to correctly differentiate each function separately before applying the product rule.

3. **Chain rule confusion**: When one of the functions is a composition, remember to apply the chain rule to differentiate it correctly.

## Products with More Than Two Functions

For a product of three functions $f(x) \cdot g(x) \cdot h(x)$, you can use the product rule repeatedly:

1. First, consider $(f(x) \cdot g(x)) \cdot h(x)$ and apply the product rule
2. Then, use the product rule to find the derivative of $f(x) \cdot g(x)$

Alternatively, for $n$ functions, the derivative of their product follows this pattern:

$$\frac{d}{dx}[f_1(x)f_2(x)...f_n(x)] = \sum_{i=1}^n f_1(x)f_2(x)...f'_i(x)...f_n(x)$$

This means you take the derivative of each function in turn while keeping the others unchanged, and then sum all these terms.

## Application: Leibniz's Rule for Derivatives of Integrals

The product rule leads to Leibniz's rule for differentiating an integral with variable limits:

$$\frac{d}{dx}\left[\int_{a(x)}^{b(x)} f(t) \, dt\right] = f(b(x)) \cdot b'(x) - f(a(x)) \cdot a'(x) + \int_{a(x)}^{b(x)} \frac{\partial f}{\partial x}(t) \, dt$$

## Practice Problems

1. Find the derivative of $f(x) = (x^2 + 3x) \cdot (4x - 1)$
2. Differentiate $g(x) = e^x \cdot \cos(x)$
3. Find the derivative of $h(x) = x \cdot \ln(x) \cdot \sin(x)$
4. Calculate $\frac{d}{dx}[x^3 \cdot (2x+1)^4]$

### Solutions

1. $f'(x) = (x^2 + 3x) \cdot 4 + (4x - 1) \cdot (2x + 3) = 4x^2 + 12x + (4x-1)(2x+3) = 4x^2 + 12x + 8x^2 + 12x - 2x - 3 = 12x^2 + 22x - 3$

2. $g'(x) = e^x \cdot \cos(x) + e^x \cdot (-\sin(x)) = e^x \cdot (\cos(x) - \sin(x))$

3. First, find the derivative of $x \cdot \ln(x)$:
   $\frac{d}{dx}(x \cdot \ln(x)) = x \cdot \frac{1}{x} + \ln(x) \cdot 1 = 1 + \ln(x)$
   
   Now, let $p(x) = x \cdot \ln(x)$ and $q(x) = \sin(x)$:
   $h'(x) = (1 + \ln(x)) \cdot \sin(x) + x \cdot \ln(x) \cdot \cos(x)$
   $h'(x) = \sin(x) + \ln(x)\sin(x) + x\ln(x)\cos(x)$
   $h'(x) = \sin(x)(1 + \ln(x)) + x\ln(x)\cos(x)$

4. $\frac{d}{dx}[x^3 \cdot (2x+1)^4] = x^3 \cdot 4(2x+1)^3 \cdot 2 + (2x+1)^4 \cdot 3x^2$
   $= 8x^3(2x+1)^3 + 3x^2(2x+1)^4$
   $= x^2(2x+1)^3(8x + 3(2x+1))$
   $= x^2(2x+1)^3(8x + 6x + 3)$
   $= x^2(2x+1)^3(14x + 3)$