---
aliases: [ ]
tags: [GR10 physics/motion GR11/Q1 ]
created: Mon 07/11 2022
modified: Thu 03/11 2022 08:00
---
# Newtons Third Law
Newton’s Third law dictates interactions where objects are applying force on one-another. It helps us understand why we aren’t all pulled to the ground by gravity, or how walls are not just pushed over when we lean on them. 

> [!definition]
> **Newton’s Third Law**: When one body everts a force on a second body, the second body everts a force of equal magnitude in the opposite direction on the first body 
>
> When we encounter these equal forces that are opposite in direction, we call them Newton III Force pairs. When working on a straight line, we can say:
> $$
> F_{a \textrm{ on } b} = - F_{b \textrm{ on } a}
> $$

Newton III force pairs are different to *opposing forces*. Newton III force pairs act between two objects on the same plane, and are always equal to each-other. Opposing forces act on *the same object* on the same plane and are not always equal. This is what gives rise to the Net Force, and as we know from [[Newton's First Law]] and [[Newton's Second Law]]:
$$
\textrm{If} \space F_1 = -F_2 \textrm{ then: } \vec{F}_{net} = 0N; a = 0m.s^{-2}
$$
$$
\textrm{If} \space F_1 > -F_2 \textrm{ then: } \vec{F}_{net} \neq 0N; a > 0m.s^{-2}
$$

> [!example]+
> **Q**: Bob ($5kg$) and Nigel ($50kg$) stand still on roller skates and push each other. They move away from each other, compare their accelerations.
>
> **A**: 
>
>
>$$
>\begin{align*}
>& Fnet_{(B \textrm{ on } N)} = Fnet_{(N \textrm{ on } B)} & ... \textrm{Newton III Pairs} \\
>& \therefore m_B \times a_B = m_N \times a_N & ...\vec{F}_{net} = m \times a \\
>& \textrm{But: } m_B < m_N \\
>& \therefore \vec{a}_B > \vec{a}_N
>\end{align*}
>$$

> [!example]+
> **Q**: Two blocks that are  $6kg$ and $3kg$ lie on a rough horizontal surface. A $20N$ force is applied onto the $3kg$ block. The frictional force between each block and the surface is $1N$. Calculate:
> 1. The force exerted by the $6kg$ block on the $3kg$ block
> 2. The acceleration of the two blocks. 
> 
> **A**: 
> $$
> \begin{align}
> & F_A = 20N \textrm{ right} \\
> & \vec{F}_{net \textrm{ of } 6} = 6a && ... \vec{F}_{net} = ma \\
> & F_{3 \textrm{ on } 6} - F_f = 6a \\
> \implies & F_{3 \textrm{ on } 6}= 6a + 1 && ... \vec{F}_{net} = F_A + F_f\\
> & \vec{F}_{net \textrm{ of } 3} = 3a && ... \vec{F}_{net} = ma \\
> & -F_{6 \textrm{ on } 3} + F_A - F_f = 3a \\
> \implies &-F_{6 \textrm{ on } 3} = 3a + (20-1) = 3a - 19&& ... \vec{F}_{net} = F_A + F_f \\
> \\
> & F_{3 \textrm{ on } 6} = -F_{6 \textrm{ on } 3} && ... \textrm{Newton III Pair} \\
> \therefore \space & 6a + 1 = -3a + 19 \\
> \therefore \space & 9a = 18 \\
> \therefore \space & a = 2m.s^{-2} \textrm{ left} && → \textrm{Answer 2}\\ 
> \\
> & F_{6 \textrm{ on } 3} = 3a - 19 \\
> & F_{6 \textrm{ on } 3} = 3(2) - 19 \\
> & F_{6 \textrm{ on } 3} = -13N \textrm{ or } 13N \textrm{ left} && → \textrm{Answer 1}
> \end{align} 
> $$
