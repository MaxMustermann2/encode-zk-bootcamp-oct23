# Homework 2

1. Is it true that all odd squares are $\equiv 1 (mod 8)$ ?

$$
\text{Let }n \in \mathbb{N} \mid n = 2x + 1 \text{ for some } x \in \mathbb{N}\\
n^2 = 4x^2 + 1 + 4x\\
n^2 = 1 + 4x(x+1)\\
\text{ }\\
\text{Since } x \in \mathbb{N}\text{ , either }x\text{ is even or }x+1\text{ is even.}\\
n^2 = 1 + 4*2*k\text{ for some }k\\
n^2 = 1 + 8k\\
n^2 \equiv 1 (mod 8)
$$

2. What about even squares (mod 8) ?

$$
\text{Let }n \in \mathbb{N} \mid n = 2y + 1 \text{ for some } y \in \mathbb{N}\\
n = 2y\\
n^2 = 4y^2\\
\text{If }y\text{ is even, }n^2 \equiv 0(mod 8)\\
\text{ }\\
\text{If }y\text{ is odd, let }y = 2x + 1\text{ for some } x \in \mathbb{N}\\
\implies n^2 = 4(2x+1)^2\\
n^2 \equiv 4(2x+1)^2 (mod 8)\\
n^2 \equiv 4(mod 8) * (2x + 1)^2 (mod 8)\\
n^2 \equiv 4 * 1 (mod 8)\\
n^2 \equiv 4 (mod 8)\\
$$

Even squares are either $0$ or $4$ (mod 8).

3. What are $O(n)$, $O(1)$, and $O(log n)$ ?

The big-O notation is used to represent the worst-case time (or space) complexity of achieving a task of size $n$. Simply put, when it is said that an algorithm has $O(n)$ time complexity, it means that the time taken by the algorithm is proportional to $n$ in the worst case. Similarly, $O(1)$ represents constant time complexity, and $O(log n)$ represents a time complexity slower than $O(n)$ since it is proportional to $log n$. Note that we use the word _proportional_ here and not equal. This means that it is possible for an algorithm that is $O(1)$ to take longer than $O(n)$ if the _factor_ for $O(n)$ is small.

4. For a proof size, which of these complexities would you want?

$O(1)$
