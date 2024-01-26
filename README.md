The complex index of refraction (or optical constant, $\\tilde{\eta}$ )  is an important property of materials that determines their interaction with light. $\\tilde{\eta}$ is formed by a real ($\\eta$) and an imaginary ($\\kappa$) parts that are both functions of the wavelength ($\\lambda$) so that
$\\tilde{\eta} = \eta + i\kappa$.<br>
Firstly, the $\\kappa$ can be calculated from the absorption coefficient, $\\alpha$, in base $e$ (Napierian):


$$ \kappa(\lambda) = \frac{\lambda\alpha(\lambda)}{4\pi} $$


Posteriorly, the K-K relation enables then an affordable way to find $\\eta$ from $\\kappa$:


$$ \eta(\lambda_i) = \eta_{offset} + \frac{2}{\pi} PV \int_{\lambda_{L}}^{\lambda_{U}} \frac{\lambda\kappa(\lambda)d\lambda}{\lambda^{2} - \lambda_i^{2}}, \lambda_{L} \leq \lambda_{i} \leq \lambda_{U} $$


where PV denotes the Cauchy principal value, $\\lambda_{L}$ and $\\lambda_{U}$ are the lower and upper bounds. To minimize the errors in the calculation of $\\eta(\lambda)$, the constant boundary extension procedure can be applied, so that $\\alpha(\\lambda) = \\alpha(\\lambda_{L})$ for $\\lambda \\leq \\lambda_{L}$ and $\\alpha(\\lambda) = \\alpha(\\lambda_{U})$ for $\\lambda \\geq \\lambda_{U}$. Note that the index of refraction was shifted by a constant value, where $\\eta_{offset} \\geq 1$.  In relation to $\\eta_{offset}$,  it is typically found to closely resemble the refractive index at the point of minimum dispersion, or a point in close proximity within the transparency region between the infrared and UV/Vis spectral range. In the transparency region $\\kappa$ is negligible and $\\eta_{offset}=\\sqrt{\\varepsilon_{r}}$, where in this specific circumstance $\\varepsilon_{r}$ is often called relative dielectric constant of the medium.


Note that the complex relative permittivity of the medium is given by: 


$$ \varepsilon_{r} = \varepsilon_{r}' - i\varepsilon_{r}'' $$


where


$$ \varepsilon_{r}' = \eta^{2} - \kappa^{2} $$


and


$$ \varepsilon_{r}'' = 2\eta\kappa $$


**Observaton:** In most works, the absorption coefficient spectrum presented by the researchers is decadic (units: $\ cm^{-1}$). The relationship between the base $e$ (Napierian) absorption coefficient, $\\alpha$, and the base $\ 10$ (decadic) absorption coefficient, $a$, is given by: 
$\\alpha = a \times ln(10)$. The absorption coefficient in the base $\ 10$ will be used as an input parameter in our software because it is more frequently used in the literature.


Detailed instructions for using RI-Calc can be consulted in our published article:


**RI−Calc: A User Friendly Software and Web Server for Refractive Index Calculation, Computer Physics Communications, 2024, 109100.** 


 [![DOI:10.1016/j.cpc.2024.109100](https://img.shields.io/badge/DOI-10.1016/j.cpc.2024.109100-B31B1B.svg)](https://doi.org/10.1016/j.cpc.2024.109100)


**The preprint of this article is available for download:** [here](https://github.com/NanoCalc/PLQ-Sim/blob/main/PLQ-Sim.pdf).


**The software binaries can be downloaded for the following operating systems:** [*Unix-like systems (Linux)*](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/RICalc_3_0_Unix.zip), [*Windows*](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/RICalc_3_0_Windows.zip) and [*macOS*](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/RICalc_3_0_MacOS.zip).<br> 


Program interface:
<p align="center">  
  <img width="500em" src="https://github.com/NanoCalc/RICalc/assets/34662089/3c988d90-1980-49d0-8f20-cf689a9a7e15" />
</p>


`RI-Calc` can also be used online on our website [nanocalc.org/ricalc](https://nanocalc.org/ricalc).


Test the app using [sample data](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/data_sample.zip).


More spectral data for testing the app can be downloaded [here](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/spectral-data.zip).


Find out more about our research groups: [*DiNE*](https://dineufpr.wixsite.com/dineufpr) and [*NAMOR*](http://sites.if.ufrj.br/namor/).


# Authors
* [Leandro Benatto](https://orcid.org/0000-0001-9976-3574)<sup>a,b</sup>
* [Omar Mesquita](https://orcid.org/0000-0002-6656-5683)<sup>a</sup>
* [Lucimara S. Roman](https://orcid.org/0000-0001-6567-5920)<sup>b</sup>
* [Marlus Koehler](https://orcid.org/0000-0001-9935-5060)<sup>b</sup>
* [Rodrigo B. Capaz](https://orcid.org/0000-0001-5770-5026)<sup>a,c</sup>
* [Graziâni Candiotto](https://orcid.org/0000-0001-6755-660X)<sup>a</sup>


# Institutions
<sup>a</sup>Institute of  Physics, Federal University of Rio de Janeiro, 21941-909, Rio de Janeiro-RJ, Brazil.<br> [UFRJ](https://pos.if.ufrj.br/pt/)


<sup>b</sup>Department of Physics, Federal University of Paraná, 81531-980, Curitiba-PR, Brazil.<br> [UFPR](http://fisica.ufpr.br/posgrad/)


<sup>c</sup>Brazilian Nanotechnology National Laboratory (LNNano), Brazilian Center for Research in Energy and Materials (CNPEM), 13083-100, Campinas- SP, Brazil.<br/> [LNNano](https://lnnano.cnpem.br/en/home-en/)


# Developers
* [Leandro Benatto](https://github.com/LeandroBenatto)
* [Omar Mesquita](https://github.com/OmarMesqq)
* [Graziâni Candiotto](https://github.com/gcandiotto)


# Data Sample
* The [`Data Sample`](https://github.com/NanoCalc/RICalc/tree/main/Data%20Sample) folder contains an example of the data set needed to run `RICalc`.<br> 
You can download it [here](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/data_sample.zip)


# Spectral Data
In the [`Spectral Data`](https://github.com/NanoCalc/RICalc/tree/main/Spectral%20Data) folder, you will find additional data that can be used to obtain the refractive index of different materials.


You can also directly download them [here](https://github.com/NanoCalc/RICalc/releases/download/3.0-beta/spectral-data.zip).
