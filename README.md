

**Refractive Index Calculator (`RI-Calc`)** is a user-friendly software that applies the Kramers-Kronig (K-K) relations to calculate the refractive index of mixed organic compounds, molecules, polymers, perovskites, and inorganic compounds. The program can be used when ellipsometric measurements are unavailable, which is the case
in many laboratories. 

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

**The software binaries can be downloaded for the following operating systems:** [*Unix-like systems (Linux)*](https://github.com/NanoCalc/RICalc/releases/download/2.0-beta/RICalc-Unix.zip), [*Windows*](https://github.com/NanoCalc/RICalc/releases/download/2.0-beta/RICalc-Windows.zip) and [*macOS*](https://github.com/NanoCalc/RICalc/releases/download/2.0-beta/RICalc-MacOS.zip).<br> 

Program interface:
<p align="center">  
  <img width="500em" src="https://raw.githubusercontent.com/NanoCalc/ri-src/main/res/background.png?token=GHSAT0AAAAAACGBCJECMDFADGBSN3AJYQC6ZGRPELA" />
</p>

`RI-Calc` can also be used online on our website [nanocalc.org/ricalc](https://nanocalc.org/ricalc).

Test the app using [sample data](https://github.com/NanoCalc/RICalc/releases/download/1.0-beta/data-sample.zip).

Find out more about our research groups: [*DiNE*](https://dineufpr.wixsite.com/dineufpr) and [*NAMOR*](http://sites.if.ufrj.br/namor/).

# Authors
* [Leandro Benatto](https://orcid.org/0000-0001-9976-3574)<sup>a,b</sup>
* [Omar Mesquita](https://orcid.org/0000-0002-6656-5683)<sup>a</sup>
* [Lucimara S. Roman](https://orcid.org/0000-0001-6567-5920)<sup>b</sup>
* [Marlus Koehler](https://orcid.org/0000-0001-9935-5060)<sup>b</sup>
* [Rodrigo B. Capaz](https://orcid.org/0000-0001-5770-5026)<sup>a,c</sup>
* [Graziâni Candiotto](https://orcid.org/0000-0001-6755-660X)<sup>a</sup>

# Institutions
<sup>a</sup>Institute of  Physics, Federal University of Rio de Janeiro, 21941-909, Rio de Janeiro-RJ, Brazil.<br>
<sup>b</sup>Department of Physics, Federal University of Paraná, 81531-980, Curitiba-PR, Brazil.<br>
<sup>c</sup>Brazilian Nanotechnology National Laboratory (LNNano), Brazilian Center for Research in Energy and Materials (CNPEM), 13083-100, Campinas- SP, Brazil.<br/>

# Developers
* [Leandro Benatto](https://github.com/LeandroBenatto)
* [Omar Mesquita](https://github.com/OmarMesqq)
* [Graziâni Candiotto](https://github.com/gcandiotto)

# Data Sample
* The [`Data Sample`](https://github.com/NanoCalc/RICalc/tree/main/Data%20Sample) folder contains an example of the data set needed to run `RICalc`.<br> 
You can download it [here](https://github.com/NanoCalc/RICalc/releases/download/1.0-beta/data-sample.zip)

# Spectral Data
In the [`Spectral Data`](https://github.com/NanoCalc/RICalc/tree/main/Spectral%20Data) folder, you will find additional data that can be used to obtain the refractive index of different materials.

You can also directly download them [here](https://github.com/NanoCalc/RICalc/releases/download/1.0-beta/Spectral.Data.tar.gz).


# Acknowledgments
The authors acknowledge financial support from LCNano/SisNANO 2.0 (grant 442591/2019-5). L.B. (grant E-26/202.091/2022 process 277806), O.M. (grant E-26/200.729/2023 process 285493) and G.C. (grant E-26/200.627/2022 and E-26/210.391/2022 process 271814) are greatfully for financial support from FAPERJ. The authors also acknowledge the computational support of Núcleo Avançado de Computação de Alto Desempenho (NACAD/COPPE/UFRJ), Sistema Nacional de Processamento de Alto Desempenho (SINAPAD) and Centro Nacional de Processamento de Alto Desempenho em São Paulo (CENAPAD-SP) and technical support of SMMOL - solutions in functionalyzed materials.

# Cited by

Papers that recently cited `RICalc` are shown below.
<!-- [![DOI:<your number>](http://img.shields.io/badge/DOI-<your number>-<colour hexcode>.svg)](<doi link>) -->
<!-- exemplo [![DOI:10.1101/2021.01.08.425840](http://img.shields.io/badge/DOI-10.1101/2021.01.08.425840-B31B1B.svg)](https://doi.org/10.1101/2021.01.08.425840) -->
