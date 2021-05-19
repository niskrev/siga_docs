_Uribe (2021)_ investigates the nature and empirical importance of monetary policy shocks that produce neo-Fisherian dynamics, i.e. move interest rates and inflation in the same direction over the short run. To that end, the author estimates a standard small-scale New-Keynesian model with price stickiness and habit formation, augmented with seven structural shocks. Full details about the model can be found in the original publication. Here I only describe those of its features that are directly relevant for the analysis which follows.

Firstly, three of the shocks are to monetary policy, which is described by the following policy rule:
$$
\frac{1+I_t}{\Gamma_t} = \left[A \left(\frac{1 + \Pi_t}{\Gamma_t} \right)^{\alpha_t} \left(\frac{Y_t}{X_t} \right)^{\alpha_{y}} \right]^{1-\gamma_I} \left(\frac{1 + I_{t-1}}{\Gamma_{t-1}} \right)^{\gamma_I} e^{z_t^{m}},
$$
where $I_t$ the nominal interest rate,  $Y_t$ is aggregate output, $\Pi_t$ is the inflation rate, $\Gamma_t$ is the inflation-target, $X_t$ is a nonstationary productivity shocks, and $z_t^{m}$ is a stationary interest-rate shock. The inflation target is defined as
$$
\Gamma_t = X_t^m e^{z_t^{m2}},
$$
where $X_t^m$ and $z_t^{m2}$ are permanent and transitory components of the inflation target. It is assumes that $X_t^m$ and $X_t$ grow at a rates $g^m_t$ and $g_t$, respectively.

There are two preference shocks affecting the lifetime utility function of the representative household, given by
$$
\E_0 \sum_{t=0}^{\infty}\beta^t e^{\xi_t}\Bigg\{ \frac{\left[\left(C_t - \delta \tilde{C}_{t-1}\right) \left(1-e^{\theta_t}h_t \right)^{\chi} \right]^{1-\sigma} - 1}{1-\sigma} \Bigg\},
$$
where $C_t$ is consumption, $\tilde{C}_t$ is the cross sectional average of consumption, $h_t$ is hours worked, $\xi_t$ is an intertemporal preference shock, and $\theta_t$ is a shock to labor supply.

In addition to $X_t$, there is also a stationary productivity shock $z_t$, which affects the production technology according to
$$
Y_t = e^{z_t}X_t h_t^{\alpha},
$$

The five stationary shocks ($\xi_t$, $\theta_t$, $z_t$, $z_t^{m}$, and $z_t^{m2}$ ) and the growth rates of the two non-stationary shocks ($g_t$ and $g^m_t$) are all assumed to follow first-order autoregressive processes.

Uribe (2021) estimates the model using quarterly US data on three variables: per capita output growth ($\triangle y_t$), the interest-rate-inflation differential ($r_t=i_t - \pi_t$), and the change in the nominal interest rate ($\triangle i_t$). All variables are assumed to be observed with measurement errors. Thus, there are ten independent sources of randomness in the data and only three observables. Clearly, not all, if any,  of the latent variables can be recovered fully. The purpose of the remainder of this section is to determine how well each structural shock can be recovered and where in the spectrum most of the information comes from, as well as what are the information contributions of different observed variables overall and across different frequency bands.