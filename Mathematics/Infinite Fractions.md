---
aliases: [ ]
tags: [GR10/Q4 maths/algebra apm ]
created: Tue 01/11 2022
modified: Tue 01/11 2022
---
# Infinite Fractions
 ^blurb

This is a infinitely repeating fraction: 
$$ 4 + \frac{5}{4 + \frac{5}{4 + \frac{5}{4}...}}$$
To solve this, we would put it in terms of 𝑥
$$x = 4+\frac{5}{4 + \frac{5}{4 + \frac{5}{4}...}}$$
then, we would say:
$$x= 4+\frac{5}{x}$$
and from there we would simplify
$$
\begin{flalign}

   & x \times x = 4 + \frac{5}{x} \times x \textrm{ ... we get rid of the fraction by multiplying both sides by x}
\\ & x^2 = 4 + 5x
\\ & 0 = x^2 -5x -4 \textrm{ ... Bring over the x and change all signs so we have a standard trinomial}
\\ & 0 = (x - 5)(x + 1) \textrm{ ... Note how we can use the zero-product rule here}
\\ & ∴ x = 5 \textrm{ or } x = -1
\end{flalign}
$$
if we take a close look here, we can see that -1 would not suit our original sum, as there were no negatives in it. So, we can say:
$$
∴ x = 5 ∵ \textrm{no negatives in original statement}
$$

## Other uses:
This method is actually useful in other places as well, such as repeating square roots
$$
\begin{flalign}
\\ & \sqrt{2 + \sqrt{2 + \sqrt{2 + \sqrt{2 + }}}}... \\
\\ & x = \sqrt{2+x}
\\ & x^2 = \sqrt{2+x}^2 \textrm{ ... square both sides}
\\ & x^2 = 2 + x
\\ & 0 = x^2 -x -2 \textrm{ ... zero product and }
\\ & 0 = (x + 2)(x - 1) \textrm{ ... factorize}
\\ & ∴ x = -2 \textrm{ or } x = 1
\\ & x = 1 ∵ \textrm{ there are no negtives in the original statement}
\end{flalign}
$$