# Differentiation Rules

While the definition of a derivative can always be used to find the derivative of a function, there are established rules that make differentiation much more efficient. This section covers the main differentiation rules.

## Basic Rules

### 1. Constant Rule

The derivative of a constant is zero:

$$\frac{d}{dx}(c) = 0$$

where $c$ is any constant.

**Example**: $\frac{d}{dx}(5) = 0$

### 2. Power Rule

For any real number $n$:

$$\frac{d}{dx}(x^n) = nx^{n-1}$$

**Examples**:
- $\frac{d}{dx}(x^3) = 3x^2$
- $\frac{d}{dx}(x^{-2}) = -2x^{-3} = -\frac{2}{x^3}$
- $\frac{d}{dx}(\sqrt{x}) = \frac{d}{dx}(x^{1/2}) = \frac{1}{2}x^{-1/2} = \frac{1}{2\sqrt{x}}$

### 3. Constant Multiple Rule

For any constant $c$:

$$\frac{d}{dx}[c \cdot f(x)] = c \cdot \frac{d}{dx}[f(x)]$$

**Example**: $\frac{d}{dx}(3x^2) = 3 \cdot \frac{d}{dx}(x^2) = 3 \cdot 2x = 6x$

### 4. Sum and Difference Rules

For any two differentiable functions $f(x)$ and $g(x)$:

$$\frac{d}{dx}[f(x) + g(x)] = \frac{d}{dx}[f(x)] + \frac{d}{dx}[g(x)]$$

$$\frac{d}{dx}[f(x) - g(x)] = \frac{d}{dx}[f(x)] - \frac{d}{dx}[g(x)]$$

**Example**: $\frac{d}{dx}(x^3 + 2x - 5) = \frac{d}{dx}(x^3) + \frac{d}{dx}(2x) - \frac{d}{dx}(5) = 3x^2 + 2 - 0 = 3x^2 + 2$

## Product Rule

For two differentiable functions $f(x)$ and $g(x)$:

$$\frac{d}{dx}[f(x) \cdot g(x)] = f(x) \cdot \frac{d}{dx}[g(x)] + g(x) \cdot \frac{d}{dx}[f(x)]$$

Mnemonic: The derivative of a product is the "first times the derivative of the second, plus the second times the derivative of the first."

**Example**: Find $\frac{d}{dx}(x^2 \cdot \sin(x))$

Solution:
Let $f(x) = x^2$ and $g(x) = \sin(x)$
$f'(x) = 2x$ and $g'(x) = \cos(x)$

Using the product rule:
$\frac{d}{dx}(x^2 \cdot \sin(x)) = x^2 \cdot \cos(x) + \sin(x) \cdot 2x = x^2\cos(x) + 2x\sin(x)$

## Quotient Rule

For two differentiable functions $f(x)$ and $g(x)$ where $g(x) \neq 0$:

$$\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{g(x) \cdot \frac{d}{dx}[f(x)] - f(x) \cdot \frac{d}{dx}[g(x)]}{[g(x)]^2}$$

Mnemonic: "Low d-high minus high d-low, all over low squared."

**Example**: Find $\frac{d}{dx}\left(\frac{x^2+1}{\sin(x)}\right)$

Solution:
Let $f(x) = x^2+1$ and $g(x) = \sin(x)$
$f'(x) = 2x$ and $g'(x) = \cos(x)$

Using the quotient rule:
$\frac{d}{dx}\left(\frac{x^2+1}{\sin(x)}\right) = \frac{\sin(x) \cdot 2x - (x^2+1) \cdot \cos(x)}{[\sin(x)]^2} = \frac{2x\sin(x) - (x^2+1)\cos(x)}{\sin^2(x)}$

## Chain Rule

The chain rule is used when dealing with composite functions. If $y = f(g(x))$, then:

$$\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$$

where $u = g(x)$. Alternatively, this can be written as:

$$\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$$

**Example**: Find $\frac{d}{dx}[\sin(x^2)]$

Solution:
Let $u = x^2$ and $y = \sin(u)$
$\frac{dy}{du} = \cos(u)$ and $\frac{du}{dx} = 2x$

Using the chain rule:
$\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx} = \cos(u) \cdot 2x = \cos(x^2) \cdot 2x = 2x\cos(x^2)$

## Derivatives of Common Functions

### 1. Exponential Functions

$$\frac{d}{dx}(e^x) = e^x$$

$$\frac{d}{dx}(a^x) = a^x \ln(a)$$

**Example**: $\frac{d}{dx}(2^x) = 2^x \ln(2)$

### 2. Logarithmic Functions

$$\frac{d}{dx}(\ln(x)) = \frac{1}{x}$$

$$\frac{d}{dx}(\log_a(x)) = \frac{1}{x \ln(a)}$$

**Example**: $\frac{d}{dx}(\log_{10}(x)) = \frac{1}{x \ln(10)}$

### 3. Trigonometric Functions

$$\frac{d}{dx}(\sin(x)) = \cos(x)$$

$$\frac{d}{dx}(\cos(x)) = -\sin(x)$$

$$\frac{d}{dx}(\tan(x)) = \sec^2(x)$$

$$\frac{d}{dx}(\cot(x)) = -\csc^2(x)$$

$$\frac{d}{dx}(\sec(x)) = \sec(x)\tan(x)$$

$$\frac{d}{dx}(\csc(x)) = -\csc(x)\cot(x)$$

### 4. Inverse Trigonometric Functions

$$\frac{d}{dx}(\arcsin(x)) = \frac{1}{\sqrt{1-x^2}}$$

