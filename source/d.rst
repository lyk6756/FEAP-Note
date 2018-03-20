``d(*)``： Material Parameters
=================================

:math:`\begin{array}{rll}
\hline
\textrm{Parameter} & \textrm{Name} & \textrm{Description} \\
\hline
1   & E         & \textrm{Young's modulus} \\
2   & \nu       & \textrm{Poisson ratio} \\
3   & \alpha    & \textrm{Thermal expansion coefficient} \\
4   & \rho      & \textrm{Mass density} \\
5   & -         & \textrm{Quadrature order for arrays} \\
6   & -         & \textrm{Quadrature order for outputs} \\
7   & a         & \textrm{Mass interpolation} (a = 0: \textrm{Diagonal}; a = 1: \textrm{Consistent})\\
8   & q         & \textrm{Loading intensity (plates/shells)} \\
9   & T_0       & \textrm{Stress free reference temperature} \\
10  & \kappa    & \textrm{Shear factor (plates/shells/beams)} \\
11  & b_1       & \textrm{Body force/volume in 1-directions} \\
12  & b_2       & \textrm{Body force/volume in 2-directions} \\
13  & b_3       & \textrm{Body force/volume in 3-directions} \\
14  & h         & \textrm{Thickness (plates/shells)} \\
15  & \texttt{nh1}   & \textrm{History variable counter} \\
16  & \texttt{stype} & \textrm{Two dimensional type: 1 - plane stress; 2 - plane strain; 3 - axisymmetric} \\
17  & \texttt{etype} & \textrm{Element formulation: 1 - displ; 2 - mixed; 3 - enhanced} \\
18  & \texttt{dtype} & \textrm{Deformation type: <0 - finite; >0 - small} \\
19  & \texttt{tdof}  & \textrm{Thermal degree-of-freedom} \\
20  & \texttt{imat}  & \textrm{Non-linear elastic material type} \\
21  & d_{11}    & \textrm{Material moduli} \\
22  & d_{22}    & \textrm{Material moduli} \\
23  & d_{33}    & \textrm{Material moduli} \\
24  & d_{12}    & \textrm{Material moduli} \\
25  & d_{23}    & \textrm{Material moduli} \\
26  & d_{31}    & \textrm{Material moduli} \\
27  & g_{12}    & \textrm{Material moduli} \\
28  & g_{23}    & \textrm{Material moduli} \\
29  & g_{31}    & \textrm{Material moduli} \\
30  & C         & \textrm{Fung pseudo elastic model modulus} \\
31  & \psi      & \textrm{Orthotropic angle} x_1 \textrm{principal axis 1} \\
32  & A         & \textrm{Area cross section (beam/truss)} \\
33  & I_{11}    & \textrm{Inertia cross section (beam/truss)} \\
34  & I_{22}    & \textrm{Inertia cross section (beam/truss)} \\
35  & I_{12}    & \textrm{Inertia cross section (beam/truss)} \\
36  & J         & \textrm{Polar inertia cross section (beam/truss)} \\
37  & \kappa_1  & \textrm{Shear factor plate} \\
38  & \kappa_2  & \textrm{Shear factor plate} \\
39  & -         & \textrm{Non-linear flag (beam/truss)} \\
40  & -         & \textrm{Inelastic material model type} \\
41  & Y_0       & \textrm{Initial yield stress (Mises)} \\
42  & Y_{\infty} & \textrm{Final yield stress (Mises)} \\
43  & \beta     & \textrm{Exponential hardening rate} \\
44  & H_{iso}   & \textrm{Isotropic hardening modulus (linear)} \\
45  & H_{kin}   & \textrm{Kinematic hardening modulus (linear)} \\
46  & -         & \textrm{Yield flag} \\
47  & \beta_1   & \textrm{Orthotropic thermal stress} \\
48  & \beta_2   & \textrm{Orthotropic thermal stress} \\
49  & \beta_3   & \textrm{Orthotropic thermal stress} \\
50  & -         & \textrm{Error estimator parameter} \\
51  & \nu_1     & \textrm{Viscoelastic shear parameter} \\
52  & \tau_1    & \textrm{Viscoelastic relaxation time} \\
53  & \nu_2     & \textrm{Viscoelastic shear parameter} \\
54  & \tau_2    & \textrm{Viscoelastic relaxation time} \\
55  & \nu_3     & \textrm{Viscoelastic shear parameter} \\
56  & \tau_3    & \textrm{Viscoelastic relaxation time} \\
57  & \texttt{nvis} & \textrm{Number of viscoelastic terms (1-3)} \\
58  & -         & \textrm{Damage limit} \\
59  & -         & \textrm{Damage rate} \\
60  & k         & \textrm{Penalty parameter} \\
61  & K_1       & \textrm{Fourier thermal conductivity} \\
62  & K_2       & \textrm{Fourier thermal conductivity} \\
63  & K_3       & \textrm{Fourier thermal conductivity} \\
64  & c         & \textrm{Fourier specific heat} \\
65  & \omega    & \textrm{Angular velocity} \\
66  & Q         & \textrm{Body heat} \\
67  & -         & \textrm{Heat constitution added indicator} \\
68  & -         & \textrm{Follower loading indicator} \\
69  & -         & \textrm{Rotational mass factor} \\
70  & -         & \textrm{Damping factor} \\
71  & g_1       & \textrm{Ground acceleration factor} \\
72  & g_2       & \textrm{Ground acceleration factor} \\
73  & g_3       & \textrm{Ground acceleration factor} \\
74  & p_1       & \textrm{Ground acceleration proportional load number} \\
75  & p_2       & \textrm{Ground acceleration proportional load number} \\
76  & p_3       & \textrm{Ground acceleration proportional load number} \\
77  & a_0       & \textrm{Rayleigh damping mass ratio} \\
78  & a_1       & \textrm{Rayleigh damping stiffness ratio} \\
79  & -         & \textrm{Plate/Shell/Rod shear activation flag} \\
80  &           & \textrm{Method: Type 1} \\
81  &           & \textrm{Method: Type 2} \\
82  & -         & \textrm{Truss/Rod quadrature number} \\
83  & -         & \textrm{Axial loading value} \\
84  & -         & \textrm{Constitutive start indicator} \\
85  & -         & \textrm{Polar angle indicator} \\
\end{array}`

