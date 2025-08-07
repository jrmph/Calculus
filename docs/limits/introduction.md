# Introduction to Limits

Limits are the foundation of calculus. They allow us to describe the behavior of functions as their inputs approach specific values, even if the function isn't defined at those values.

## The Intuitive Idea of a Limit

Consider the function $f(x) = \frac{x^2 - 1}{x - 1}$. This function is not defined at $x = 1$ because we'd get $\frac{0}{0}$, which is indeterminate.

But what happens when $x$ gets very close to 1?

| $x$ | $f(x) = \frac{x^2 - 1}{x - 1}$ |
|-----|------------------------------|
| 0.9 | 1.9 |
| 0.99 | 1.99 |
| 0.999 | 1.999 |
| 1.001 | 2.001 |
| 1.01 | 2.01 |
| 1.1 | 2.1 |

We can see that as $x$ approaches 1 (from either side), $f(x)$ approaches 2. We write this as:

$$\lim_{x \to 1} \frac{x^2 - 1}{x - 1} = 2$$

This is read as "the limit of $f(x)$ as $x$ approaches 1 is 2."

## Formal Definition of a Limit

For a function $f(x)$ and a real number $a$, we say that the limit of $f(x)$ as $x$ approaches $a$ is $L$, written as:

$$\lim_{x \to a} f(x) = L$$

if for every $\epsilon > 0$, there exists a $\delta > 0$ such that:

$$\text{if } 0 < |x - a| < \delta, \text{ then } |f(x) - L| < \epsilon$$

This is often called the epsilon-delta definition of a limit.

## One-Sided Limits

There are two types of one-sided limits:

1. **Left-hand limit**: The limit as $x$ approaches $a$ from values less than $a$, denoted as $\lim_{x \to a^-} f(x)$
2. **Right-hand limit**: The limit as $x$ approaches $a$ from values greater than $a$, denoted as $\lim_{x \to a^+} f(x)$

A limit exists if and only if both one-sided limits exist and are equal:

$$\lim_{x \to a} f(x) = L \iff \lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) = L$$

## Properties of Limits

Assuming the limits of functions $f(x)$ and $g(x)$ exist as $x$ approaches $a$, the following properties hold:

1. **Constant Rule**: $\lim_{x \to a} c = c$, where $c$ is a constant
2. **Identity Rule**: $\lim_{x \to a} x = a$
3. **Sum Rule**: $\lim_{x \to a} [f(x) + g(x)] = \lim_{x \to a} f(x) + \lim_{x \to a} g(x)$
4. **Difference Rule**: $\lim_{x \to a} [f(x) - g(x)] = \lim_{x \to a} f(x) - \lim_{x \to a} g(x)$
5. **Product Rule**: $\lim_{x \to a} [f(x) \cdot g(x)] = \lim_{x \to a} f(x) \cdot \lim_{x \to a} g(x)$
6. **Quotient Rule**: $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{\lim_{x \to a} f(x)}{\lim_{x \to a} g(x)}$, if $\lim_{x \to a} g(x) \neq 0$
7. **Power Rule**: $\lim_{x \to a} [f(x)]^n = [\lim_{x \to a} f(x)]^n$
8. **Root Rule**: $\lim_{x \to a} \sqrt[n]{f(x)} = \sqrt[n]{\lim_{x \to a} f(x)}$, if $\lim_{x \to a} f(x) \geq 0$ for even $n$

## Common Limits

1. $\lim_{x \to 0} \frac{\sin(x)}{x} = 1$
2. $\lim_{x \to 0} \frac{1 - \cos(x)}{x} = 0$
3. $\lim_{x \to \infty} (1 + \frac{1}{x})^x = e$

## Limits That Do Not Exist

A limit doesn't exist if:

1. The function approaches different values from the left and right sides
2. The function grows without bound (tends to infinity)
3. The function oscillates without settling towards a specific value

## Example: Finding a Limit

Let's evaluate $\lim_{x \to 1} \frac{x^2 - 1}{x - 1}$

Solution:
We can factor the numerator to simplify:

$$\lim_{x \to 1} \frac{x^2 - 1}{x - 1} = \lim_{x \to 1} \frac{(x+1)(x-1)}{x - 1}$$

Canceling the common factor $(x-1)$ when $x \neq 1$:

$$\lim_{x \to 1} (x+1) = 1+1 = 2$$

## When Direct Substitution Doesn't Work

When a limit leads to indeterminate forms like $\frac{0}{0}$, $\frac{\infty}{\infty}$, $0 \cdot \infty$, etc., we need special techniques:

1. **Factoring**: As shown in the example above
2. **Rationalization**: For limits involving square roots
3. **L'Hôpital's Rule**: For certain indeterminate forms (covered later)

## Limits in Applications

Limits appear in many calculus applications, including:

1. **Instantaneous rate of change** (the derivative)
2. **Area under curves** (the definite integral)
3. **Continuity** of functions
4. **Asymptotic behavior** of functions

## Practice Problems

1. Evaluate $\lim_{x \to 3} \frac{x^2 - 9}{x - 3}$
2. Find $\lim_{x \to 0} \frac{\sin(2x)}{x}$
3. Determine whether $\lim_{x \to 0} \frac{|x|}{x}$ exists
4. Calculate $\lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4}$

### Solutions

1. $\lim_{x \to 3} \frac{x^2 - 9}{x - 3} = \lim_{x \to 3} \frac{(x+3)(x-3)}{x - 3} = \lim_{x \to 3} (x+3) = 6$

2. $\lim_{x \to 0} \frac{\sin(2x)}{x} = \lim_{x \to 0} \frac{2\sin(2x)}{2x} \cdot 2 = 2 \cdot \lim_{u \to 0} \frac{\sin(u)}{u} = 2 \cdot 1 = 2$ (where $u = 2x$)

3. This limit doesn't exist. As $x$ approaches 0 from the right, $\frac{|x|}{x} = \frac{x}{x} = 1$, but as $x$ approaches 0 from the left, $\frac{|x|}{x} = \frac{-x}{x} = -1$. Since the left and right limits are different, the limit doesn't exist.

4. $\lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4} = \lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4} \cdot \frac{\sqrt{x} + 2}{\sqrt{x} + 2} = \lim_{x \to 4} \frac{x - 4}{(x - 4)(\sqrt{x} + 2)} = \lim_{x \to 4} \frac{1}{\sqrt{x} + 2} = \frac{1}{4}$