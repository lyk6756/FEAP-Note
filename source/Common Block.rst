Common Block Definitions
=============================


:math:`\begin{array}{lll}
\hline
\textrm{Block Name} & \textrm{Variable} & \textrm{Definition} \\
\hline
\texttt{bdata} & \texttt{o} & \textrm{Page eject option} \\
& \texttt{head} & \textrm{Title record} \\
\hline
\texttt{cdat1} & \texttt{ndd} & \textrm{Size of program material parameters} \ \texttt{d(ndd, nummat)} \\
& \texttt{nie} & \textrm{Size of element control array} \ \texttt{ie(nie, nummat)} \\
& \texttt{nud} & \textrm{Size of user material parameters} \ \texttt{ud(*)} \\
\hline
\texttt{cdata} & \texttt{numnp} & \textrm{Number of mesh nodes} \\
& \texttt{numel} & \textrm{Number of mesh elements} \\
& \texttt{nummat} & \textrm{Number of material sets} \\
& \texttt{nen} & \textrm{Maximum nodes/element} \\
& \texttt{neq} & \textrm{Number active equations} \\
& \texttt{ipr} & \textrm{Real variable precision} \\
\hline
\texttt{comblk} & \texttt{hr} & \textrm{Real array data} \\
& \texttt{mr} & \textrm{Integer array data} \\
\hline
\texttt{elcoor} & \texttt{xref} & \textrm{Reference coordinates for the constitutive point} \\
& \texttt{xcur} & \textrm{Current coordinates for the constitutive point} \\
\hline
\texttt{counts} & \texttt{nstep} & \textrm{Total number of time steps} \\
& \texttt{niter} & \textrm{Number of iterations current step} \\
& \texttt{naugm} & \textrm{Number of augments current step} \\
& \texttt{titer} & \textrm{Total iterations} \\
& \texttt{taubm} & \textrm{Total augments} \\
& \texttt{iaugm} & \textrm{Augmenting counter} \\
& \texttt{iform} & \textrm{Number residuals in line search} \\
\hline
\texttt{eldata} & \texttt{dm} & \textrm{Element proportional load} \\
& \texttt{n_el} & \textrm{Current element number} \\
& \texttt{ma} & \textrm{Current element material set} \\
& \texttt{mct} & \textrm{Print counter} \\
& \texttt{iel} & \textrm{User element number} \\
& \texttt{nel} & \textrm{Number nodes on current element} \\
\hline
\texttt{elplot} & \texttt{tt} & \textrm{Element stress values for} \ \texttt{TPLOt} \\
\hline
\texttt{eltran} & \texttt{bpr} & \textrm{Principal stretch} \\
& \texttt{ctan} & \textrm{Element multipliers} \\
\hline
\texttt{eluser} & \texttt{ut} & \textrm{Element user values for} \ \texttt{TPLOt} \\
\hline
\texttt{hdata} & \texttt{nh1} & \textrm{Pointer to} \ t_n \ \textrm{history data} \\
& \texttt{nh2} & \textrm{Pointer to} \ t_{n+1} \ \textrm{history data} \\
& \texttt{nh3} & \textrm{Pointer to element history} \\
\hline
\texttt{iofile} & \texttt{ior} & \textrm{Current input logical unit} \\
& \texttt{iow} & \textrm{Current output logical unit} \\
\hline
\texttt{pointer} & \texttt{np} & \textrm{Pointer for standard program array} \\
& \texttt{up} & \textrm{Pointer for user defined array} \\
\hline
\texttt{prstrs} & \texttt{nph} & \textrm{Pointer to global projection arrays} \\
& \texttt{ner} & \textrm{Pointer to global error indicator} \\
& \texttt{erav} & \textrm{Element error value} \\
& \texttt{j-int} & \textrm{J integral values} \\
\hline
\texttt{qudshp} & \texttt{jac} & \textrm{Jacobian matrix determinant at points} \\
& \texttt{lint} & \textrm{Number of quadrature points} \\
& \texttt{sg1} & \textrm{Points natural coordinates and weights in 1D} \\
& \texttt{shp1} & \textrm{Shape functions and derivatives of points in 1D} \\
& \texttt{sg2} & \textrm{Points natural coordinates and weights in 2D} \\
& \texttt{el2} & \textrm{Points natural area coordinates and weights in 2D} \\
& \texttt{shp2} & \textrm{Shape functions and derivatives of points in 2D} \\
& \texttt{sg3} & \textrm{Points natural coordinates and weights in 3D} \\
& \texttt{el3} & \textrm{Points natural volume coordinates and weights in 3D} \\
& \texttt{shp3} & \textrm{Shape functions and derivatives of points in 3D} \\
\hline
\texttt{sdata} & \texttt{ndf} & \textrm{Maximum dof/node} \\
& \texttt{ndm} & \textrm{Mesh space dimension} \\
& \texttt{nen1} & \textrm{Dimension 1 on IX array} \\
& \texttt{nst} & \textrm{Size of element matrix} \\
& \texttt{nneq} & \textrm{Total dof in problem} \\
\hline
\texttt{tdata} & \texttt{ttim} & \textrm{Current time} \\
& \texttt{dt} & \textrm{Current time increment} \\
& \texttt{ci} & \textrm{Integration parameters} \\
\hline
\end{array}`
