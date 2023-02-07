---
date: Thu 13/10 2022
aliases: [ ]
tags: [GR10/Q4 terminology physics/waves ]
modified: Thu 03/11 2022 08:00
---
# Period (T)
**Definition**: the Period of a wave is the time it takes for one complete [[Wavelength (λ)|wavelengths]] to pass a certain point. ^definition

**Unit of Measure**: seconds (s)

**Formula**: 

Given Frequency:
$$
\begin{flalign}
\\& T = \frac{1}{f}
\\& Where:
\\& T = Period
\\& f = Frequency
\end{flalign}
$$
[[Period (T)]]

Given Wave speed:
$$
\begin{flalign}
\\& v = \frac{\lambda}{T}
\\& \therefore T = \frac{\lambda}{v}
\\& Where:
\\& T = \textrm{Period } (s)
\\& \lambda = \textrm{Wavelength } (m)
\\& v = \textrm{Wave Speed } (m.s^{-1})
\end{flalign}
$$
[[Wavelength (λ)]]; [[Wave Speed (v)]]
## How to measure Period
1 wave is made of 2 [[Transverse Pulses|pulses]]
```desmos-graph
left=-2; right=2;
top=2; bottom=-2;
---
y=\sin(2x)
x=\pi/2|dashed|red
x=\pi/-2|dashed|red
(\pi/2,0)|label:C
(0,0)|label:B
(\pi/-2,0)|label:A
```
> A → B is one pulse, but A → C is a wave

```desmos-graph
left=-2; right=2;
top=2; bottom=-2;
---
y=\sin(4x)
x=\pi/2|dashed|red

(\pi/2,0)|label:A
```
The period will be the amount of time it takes for one full wave to pass A. This is inverse to the [[Frequency (f)]], but is linked with the [[Wave Speed (v)]]