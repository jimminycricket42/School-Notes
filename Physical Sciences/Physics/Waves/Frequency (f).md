---
date: Thu 13/10 2022
aliases: [ ]
tags: [GR10/Q4 physics/waves ]
modified: Thu 03/11 2022 08:00
---
# Frequency (f)
**Definition**:  Frequency is the number of [[Wavelength (λ)|wavelengths]] that move past a certain point in a second. ^definition

**Unit of Measure**:

**Formula**:
Given [[Period (T)]]
$$
\begin{flalign}
\\& f = \frac{1}{T}

\\& Where:
\\& f = \textrm{Freqency } (Hz)
\\& T = \textrm{Period } (s)
\end{flalign}
$$
> [[Period (T)]]

> [!note]+ :spiral_notepad: Alternative Measure of frequency than Hertz
> Frequency can also be measured as $n.s^{-1}$

Given [[Wave Speed (v)]]
$$
\begin{flalign}
\\& v = f\times\lambda
\\& \therefore f = \frac{v}{\lambda}
\\& Where:
\\& f = \textrm{Freqency } (Hz)
\\& v = \textrm{Wave Speed } (m.s^{-1})
\\& \lambda = \textrm{Wavelength } (m)
\end{flalign}
$$
> [[Wavelength (λ)]]; [[Wave Speed (v)]]

## How to measure Freqency
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
The Frequency will be the amount of waves that pass A in a second. This is inverse to the [[Period (T)]], but is linked with the [[Wave Speed (v)]]. 