:math:`\begin{array}{rll}
86  & -         & \textrm{Polar angle coord 1} \\
87  & -         & \textrm{Polar angle coord 2} \\
88  & -         & \textrm{Polar angle coord 3} \\
89  & -         & \textrm{Constitution transient type} \\
90  & d_{31}    & \textrm{Plane stress recovery} \\
91  & d_{32}    & \textrm{Plane stress recovery} \\
92  & \alpha_3  & \textrm{Plane stress recovery} \\
93  & \texttt{sref} & \textrm{Shear center type} \\
94  & y_1       & \textrm{Shear center coordinate} \\
95  & y_2       & \textrm{Shear center coordinate} \\
96  & \texttt{lref} & \textrm{Reference vector type} \\
97  & n_1       & \textrm{Reference vector parameter} \\
98  & n_2       & \textrm{Reference vector parameter} \\
99  & n_3       & \textrm{Reference vector parameter} \\
100 & -         & \textrm{Cross section shape type: 1 - rectangles; 2 - tube; 3 - Wide flange;} \\
&           & \textrm{4 - Channel; 5 - Angle; 6 - Circle} \\
101-126 & -     & \textrm{Shape data} \\
127 & -         & \textrm{Surface convection} (h) \\
128 & -         & \textrm{Free-stream temperature} (T_{\infty}) \\
129 & -         & \textrm{Reference absolute temperature} \\
130 & \texttt{nseg} & \textrm{Number of hardening segments} \\
131-148 & -     & \textrm{Segment data sets} e_pY_{iso}H_{kin} \\
149 & -         & \textrm{Total variables on frame section} \\
150 & -         & \textrm{Piezoelectric flag} \\
151-159 & -     & \textrm{Piezoelectric data} \\
160 & -         & \textrm{Initial stress flag} \\
161-166 & \sigma_{ij} & \textrm{Initial stresses (constant)} \\
167 & -         & \textrm{Tension/compression only indicator} \\
168 & -         & \textrm{Thermal activation indicator} \\
169 & -         & \textrm{Mechanical activation indicator} \\
170 & -         & \textrm{Volume model number (default 1)} \\
171 & a_1       & \textrm{Fung model energy parameter} \\
172 & a_2       & \textrm{Fung model energy parameter} \\
173 & a_3       & \textrm{Fung model energy parameter} \\
174 & a_4       & \textrm{Fung model energy parameter} \\
175 & a_5       & \textrm{Fung model energy parameter} \\
176 & a_6       & \textrm{Fung model energy parameter} \\
177 & a_7       & \textrm{Fung model energy parameter} \\
178 & a_8       & \textrm{Fung model energy parameter} \\
179 & a_9       & \textrm{Fung model energy parameter} \\
180-181 & -     & \textrm{Viscoplastic rate parameters} \\
182 & -         & \textrm{Nodal quadrature parameters} \\
183 & \beta_m   & M_L - M_C \textrm{mass scaling factor} \\
184 & c         & \textrm{Estimate on maximum wave speed} \\
185 & -         & \textrm{Augmentation switch: <on/off>} \\
186 & -         & \textrm{Augmentation explicit indicator} \\
187 &           & \textrm{Implicit = 0; Explicit = 1 element integration} \\
188 & -         & \textrm{Number stress components in rod elements} \\
189 & -         & \textrm{Nurbs and VEM flag} \\
190-192 & -     & \textrm{Nurbs quadrature values/direction} \\
193 & \texttt{tmat}   & \textrm{Thermal material numbers} \\
194 & \texttt{ietype} & \textrm{Element type} \\
195 & T - frac  & \textrm{Fraction of work to heat} \\
196 & q - prop  & \textrm{Proportional load factor for pressure loading} \\
197-198 & -     & \textrm{Body patch loading values} \\
199 & -         & \textrm{Axisymmetric 1-d: Plane stress in thickness} \\
200 & \texttt{nsiz}   & \textrm{Size of modulus or compliance array} \\
201-236 & -     & \textrm{Anisotropic Modulus or Compliance array} \\
237 & -         & \textrm{Number of element global equations} \texttt{nge} \\
238 & -         & \textrm{Partition of element global equations} \\
239 & -         & \textrm{Unused} \\
240 & -         & \textrm{0 - Element based; 1 - nodal based formulation} \\
241 & -         & \textrm{Number of active element degrees of freedom} \\
242-248 & V_1, V_2    & \textrm{Plastic Vector orientation} \\
249-255 & -     & \textrm{Reference vector types and values} \\
260-279 & \texttt{nstv} & \textrm{Number structure vectors/values} \\
280-282 & g_i   & \textrm{Thermal-elastic temperature function} \\
283 & -         & \textrm{Unused} \\
283-286 & -     & \textrm{Delete element data} \\
287 & -         & \textrm{Total energy computation switch} \\
288 & -         & \textrm{Shell thickness change flag} \\
289 & -         & \textrm{Rate switch (on=0,off=1)} \\
290-293 & -     & \textrm{Constitutive equation coordinate frame} \\
294 & -         & \textrm{Rotatory inertia on/off flag} \\
295-296 & -     & \textrm{Body force user parameters} \\
\hline
\textrm{Parameter} & \textrm{Name} & \textrm{Description} \\
\hline
\end{array}`


Reference
---------

* `FEAP Programmer Manual: v8.5 <http://projects.ce.berkeley.edu/feap/pmanual85.pdf>`_
