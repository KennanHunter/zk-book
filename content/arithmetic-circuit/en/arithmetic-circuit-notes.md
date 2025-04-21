arithmetic circuit vs system of equations?

okay they're basically just systems of equations

lit i know those already

i saw the table of contents, interested in what set theory can do to simplify some of these arithmetic circuits, like with the three color problem where they represented the colors as bools, and now they represent the colors as numbers, instead of the more set theory idea of them being member of a union type

how did they get

```javascript
0 === (2 - xy) * (3 - xy) * (6 - xy)
```

ohh it's the set of products of the valid factor ok yep

is it possible to have cases where like a valid and a invalid combo both produce the same, i guess not when you constrain it to only multiplication

if it were addition you could have like

```javascript
4 === (x + y)
// or 
0 === 4 - (x + y)
```

and then x could be 1 and y could be 3, or x could be 2 and y could be 2

i feel like this binary encoding stuff is a little on the implementation detail side

NOTE: Rewatch the videos, i don't fully get the identity that 

> If the most significant bit of $2^{n-1} + (u - v)$ is 1, then $u \geq v$ and vice versa.

# Conclusion


# Practice problems

1. Create an arithmetic circuit that takes signals `x₁`, `x₂`, ..., `xₙ` and is satisfied if *at least* one signal is 0.

```javascript
0 = x_1 * x_2 * x_3 * ... x_n
```

2. Create an arithmetic circuit that takes signals `x₁`, `x₂`, ..., `xₙ` and is satsified if all signals are 1.

```javascript
0 = 1 - ((1 - x_1) * (1 - x_2) * (1 - x_3) * ... (1 - x_n))
```

3. A bipartite graph is a graph that can be colored with two colors such that no two neighboring nodes share the same color. Devise an arithmetic circuit scheme to show you have a valid witness of a 2-coloring of a graph. Hint: the scheme in this tutorial needs to be adjusted before it will work with a 2-coloring.
 :(

4. Create an arithmetic circuit that constrains `k` to be the maximum of `x`, `y`, or `z`. That is, `k` should be equal to `x` if `x` is the maximum value, and same for `y` and `z`.



