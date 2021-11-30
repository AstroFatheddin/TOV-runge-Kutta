# TOV-runge-Kutta
Solving the Tolman–Oppenheimer–Volkoff (TOV) equations for Polytropic Equations of State, Using the Runge-kutta 4th order method.
TOV Equation Solver by Python
by Hossein Fatheddin

This Program is written in Python in order to solve TOV Equations Using Runge-Kutta 4th order method:\\
$\epsilon = \epsilon_0 P^n (r)$ \\
$p = K \epsilon^{1+1/n} = p_0 P^{n+1} (r)$ \\
then the program will depend on 3 parameters:\\
$c=\frac{\epsilon_0}{p_0}$ , K and n.\\
I have used the TOV solving methods mentiond in references [1] , [2] and [3].\\
At the end there is a program to plot Mass - Distance and Pressure - Distance plots.\\
Also please note that here I have used units as $c = G = 1$ and in the main body, the dimensionless quantities are used.\\
EOS:\\
$\frac{dm}{dr}=4\pi \epsilon r^2$\\
$\frac{dp}{dr}=\frac{-(m(r)+4\pi \epsilon r^3)(\epsilon +p)}{(1+2\frac{m(r)}{r})r^2}$\\
Dimensionless quantities:\\
$M=m\sqrt{\epsilon_0}$\\
$R=r\sqrt{\epsilon_0}$\\
NEW EOS:\\
$\frac{dM}{dR}=4\pi R^2P^n(r)$
$\frac{dP}{dR}=\frac{-c+PM(R)+4\pi R^3 \frac{P^{n+1}}{c}}{(n+1)R(R-2M(R))}$
With Initial Conditions: M(0)=0 & P(0)=1
