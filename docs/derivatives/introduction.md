# Introduction to Derivatives

The derivative is one of the central concepts in calculus, representing the instantaneous rate of change of a function with respect to one of its variables.

## The Problem of Instantaneous Rate of Change

Imagine you're driving a car and looking at your speedometer, which gives your instantaneous speed. How is this value determined mathematically?

If we know the position function $s(t)$ of the car at time $t$, the average speed over a time interval $[t, t+h]$ is:

$$\text{Average speed} = \frac{s(t+h) - s(t)}{h}$$

But what about the speed at exactly time $t$? This requires finding the instantaneous rate of change, which is where derivatives come in.

## Definition of the Derivative

The derivative of a function $f$ at a point $x = a$ is defined as the limit:

$$f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}$$

Alternatively, using the limit notation with $x$ approaching $a$:

$$f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$

The derivative $f'(x)$ (read as "f prime of x") gives the instantaneous rate of change of $f(x)$ with respect to $x$.

## Notation for Derivatives

There are several notations for the derivative:

1. **Lagrange's notation**: $f'(x)$, $f''(x)$, etc.
2. **Leibniz's notation**: $\frac{dy}{dx}$ or $\frac{d}{dx}f(x)$ where $y = f(x)$
3. **Newton's notation**: $\dot{y}$ (dot notation)
4. **Euler's notation**: $Df$ or $D_x f$

## Interpretations of the Derivative

The derivative has several important interpretations:

1. **Rate of Change**: $f'(a)$ is the instantaneous rate of change of $f$ at $x = a$
2. **Slope of the Tangent Line**: $f'(a)$ is the slope of the line tangent to the curve $y = f(x)$ at the point $(a, f(a))$
3. **Velocity**: If $s(t)$ represents position, then $s'(t)$ represents velocity
4. **Sensitivity Analysis**: How sensitive the output is to small changes in the input

## Differentiability

A function $f$ is differentiable at a point $a$ if $f'(a)$ exists. For a function to be differentiable at a point, it must be:

1. Defined at that point
2. Continuous at that point

However, continuity alone doesn't guarantee differentiability. A function can be continuous but have a "sharp point" or "corner" where the derivative doesn't exist.

## The Derivative as a Function

While $f'(a)$ gives the derivative at a specific point $a$, we can also consider the derivative as a function $f'(x)$ that gives the rate of change at any point $x$ in the domain.

## Example: Finding a Derivative from the Definition

Let's find the derivative of $f(x) = x^2$ using the definition.

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

$$f'(x) = \lim_{h \to 0} \frac{(x+h)^2 - x^2}{h}$$

$$f'(x) = \lim_{h \to 0} \frac{x^2 + 2xh + h^2 - x^2}{h}$$

$$f'(x) = \lim_{h \to 0} \frac{2xh + h^2}{h}$$

$$f'(x) = \lim_{h \to 0} (2x + h)$$

$$f'(x) = 2x$$

So, the derivative of $f(x) = x^2$ is $f'(x) = 2x$.

## Basic Rules of Differentiation

While we can always use the definition to find derivatives, there are established rules that make the process much simpler:

1. **Constant Rule**: If $f(x) = c$ (a constant), then $f'(x) = 0$
2. **Power Rule**: If $f(x) = x^n$, then $f'(x) = nx^{n-1}$
3. **Constant Multiple Rule**: If $f(x) = c \cdot g(x)$, then $f'(x) = c \cdot g'(x)$
4. **Sum Rule**: If $f(x) = g(x) + h(x)$, then $f'(x) = g'(x) + h'(x)$
5. **Difference Rule**: If $f(x) = g(x) - h(x)$, then $f'(x) = g'(x) - h'(x)$

More advanced rules like the Product Rule, Quotient Rule, and Chain Rule will be covered in subsequent sections.

## The Derivative of Common Functions

1. $\frac{d}{dx}(c) = 0$ where $c$ is a constant
2. $\frac{d}{dx}(x) = 1$
3. $\frac{d}{dx}(x^n) = nx^{n-1}$ for any real number $n$
4. $\frac{d}{dx}(e^x) = e^x$
5. $\frac{d}{dx}(\ln(x)) = \frac{1}{x}$ for $x > 0$
6. $\frac{d}{dx}(\sin(x)) = \cos(x)$
7. $\frac{d}{dx}(\cos(x)) = -\sin(x)$
8. $\frac{d}{dx}(\tan(x)) = \sec^2(x)$

## Application: Tangent Lines

One immediate application of derivatives is finding the equation of the tangent line to a curve at a specific point.

If we want to find the tangent line to $y = f(x)$ at the point $(a, f(a))$:

1. Find the derivative $f'(a)$ at the point $x = a$
2. Use the point-slope form of a line: $y - f(a) = f'(a)(x - a)$

Example: Find the equation of the tangent line to $f(x) = x^2$ at the point $(2, 4)$.

1. We know $f'(x) = 2x$, so $f'(2) = 4$
2. Using point-slope form: $y - 4 = 4(x - 2)$
3. Simplifying: $y = 4x - 4$

## Higher-Order Derivatives

We can differentiate a function more than once:

- The second derivative, denoted $f''(x)$ or $\frac{d^2y}{dx^2}$, is the derivative of the first derivative
- The third derivative, denoted $f'''(x)$ or $\frac{d^3y}{dx^3}$, is the derivative of the second derivative
- And so on...

Higher-order derivatives have important physical interpretations. For example, if $s(t)$ is position:
- $s'(t)$ is velocity
- $s''(t)$ is acceleration

## When Derivatives Don't Exist

A function is not differentiable at points where:

1. There's a vertical tangent (infinite slope)
2. There's a corner or cusp
3. There's a discontinuity

For example, $f(x) = |x|$ is not differentiable at $x = 0$ because there's a corner at that point.

## Practice Problems

1. Find the derivative of $f(x) = 3x^2 - 2x + 5$ using the basic rules.
2. Find the derivative of $g(x) = \sqrt{x}$ using the definition of the derivative.
3. Find the equation of the tangent line to $f(x) = x^3$ at the point $(1, 1)$.
4. Determine where the function $h(x) = |x^2 - 4|$ is not differentiable.

### Solutions

1. Using the sum, difference, and power rules:
   $f'(x) = 3(2x) - 2(1) + 0 = 6x - 2$

2. Using the definition with $g(x) = x^{1/2}$:
   $g'(x) = \lim_{h \to 0} \frac{\sqrt{x+h} - \sqrt{x}}{h}$
   $= \lim_{h \to 0} \frac{\sqrt{x+h} - \sqrt{x}}{h} \cdot \frac{\sqrt{x+h} + \sqrt{x}}{\sqrt{x+h} + \sqrt{x}}$
   $= \lim_{h \to 0} \frac{(x+h) - x}{h(\sqrt{x+h} + \sqrt{x})}$
   $= \lim_{h \to 0} \frac{h}{h(\sqrt{x+h} + \sqrt{x})}$
   $= \lim_{h \to 0} \frac{1}{\sqrt{x+h} + \sqrt{x}}$
   $= \frac{1}{2\sqrt{x}}$

3. For $f(x) = x^3$, we have $f'(x) = 3x^2$.
   At $x = 1$: $f'(1) = 3(1)^2 = 3$
   Using point-slope form: $y - 1 = 3(x - 1)$
   Simplifying: $y = 3x - 2$

4. The function $h(x) = |x^2 - 4|$ is not differentiable at $x = \pm 2$ (where $x^2 - 4 = 0$) because the absolute value function creates corners at these points.