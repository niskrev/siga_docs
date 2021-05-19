### Spectral decomposition of the information about latent variables in dynamic macroeconomic models 

<br/><br/>

#### Abstract
In this paper, I show how to perform spectral decomposition of the information about latent variables in dynamic economic models. A model describes the joint probability distribution of a set of observed and latent variables. The amount of information transferred from the former to the latter is measured by the reduction of uncertainty in the posterior compared to the prior distribution of any given latent variable. Casting the analysis in the frequency domain allows decomposing the total amount of information in terms of frequency-specific contributions as well as in terms of information contributed by individual observed variables. I illustrate the usefulness of the proposed methodology with applications to two DSGE models taken from the literature.
<br/>
<br/>

#### Information gain measures
<br/>

* the **information gain** at frequency $\omega$ measures the reduction of uncertainty about $x$ at a given frequency $\omega$ due to information from $\mathbf{y}$ at that frequency.

$$
\mathrm{IG}_{\mathbf{y} \rightarrow x} (\omega)  =  \left( \frac{f_{x x}(\omega) -  f_{x \lvert \mathbf{y}}(\omega) }{f_{xx}(\omega)} \right) \times 100
$$

where $f_{x \lvert \mathbf{y}}(\omega) = f_{x x}(\omega) - f_{x \mathbf{y}}(\omega) f_{\mathbf{y}\mathbf{y}}^{-1}(\omega) f_{\mathbf{y} x}(\omega)$ is the partial spectrum of $x$ given $\mathbf{y}$
<br/>

* the **conditional information gain** at frequency $\omega$ measures the additional reduction of uncertainty about $x$ at a given frequency $\omega$ due to information from $\mathbf{y_1}$ which is not in $\mathbf{y_2}$

$$
\mathrm{IG}_{\mathbf{y}_{{}_1} \rightarrow x \lvert \mathbf{y}_{{}_2}} (\omega)  =  \left( \frac{f_{x  \vert \mathbf{y}_{{}_2}}(\omega) -  f_{x \lvert \mathbf{y}}(\omega) }{f_{xx}(\omega)} \right) \times 100
$$

<br/>

Similarly, the **integrated** unconditional and conditional information gain measures over a band of frequencies $\mathbf{\omega} = \{\omega: \omega \in [\underline{\omega},\overline{\omega}] \cup [-\overline{\omega}, -\underline{\omega}] \}$ are given by

$$
\mathrm{IG}_{\mathbf{y} \rightarrow x} (\mathbf{\omega})  =  \left( \frac{f_{x x}(\mathbf{\omega}) -  f_{x \lvert \mathbf{y}}(\mathbf{\omega}) }{f_{xx}(\mathbf{\omega})} \right) \times 100 
$$

$$
\mathrm{IG}_{\mathbf{y}_{{}_1} \rightarrow x \lvert \mathbf{y}_{{}_2}} (\mathbf{\omega})  =  \left( \frac{f_{x  \vert \mathbf{y}_{{}_2}}(\mathbf{\omega}) -  f_{x \lvert \mathbf{y}}(\mathbf{\omega}) }{f_{xx}(\mathbf{\omega})} \right) \times 100 
$$

where $\displaystyle{f_{xx}(\mathbf{\omega})  =  \int_{\omega \in \mathbf{\omega}}f_{xx}(\omega) \mathrm{d} \omega}$, and $\displaystyle{f_{x \lvert \mathbf{y}}(\mathbf{\omega})  =  \int_{\omega \in \mathbf{\omega}} f_{x \lvert \mathbf{y}}(\omega) \mathrm{d} \omega}$.
<br/>
<br/>

#### Information complementarity measures
<br/>

* the **information complementarity** between variables $y_1$ and $y_2$ conditional on variables $\mathbf{y}_{3} \subset \{ \mathbf{y} \setminus \mathbf{y}_{12} \}$ at frequency band $\mathbf{\omega}$ is defined as:

$$
\mathrm{IC}_{\mathbf{y}_{{}_{12}}\rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) = \frac{\mathrm{IG}_{\mathbf{y}_{{}_{12}} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega})}{\mathrm{IG}_{y_{{}_1} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) + \mathrm{IG}_{y_{{}_2} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega})} - 1.
$$

Negative values indicate negative complementarity, or information redundancy, between $y_1$ and $y_2$, and positive values indicate positive complementarity between the two variables. Since the information gain is non-negative, we have $\mathrm{IC}_{\mathbf{y}_{{}_{12}}\rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) \geq -1/2$, with equality when $y_1$ and $y_2$ are (conditionally on $\mathbf{y}_3$) functionally dependent, in which case $\mathrm{IG}_{\mathbf{y}_{{}_{12}} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) = \mathrm{IG}_{y_{{}_1} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) = \mathrm{IG}_{y_{{}_2} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega})$. A lack of information complementarity, i.e. $\mathrm{IC}_{\mathbf{y}_{{}_{12}}\rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega})=0$ occurs when $y_1$ and $y_2$ are (conditionally on $\mathbf{y}_3$) independent, and hence $\mathrm{IG}_{\mathbf{y}_{{}_{12}} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) = \mathrm{IG}_{y_{{}_1} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega}) + \mathrm{IG}_{y_{{}_2} \rightarrow x \lvert \mathbf{y}_{{}_3}}(\mathbf{\omega})$. Note that the conditioning could be with respect to any subset of observables, including the empty set, in which case we have unconditional complementarity between $y_1$ and $y_2$.