$$\frac{d}{dx}(\arccos(x)) = -\frac{1}{\sqrt{1-x^2}}$$

$$\frac{d}{dx}(\arctan(x)) = \frac{1}{1+x^2}$$

$$\frac{d}{dx}(\arccot(x)) = -\frac{1}{1+x^2}$$

$$\frac{d}{dx}(\arcsec(x)) = \frac{1}{|x|\sqrt{x^2-1}}$$

$$\frac{d}{dx}(\arccsc(x)) = -\frac{1}{|x|\sqrt{x^2-1}}$$

### 5. Hyperbolic Functions

$$\frac{d}{dx}(\sinh(x)) = \cosh(x)$$

$$\frac{d}{dx}(\cosh(x)) = \sinh(x)$$

$$\frac{d}{dx}(\tanh(x)) = \text{sech}^2(x)$$

## Combining Rules

Most functions require combining multiple rules to find their derivatives.

**Example**: Find $\frac{d}{dx}[e^{x^2} \cdot \ln(3x+1)]$

Solution:
This requires the product rule, and within each part, the chain rule.

Let $f(x) = e^{x^2}$ and $g(x) = \ln(3x+1)$

For $f'(x)$:
- Using the chain rule: $f'(x) = e^{x^2} \cdot \frac{d}{dx}(x^2) = e^{x^2} \cdot 2x = 2xe^{x^2}$

For $g'(x)$:
- Using the chain rule: $g'(x) = \frac{1}{3x+1} \cdot \frac{d}{dx}(3x+1) = \frac{1}{3x+1} \cdot 3 = \frac{3}{3x+1}$

Now applying the product rule:
$\frac{d}{dx}[e^{x^2} \cdot \ln(3x+1)] = e^{x^2} \cdot \frac{3}{3x+1} + \ln(3x+1) \cdot 2xe^{x^2} = e^{x^2} \cdot \left(\frac{3}{3x+1} + 2x\ln(3x+1)\right)$

## Implicit Differentiation

Sometimes a function $y(x)$ is defined implicitly by an equation like $F(x, y) = 0$ rather than explicitly as $y = f(x)$. Implicit differentiation allows us to find $\frac{dy}{dx}$ without solving for $y$ explicitly.

The key is to differentiate both sides of the equation with respect to $x$, treating $y$ as a function of $x$ and using the chain rule when differentiating terms involving $y$.

**Example**: Find $\frac{dy}{dx}$ given that $x^2 + y^2 = 25$

Solution:
Differentiating both sides with respect to $x$:
$\frac{d}{dx}(x^2 + y^2) = \frac{d}{dx}(25)$
$2x + 2y\frac{dy}{dx} = 0$
Solving for $\frac{dy}{dx}$:
$2y\frac{dy}{dx} = -2x$
$\frac{dy}{dx} = -\frac{x}{y}$

## Logarithmic Differentiation

Logarithmic differentiation is useful for functions that involve products, quotients, or variables in exponents.

The technique involves:
1. Taking the natural logarithm of both sides of the equation
2. Using properties of logarithms to simplify
3. Differentiating implicitly with respect to $x$
4. Solving for $\frac{dy}{dx}$

**Example**: Find $\frac{d}{dx}[x^x]$

Solution:
Let $y = x^x$
Taking the natural logarithm of both sides:
$\ln(y) = \ln(x^x) = x\ln(x)$

Differentiating implicitly:
$\frac{1}{y}\frac{dy}{dx} = 1 \cdot \ln(x) + x \cdot \frac{1}{x} = \ln(x) + 1$

Solving for $\frac{dy}{dx}$:
$\frac{dy}{dx} = y(\ln(x) + 1) = x^x(\ln(x) + 1)$

## Practice Problems

1. Find the derivative of $f(x) = x^3\sin(x)$
2. Differentiate $g(x) = \frac{e^x}{x^2+1}$
3. Find $\frac{dy}{dx}$ if $xy + y^2 = 4$
4. Differentiate $h(x) = (x^2+1)^5$
5. Find the derivative of $f(x) = \ln(x\sqrt{1+x^2})$

### Solutions

1. $f'(x) = 3x^2\sin(x) + x^3\cos(x)$ (using the product rule)

2. $g'(x) = \frac{e^x(x^2+1) - e^x(2x)}{(x^2+1)^2} = e^x\cdot\frac{x^2+1-2x}{(x^2+1)^2} = e^x\cdot\frac{x^2-2x+1}{(x^2+1)^2}$ (using the quotient rule)

3. Differentiating implicitly:
   $x\frac{dy}{dx} + y + 2y\frac{dy}{dx} = 0$
   $(x + 2y)\frac{dy}{dx} = -y$
   $\frac{dy}{dx} = \frac{-y}{x + 2y}$

4. $h'(x) = 5(x^2+1)^4 \cdot 2x = 10x(x^2+1)^4$ (using the chain rule)

5. $f'(x) = \frac{1}{x\sqrt{1+x^2}} \cdot \left(1 \cdot \sqrt{1+x^2} + x \cdot \frac{1}{2}(1+x^2)^{-1/2} \cdot 2x\right)$ 
   $= \frac{1}{x\sqrt{1+x^2}} \cdot \left(\sqrt{1+x^2} + \frac{x^2}{\sqrt{1+x^2}}\right)$ 
   $= \frac{1}{x\sqrt{1+x^2}} \cdot \frac{1+x^2+x^2}{\sqrt{1+x^2}}$ 
   $= \frac{1+2x^2}{x(1+x^2)}$ (using the chain rule and the product rule)