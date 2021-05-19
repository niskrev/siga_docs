JPT (2011) investigate whether investment shocks are important drivers of business cycle fluctuations. To that end, and expanding on their previous work in JPT (2010), they estimate a New Keynesian model featuring imperfectly competitive goods and labor markets, as well as different nominal and real frictions such as sticky prices and wages, habit formation in consumption, variable capital utilization and investment adjustment costs. 

The model has eight structural shocks in total, with three technology shocks, two of which are related to investment. Specifically, JPT distinguish between final and intermediate consumption, investment, and capital goods, each being produced in a different sector. They introduce a shock that affects the transformation of consumption into investment goods, and another shock that affects the transformation of investment goods into productive capital. The first, called investment-specific technology (IST) shock, is introduced via the production function in the investment good producing sector:

$$
I_t = \Upsilon_t Y_t^I,
$$

where $I_t$ is the quantity of investment goods in efficiency units produced with $Y_t^I$ units of the final good. $\Upsilon_t$ represents the IST and is assumed to be a non-stationary random process growing at a rate $\upsilon_t$.

The second investment technology shock is introduced via the production technology in the capital good producing sector, which assumes that new capital, denoted with $i_t$, is produced from investment goods according to

$$
i_t = \mu_t \left(1 - S\left( \frac{I_t}{I_{t-1}}\right)\right)
$$

where $S$ is an investment adjustment cost function, and $\mu_t$ is a stationary shock to the marginal efficiency of investment (MEI), assumed to be an AR(1) process.

The third technology shocks affects the production functions in the intermediate good producing sector according to:

$$
Y_t(i) = \max \{ A_t^{1-\alpha} K_t(i)^{\alpha} L_t(i)^{1-\alpha} - A_t \Upsilon_t^{\frac{\alpha}{1-\alpha}} F; 0 \}
$$

where $Y_t(i)$, $K_t(i)$, and $L_t(i)$ are the quantities of output produced, and effective capital and labor employed by intermediate good producer $i$. $F$ represents fixed cost of production, and $A_t$ is a common  non-stationary neutral technology process, growing at rate $z_t$.

The final consumption good $Y_t$ is produced by combining a continuum of intermediate goods, according to

$$
Y_t = \left[ \int_{0}^{1} Y_t(i)^{\frac{1}{1+\lambda_{p,t}}} \right]^{1+\lambda_{p,t}}
$$

where $\lambda_{p,t}$ is a stationary price markup shock following ARMA(1,1) process.

Similarly to the model in the previous section, there is a shock to the intertemporal preferences of the households populating the economy whose lifetime utility function is given by

$$
\operatorname{E}_0 \sum_{t=0}^{\infty}\beta^t b_{t}\Bigg\{ \log\left(C_t - h C_{t-1}\right) - \varphi \frac{L_t(j)^{1+\nu}}{1+\nu} \Bigg\},
$$

where $C_t$ is consumption, $b_t$ is the stationary intertemporal preference shock, assumed to follow an AR(1) process. JPT assume that there is a continuum of households $j\in[0,1]$, each one being a supplier of specialized labor denoted by $L_t(j)$. The specialized labor in turn is combined into homogenous labor input according to

$$
L_t = \left[ \int_{0}^{1} L_t(i)^{\frac{1}{1+\lambda_{w,t}}} \right]^{1+\lambda_{w,t}}
$$

where $\lambda_{w,t}$ is a stationary wage markup shock assumed to follow an ARMA(1,1) process.

The last two shocks are to government fiscal and monetary policy. Public spending $G_t$ is a time-varying fraction of output,

$$
G_t = \left( 1 - \frac{1}{g_t} \right) Y_t
$$

where the government spending shock $g_{t}$ as a stationary AR(1) process.

Monetary policy consists of setting the nominal interest rate $R_t$ according to the following policy rule:

$$
\frac{R_t}{R} = \left( \frac{R_{t-1}}{R} \right)^{\rho_R}  \left[\left( \frac{\pi_{t}}{\pi}\right)^{\phi_{\pi}} \left( \frac{X_{t}}{X_t^{\ast}}\right)^{\phi_{X}} \right]^{1-\rho_R}  \left[\frac{X_t/X_{t-1}}{X^{\ast}_t/X^{\ast}_{t-1}} \right]^{\phi_{dX}} \varepsilon_{mp,t},
$$

where $e_{mp,t}$ is the monetary policy shock, $R$ is the steady state of the nominal rate, $\pi_t$ is the inflation rate, $X_t=C_t+I_t+G_t$ is actual real GDP and $X_t^{\ast}$ is the level of GDP under flexible prices and wages and in the absence of markup shocks.

To summarize, there are eight shocks in the model, six stationary and two non-stationary. Two of the stationary shocks -- to price and wage markups, follow ARMA(1,1) processes, and one -- to monetary policy, is an i.i.d process. The remaining stationary shocks -- to government spending, MEI, and intertemporal preferences, as well as the growth rates of the two non-stationary shocks -- to IST and neutral technology, follow AR(1) processes. The disturbances to all shocks are assumed to be Gaussian, leading to a linear Gaussian state space representation of the solution of log-linear approximation of model.

JPT estimate the model using US data on hours worked ($h_t=\log L_t$), inflation ($\pi_t$), the nominal interest rate ($R_t$), and the growth rates of GDP ($x_t= \triangle \log X_t$), consumption ($c_t= \triangle \log C_t$), investment ($i_t= \triangle \log I_t$), real wages ($w_t=\triangle \log \frac{W_t}{P_t}$), and the relative price of investment ($\pi^i_t=\triangle \log \frac{P_{It}}{P_t}$). Unlike Uribe (2021), they do not allow for measurement errors in any of the series. 