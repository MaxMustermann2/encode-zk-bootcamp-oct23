# Homework 1

## Maths Introduction

### Some modular arithmetic

1. Working with the following set of integers $S={0,1,2,3,4,5,6}$, what is

- $4 + 4 = 8 \equiv 1 (mod 7)$
- $3 * 5 = 15 \equiv 1 (mod 7)$
- $3^{-1} \equiv 5 (mod 7) \because 3 * 5 = 15 \equiv 1 (mod 7) \text{ or } 3^{-1} \equiv 3^{7-2} \equiv 243 \equiv 5 (mod 7) \text{ as per Fermat's little theorem}$

2. For $S={0,1,2,3,4,5,6}$, can the operation $+$ be considered a group? If the operation is defined under $mod 7$, the set is a group. This is because it follows the properties of closure, associativity, identity and inverse.

3. What is $-13 mod 5$? $13 mod 5 = 3 \implies -13 mod 5 = -3 \implies -13 mod 5 = 2$

4. Given a polynomial $x^3 - x^2 + 4x - 12$, what is its degree? The degree is $3$. What are its roots?

$$
f(x) = x^3 - x^2 + 4x - 12\\
f(2) = 8 - 4 + 8 - 12 = 0 \implies 2 \text{ is a root, or that } (x-2) \text{ is a factor of } f(x)
$$

We use long division to find the quotient.

$$
\begin{array}{r}
x-2\overline{\smash{\big)}\phantom{1}x^3 - \phantom{1}x^2 + 4x - 12\smash{\big(}}{x^2 + x + 6}\\
x^3 - 2x^2\phantom{+4x - 12\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 + }\overline{\phantom{1}x^2 + 4x}\phantom{ - 12\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 - }\phantom{1}x^2 - 2x\phantom{ - 12\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 - 2x^2 + }\overline{6x - 12}\phantom{\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 - 2x^2 + }6x - 12\phantom{\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 - 2x^2 + 4x - }\phantom{1}\overline{0}\phantom{\smash{\big(}{x^2 + x + 6}}\\
\phantom{x^3 - 2x^2 + 4x - 1}\overline{\phantom{0}}\phantom{\smash{\big(}{x^2 + x + 6}}\\
\end{array}
$$

Since there are no real roots of the quotient $x^2 + x + 6 = 0$, the only such root of $f(x)$ is $2$.