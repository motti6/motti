@def title = "Mottilin"
@def hasmath = true
@def hascode = true

# Set up

## Update title

## Update config.md file

* change author

* add site name for Github

## Create a table of contents

\toc

## Upload using Github Desktop

# Examples

## How to enter text

こんにちは

## How to render math equations

$$ a^2 + b^2 = c^2 $$

$$ \frac{d}{dx} \int_a^x f(t)dt = f(x)$$

$$ \bar{x} = \frac{1}{n} \Bigg(\sum{i=1}^n x_i\Bigg) = frac{x_1 + x_2 + \cdots + x_n}{n}$$

$$
  M = 
     \begin{bmatrix}
       \begin{aligned}
          &2 & &1 & -&1\space \\
          \space-&3 & -&1 & &2 \\
          -&2 & &1 & &2
       \end{aligned}
    \end{bmatrix}
$$

## How to insert julia code

Hello, World!

```julia:./ex11
println("Hello, World!")
```

\show{./ex11}

Basic Math

```julia:./ex12
1+1
```

\show{./ex12}

Create function

```julia:./ex13
function add(x,y)
    x + y
end
```

\show{./ex13}

## How to insert a clickable thumbnail to a Youtube video

[![YT thmbnail](https://img.youtube.com/vi/IjGLD2jXD50/0.jpg)](https://youtu.be/IjGLD2jXD50)

## How to inject raw HTML

~~~
<iframe width="640" height="360" src="https://www.youtube.com/embed/IjGLD2jXD50" title="モンスターハンターワールド：アイスボーン 20220319214445" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
~~~




# Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex.
