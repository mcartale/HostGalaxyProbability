# HostGalaxyProbability

In this repository you will find the results from the work entitled "An astrophysically motivated ranking criterion for
low-latency electromagnetic follow-up of gravitational wave events", from Artale M. C., Bouffanais Y., Mapelli M., Giacobbo N., Sabha N. B., Santoliquido F., Pasquato M. & Spera M.

You will find the host galaxy probabilities at redshifts *z = 0.1, 1, 2,* and *6* as a function of the stellar mass, SFR, B- and Ks- bands.
For this we combine the catalogs from the population synthesis model MOBSE 
[(Giacobbo et al. 2018)](https://ui.adsabs.harvard.edu/abs/2018MNRAS.474.2959G/abstract)
together with galaxy catalogs from the hydrodynamical cosmological simulation EAGLE [(Schaye et al. 2015)](https://ui.adsabs.harvard.edu/abs/2015MNRAS.446..521S/abstract) to derive the properties of the host galaxies of binary neutron stars (BNS), black hole-neutron star (BHNS), and binary black hole (BBH) mergers.

We have used a grid of 25 x 25 x 25 points with a range of <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\log(M_\ast{}&space;/&space;M_{\odot})&space;\in{}[&space;7.0,\,{}12.5]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\log(M_\ast{}&space;/&space;M_{\odot})&space;\in{}[&space;7.0,\,{}12.5]" title="\log(M_\ast{} / M_{\odot}) \in{}[ 7.0,\,{}12.5]" /></a>,
<a href="https://www.codecogs.com/eqnedit.php?latex=\log({\rm&space;SFR}&space;/&space;M_{\odot}&space;yr^{-1})&space;\in{}[&space;-5.5,\,{}&space;2.5]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\log({\rm&space;SFR}&space;/&space;M_{\odot}&space;yr^{-1})&space;\in{}[&space;-5.5,\,{}&space;2.5]" title="\log({\rm SFR} / M_{\odot} yr^{-1}) \in{}[ -5.5,\,{} 2.5]" /></a>, and <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\log&space;Z&space;\in{}&space;[-8,-0.7]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\log&space;Z&space;\in{}&space;[-8,-0.7]" title="\log Z \in{} [-8,-0.7]" /></a>
to compute the elements of the host galaxy probabilities.

The host galaxy probabilities can be used directly in ranking procedures for the electromagnetic follow-up searches.
Here we illustrate an example for a GW detection where NG galaxy candidates were identified and we have access to the stellar mass and SFR (this is valid also if only one galaxy property is available, such as the stellar mass, B- or <a href="https://www.codecogs.com/eqnedit.php?latex=K_s" target="_blank"><img src="https://latex.codecogs.com/gif.latex?K_s" title="K_s" /></a>- band are accesible, using p(M*), p(<a href="https://www.codecogs.com/eqnedit.php?latex=M_B" target="_blank"><img src="https://latex.codecogs.com/gif.latex?M_B" title="M_B" /></a>) or p(<a href="https://www.codecogs.com/eqnedit.php?latex=M_{K_s}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?M_{K_s}" title="M_{K_s}" /></a>), respectively):

In the simplistic case where all possible galaxies have the same sky localisation probabilities, the relative probability that the *k*th galaxy of our sample is the host of the merger is given by 

<a href="https://www.codecogs.com/eqnedit.php?latex=\mathbb{P}(\text{galaxy&space;}k)&space;=&space;\frac{\text{p}(M_\ast{}^{k},\text{SFR}^{k}&space;)}{\sum_{i=1}^{N_{G}}&space;\text{p}(M_\ast{}^{i},\text{SFR}^{i}&space;)}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbb{P}(\text{galaxy&space;}k)&space;=&space;\frac{\text{p}(M_\ast{}^{k},\text{SFR}^{k}&space;)}{\sum_{i=1}^{N_{G}}&space;\text{p}(M_\ast{}^{i},\text{SFR}^{i}&space;)}" title="\mathbb{P}(\text{galaxy }k) = \frac{\text{p}(M_\ast{}^{k},\text{SFR}^{k} )}{\sum_{i=1}^{N_{G}} \text{p}(M_\ast{}^{i},\text{SFR}^{i} )}" /></a>

where (<a href="https://www.codecogs.com/eqnedit.php?latex=$M_\ast{}^{k}$,$\text{SFR}^{k}$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$M_\ast{}^{k}$,$\text{SFR}^{k}$" title="$M_\ast{}^{k}$,$\text{SFR}^{k}$" /></a>) are the stellar mass and SFR of the *k*th galaxy of our targeted search sample and <a href="https://www.codecogs.com/eqnedit.php?latex=\text{p}(M_\ast{}^{k},\text{SFR}^{k}&space;)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\text{p}(M_\ast{}^{k},\text{SFR}^{k}&space;)" title="\text{p}(M_\ast{}^{k},\text{SFR}^{k} )" /></a> is obtained from the tables.


Information about the tables
----------------------------

In the repository there are three folders, one for each type of merging merging compact object binary studied: BBH,
BHNS, and BNS.

* The host galaxy probability using the B-band (p(<a href="https://www.codecogs.com/eqnedit.php?latex=M_B" target="_blank"><img src="https://latex.codecogs.com/gif.latex?M_B" title="M_B" /></a>)): 1DHostGalaxyProbability_B_Band_AAAA_zBBB.dat
* The host galaxy probability using the Ks-band (p(<a href="https://www.codecogs.com/eqnedit.php?latex=M_{K_s}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?M_{K_s}" title="M_{K_s}" /></a>)): 1DHostGalaxyProbability_Ks_Band_AAAA_zBBB.dat
* The host galaxy probability using the stellar mass (<a href="https://www.codecogs.com/eqnedit.php?latex=$p(M_{\ast{}})$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$p(M_{\ast{}})$" title="$p(M_{\ast{}})$" /></a>): 1DHostGalaxyProbability_Ms_AAAA_zBBB.dat
* The host galaxy probability using the stellar mass and SFR ([img[https://latex.codecogs.com/gif.latex?$p(M_{\ast{}},{\rm SFR})$]]): 2DHostGalaxyProbability_Ms_SFR_AAAA_zBBB.dat
where AAAA = BBH, BHNS, or BNS; BBB= 0p1, 1, 2, or 6 (corresponding to the redshift)
