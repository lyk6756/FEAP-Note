Orthotropic Material Array and Thermal Modulus Transformation
================================================================

Rotation of material arrays from principal to local element directions

Constitutive equation(Using Voigt's notation):

:math:`\boldsymbol{\sigma} = \textbf{D} \boldsymbol{\epsilon}`

where

:math:`\boldsymbol{\sigma} = \begin{bmatrix}
\sigma_{11} & \sigma_{22} & \sigma_{33} & \sigma_{12} & \sigma_{23} & \sigma_{31}
\end{bmatrix}^{\textrm{T}}`

:math:`\boldsymbol{\epsilon} = \begin{bmatrix}
\epsilon_{11} & \epsilon_{22} & \epsilon_{33} & 2\epsilon_{12} & 2\epsilon_{23} & 2\epsilon_{31}
\end{bmatrix}^{\textrm{T}}`

Material array :math:`\textbf{D}` defined based on principal axes :math:`x_1x_2x_3`:

:math:`\textbf{D} = \begin{bmatrix}
d_{11} & d_{12} & d_{13} & & & \\
& d_{22} & d_{23} & & 0 & \\
& & d_{33} & & & \\
& & & g_{12} & & \\
& sym. & & & g_{23} & \\
& & & & & g_{31} \\
\end{bmatrix}`

Coefficient of thermal exoansion :math:`\boldsymbol{\alpha}` defined based on principal axes :math:`x_1x_2x_3`:

:math:`\boldsymbol{\alpha} = \begin{bmatrix}
\alpha_1 \\
\alpha_2 \\
\alpha_3 \\
0 \\
0 \\
0
\end{bmatrix}`

Thermal modulus :math:`\boldsymbol{\beta}` defined based on principal axes :math:`x_1x_2x_3`:

:math:`\boldsymbol{\beta} = \begin{bmatrix}
\beta_1 \\
\beta_2 \\
\beta_3 \\
0 \\
0 \\
0
\end{bmatrix}`

And they have the relationship:

:math:`\beta_i = d_{ij}\alpha_j \quad i,j = 1, 2, 3`


Condition 1: :math:`\psi`
--------------------------

:math:`\psi` describes the angle in degrees which the principal material axis 1 (i.e. :math:`x_1`) makes with the :math:`x` axis.

N.B. It is assumed that the principal material axis 3 (i.e. :math:`x_3`) coincides with the direction of the :math:`z` axis.

Rotation matrix :math:`\textbf{R}`:

:math:`\textbf{R} = \begin{bmatrix}
\cos^2\psi & \sin^2\psi & & \cos\psi\sin\psi & & \\
\sin^2\psi & \cos^2\psi & & -\cos\psi\sin\psi & & \\
& & 1 & & & \\
-2\cos\psi\sin\psi & 2\cos\psi\sin\psi & & \cos^2\psi - \sin^2\psi & & \\
& & & & \cos\psi & -\sin\psi \\
& & & & \sin\psi & \cos\psi \\
\end{bmatrix}`

Then, Material array :math:`\textbf{D}_{\textrm{local}}` based on local axes :math:`xyz`:

:math:`\textbf{D}_{\textrm{local}} = \textbf{R}^\textbf{T} \textbf{D} \textbf{R}`

Thermal modulus :math:`\boldsymbol{\beta}_{\textrm{local}}` based on local axes :math:`xyz`:

:math:`\boldsymbol{\beta}_{\textrm{local}} = \textbf{R}^\textbf{T} \boldsymbol{\beta}`

Condition 2: :math:`\textbf{v}_1`, :math:`\textbf{v}_2`
---------------------------------------------------------

:math:`\textbf{v}_1` and :math:`\textbf{v}_2` describe the orientation of the principal material axes which lie in the plane of the principal material axes 1 and 2.

Vectors :math:`\bar{\textbf{v}}_1`, :math:`\bar{\textbf{v}}_2` and :math:`\bar{\textbf{v}}_3` form a orthonormal triad.

Matrix :math:`\textbf{R}_0`:

:math:`\textbf{R}_0 = \begin{bmatrix}
\bar{v}_{11} & \bar{v}_{21} & \bar{v}_{31} \\
\bar{v}_{12} & \bar{v}_{22} & \bar{v}_{32} \\
\bar{v}_{13} & \bar{v}_{23} & \bar{v}_{33}
\end{bmatrix}`

where :math:`\bar{v}_{1i}`, :math:`\bar{v}_{2i}`, :math:`\bar{v}_{3i}` are components of vectors :math:`\bar{\textbf{v}}_1`, :math:`\bar{\textbf{v}}_2` and :math:`\bar{\textbf{v}}_3`.

Transformation matrix :math:`\textbf{R}`:

:math:`\textbf{R} = \begin{bmatrix}
\bar{v}_{11}^2 & \bar{v}_{12}^2 & \bar{v}_{13}^2 & \bar{v}_{11}\bar{v}_{12} & \bar{v}_{12}\bar{v}_{13} & \bar{v}_{11}\bar{v}_{13} \\
\bar{v}_{21}^2 & \bar{v}_{22}^2 & \bar{v}_{23}^2 & \bar{v}_{21}\bar{v}_{22} & \bar{v}_{22}\bar{v}_{23} & \bar{v}_{21}\bar{v}_{23} \\
\bar{v}_{31}^2 & \bar{v}_{32}^2 & \bar{v}_{33}^2 & \bar{v}_{31}\bar{v}_{32} & \bar{v}_{32}\bar{v}_{33} & \bar{v}_{31}\bar{v}_{33} \\
2\bar{v}_{11}\bar{v}_{21} & 2\bar{v}_{12}\bar{v}_{22} & 2\bar{v}_{13}\bar{v}_{23} & \bar{v}_{11}\bar{v}_{22}+\bar{v}_{13}\bar{v}_{21} & \bar{v}_{12}\bar{v}_{23}+\bar{v}_{13}\bar{v}_{22} & \bar{v}_{11}\bar{v}_{23}+\bar{v}_{13}\bar{v}_{21} \\
2\bar{v}_{21}\bar{v}_{31} & 2\bar{v}_{22}\bar{v}_{32} & 2\bar{v}_{23}\bar{v}_{33} & \bar{v}_{21}\bar{v}_{32}+\bar{v}_{22}\bar{v}_{31} & \bar{v}_{22}\bar{v}_{33}+\bar{v}_{23}\bar{v}_{32} & \bar{v}_{21}\bar{v}_{33}+\bar{v}_{23}\bar{v}_{31} \\
2\bar{v}_{11}\bar{v}_{31} & 2\bar{v}_{12}\bar{v}_{32} & 2\bar{v}_{13}\bar{v}_{33} & \bar{v}_{11}\bar{v}_{32}+\bar{v}_{12}\bar{v}_{31} & \bar{v}_{12}\bar{v}_{33}+\bar{v}_{13}\bar{v}_{32} & \bar{v}_{11}\bar{v}_{33}+\bar{v}_{13}\bar{v}_{31}
\end{bmatrix}`

Then, the transformation of geometrical points between the two coordinate systems are:

:math:`\begin{bmatrix}
x \\
y \\
z
\end{bmatrix} = \textbf{R}_0 \begin{bmatrix}
x_1 \\
x_2 \\
x_3
\end{bmatrix}`

Change the vector :math:`\boldsymbol{\beta}` (defined based on principal axes :math:`x_1x_2x_3` i.e. :math:`\beta_4 = \beta_5 = \beta_6 = 0`)

:math:`\boldsymbol{\beta} = \begin{bmatrix}
\beta_1 & \beta_2 & \beta_3 & \beta_4 & \beta_5 & \beta_6
\end{bmatrix}^\textbf{T}`

into matrix form :math:`\boldsymbol{\beta}`

:math:`\boldsymbol{\beta} = \begin{bmatrix}
\beta_1 & \beta_4 & \beta_6 \\
& \beta_2 & \beta_5 \\
sym. & & \beta_3
\end{bmatrix}`

Thermal modulus :math:`\boldsymbol{\beta}_{\textrm{local}}` based on local axes :math:`xyz`:

:math:`\boldsymbol{\beta}_{\textrm{local}} = \textbf{R}_0 \boldsymbol{\beta} \textbf{R}_0^\textbf{T}`

The transformation of material arrays:

:math:`\textbf{D}_{\textrm{local}} = \textbf{R}^\textbf{T} \textbf{D} \textbf{R}`

Reference
---------

* http://homes.civil.aau.dk/lda/Continuum/material.pdf
