---
title: Typesetting Math in Texts
---

Basic math
----------

Whenever you typeset mathematical notation, it needs to have “Math” style. For
example: If $$a$$ is an integer, then $$2a+1$$ is odd.

Superscripts and subscripts are created using the characters `^` and `_`,
respectively: $$x^2+y^2=1$$ and $$a_n=0$$. It is fine to have both on a single
letter: $$x_0^2$$.

If the superscript [or subscript] is more than a single character, enclose the
superscript in curly braces: $$e^{-x}$$.

Greek letters are typed using commands such as `\gamma` ($$\gamma)$$ and
`\Gamma` ($$\Gamma$$).

Named mathematics operators are usually typeset in roman. Most of the standards
are already available. Some examples: $$\det A$$, $$\cos\pi$$, and
$$\log(1-x)$$.

Displayed equations
-------------------

When an equation becomes too large to run in-line, you display it in a “Math”
paragraph by itself.

$$
f(x) = 5x^{10}-9x^9 + 77x^8 + 12x^7 + 4x^6 - 8x^5 + 7x^4 + x^3 -2x^2 + 3x + 11.
$$

The `\begin{aligned}...\end{aligned}` environment is superb for lining up
equations.

$$
\begin{aligned}
  (x-y)^2
  &= (x-y)(x-y) \\
  &= x^2 -yx - xy + y^2 \\
  &= x^2 -2xy +y^2.
\end{aligned}
$$

$$
\begin{aligned}
  3x-y&=0 & 2a+b &= 4 \\
  x+y &=1 & a-3b &=10
\end{aligned}
$$

To insert ordinary text inside of mathematics mode, use `\text`:

$$
f(x) = \frac{x}{x-1} \text{ for $x\not=1$}.
$$

This is the $$3^{\text{rd}}$$ time I’ve asked for my money back.

The `\begin{cases}...\end{cases}` environment is perfect for defining functions
piecewise:

$$
|x| =
\begin{cases}
x & \text{when $x \ge 0$ and} \\
-x & \text{otherwise.}
\end{cases}
$$

Relations and operations
------------------------

-   Equality-like: $$x=2$$, $$x \not= 3$$, $$x \cong y$$, $$x \propto y$$,
    $$y\sim z$$, $$N \approx M$$, $$y \asymp z$$, $$P \equiv Q$$.

-   Order: $$x < y$$, $$y \le z$$, $$z \ge 0$$, $$x \preceq y$$, $$y\succ z$$,
    $$A \subseteq B$$, $$B \supset Z$$.

-   Arrows: $$x \to y$$, $$y\gets x$$, $$A \Rightarrow B$$, $$A \iff B$$, $$x
    \mapsto f(x)$$, $$A \Longleftarrow B$$.

-   Set stuff: $$x \in A$$, $$b \notin C$$, $$A \ni x$$. Use `\notin` rather
    than `\not\in`. $$A \cup B$$, $$X \cap Y$$, $$A \setminus B = \emptyset$$.

-   Arithmetic: $$3+4$$, $$5-6$$, $$7\cdot 8 = 7\times8$$,
    $$3\div6=\frac{1}{2}$$, $$f\circ g$$, $$A \oplus B$$, $$v \otimes w$$.

-   Mod: As a binary operation, use `\bmod`: $$x \bmod N$$. As a relation use
    `\mod`, `\pmod`, or `\pod`:

    $$
    \begin{aligned}
      x &\cong y \mod 10 \\
      x &\cong y \pmod{10} \\
      x &\cong y \pod{10}
    \end{aligned}
    $$

-   Calculus: $$\partial F/\partial x$$, $$\nabla g$$.

Use the right dots
------------------

Do not type three periods; instead use `\cdots` between operations and `\ldots`
in lists: $$x_1 + x_2 + \cdots + x_n$$ and $$(x_1,x_2,\ldots,x_n)$$.

Built up structures
-------------------

-   Fractions: $$\frac{1}{2}$$, $$\frac{x-1}{x-2}$$.

-   Binomial coefficients: $$\binom{n}{2}$$.

-   Sums and products. Do *not* use `\Sigma` and `\Pi`.

    $$
    \sum_{k=0}^\infty \frac{x^k}{k!} \not= \prod_{j=1}^{10} \frac{j}{j+1}.
    $$

    $$
    \bigcup_{k=0}^\infty A_k
    \qquad
    \bigoplus_{j=1}^\infty V_j
    $$

-   Integrals:

    $$
    \int_0^1 x^2 \, dx
    $$

    The extra bit of space before the $$dx$$ term is created with the `\,`
    command.

-   Limits:

    $$
    \lim_{h\to0} \frac{\sin(x+h) - \sin(x)}{h} = \cos x .
    $$

    Also $$\limsup_{n\to\infty} a_n$$.

-   Radicals: $$\sqrt{3}$$, $$\sqrt[3]{12}$$, $$\sqrt{1+\sqrt{2}}$$.

-   Matrices:

    $$
    A = \left[\begin{matrix} 3 & 4 & 0 \\ 2 & -1 & \pi \end{matrix}\right] .
    $$

    A big matrix:

    $$
    D = \left[ 
        \begin{matrix}
          \lambda_1 & 0 & 0 & \cdots & 0 \\
          0 & \lambda_2 & 0 & \cdots & 0 \\
          0 & 0 & \lambda_3 & \cdots & 0 \\
          \vdots & \vdots & \vdots & \ddots & \vdots \\
          0 & 0 & 0 & \cdots & \lambda_n
        \end{matrix}
        \right].
    $$

Delimiters
----------

-   Parentheses and square brackets are easy: $$(x-y)(x+y)$$, $$[3-x]$$.

-   For curly braces use `\{` and `\}`: $$\{x : 3x-1 \in A\}$$.

-   Absolute value: $$\vert x-y\vert$$, $$\vert\vec{x} - \vec{y}\vert$$.

-   Floor and ceiling: $$\lfloor \pi \rfloor = \lceil e \rceil$$.

-   To make delimiters grow so they are properly sized to contain their
    arguments, use `\left` and `\right`:

    $$
    \left[ \sum_{n=0}^\infty a_n x^n \right]^2 =
    \exp \left\{ - \frac{x^2}{2} \right\}
    $$

    Occasionally, it is useful to coerce a larger sized delimiters than
    `\left`/`\right` produce. Look at the two sides of this equation:

    $$
    \left((x_1+1)(x_2-1)\right)
    =
    \bigl((x_1+1)(x_2-1)\bigl).
    $$

    I think the right is better. Use `\bigl`, `\Bigl`, `\biggl`, and the
    matching `\bigr`, etc.

-   Underbraces:

    $$
    \underbrace{1+1+\cdots+1}_{\text{$n$ times}} = n .
    $$

Styled and decorated letters
----------------------------

-   Primes: $$a'$$, $$b''$$.

-   Hats: $$\bar a$$, $$\hat a$$, $$\vec a$$, $$\widehat{a_j}$$.

-   Vectors are often set in bold: $$\mathbf{x}$$.

-   Calligraphic letters (for sets of sets): $$\mathcal{A}$$.

-   Blackboard bold for number systems: $$\mathbb{C}$$.

The text above is based on a paper by Edward R. Scheinerman[^1].

[^1]: <http://www.ams.jhu.edu/~ers/learn-latex/>

A few more examples from mathTeX tutorial[^2].

[^2]: <http://www.forkosh.com/mathtex.html>.

$$
e^x=\sum_{n=0}^\infty\frac{x^n}{n!}
$$

$$
e^x=\lim_{n\to\infty} \left(1+\frac xn\right)^n
$$

$$
\varepsilon = \sum_{i=1}^{n-1} \frac1{\Delta x}
  \int\limits_{x_i}^{x_{i+1}} \left\{
    \frac1{\Delta x}\big[
      (x_{i+1}-x)y_i^\ast+(x-x_i)y_{i+1}^\ast
    \big]-f(x)
  \right\}^2dx
$$

Solution for quadratic:

$$
x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}
$$

Definition of derivative:

$$
f^\prime(x)\ = \lim_{\Delta x\to0}\frac{f(x+\Delta x)-f(x)}{\Delta x}
$$

Continued fraction:

$$
f=b_o+\frac{a_1}{b_1+\frac{a_2}{b_2+\frac{a_3}{b_3+a_4}}}
$$

Demonstrating `\left\{…\right.` and accents.

$$
\tilde y=\left\{ {\ddot x \mbox{ if $x$ odd}\atop\widehat{\bar x+1}\text{ if even}}\right.
$$

Overbrace and underbrace:

$$
\overbrace{a,...,a}^{\text{k a's}},
\underbrace{b,...,b}_{\text{l b's}}\hspace{10pt}
\underbrace{\overbrace{a...a}^{\text{k a's}},
\overbrace{b...b}^{\text{l b's}}}_{\text{k+l elements}}
$$

Illustrating array:

$$
A\ =\ \left( \begin{array}{c|ccc}
& 1 & 2 & 3 \\ \hline
1&a_{11}&a_{12}&a_{13} \\
2&a_{21}&a_{22}&a_{23} \\
3&a_{31}&a_{32}&a_{33}
\end{array} \right)
$$

See [Wikibook on
LaTeX](<http://en.wikibooks.org/wiki/LaTeX/Mathematics#Symbols>) for more
examples.
