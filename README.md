Repository for software described in

# On the evolvability hypothesis of aging: Directional selection coupled with kin selection favors the establishment of senescence

András Szilágyi<sup>1</sup>; Tamás Czárán<sup>1</sup>; Mauro Santon<sup>2</sup>; Eörs Szathmáry<sup>1,4,5,6</sup>

###<sup>1</sup>Institute of Evolution, Centre for Ecological Research, Budapest, Hungary,
<sup>2</sup>Departament de Genètica i de Microbiologia, Grup de Genòmica, Bioinformàtica i Biologia Evolutiva (GBBE), Universitat Autònoma de Barcelona, Spain,
<sup>3</sup>cE3c – Centre for Ecology, Evolution and Environmental Changes & CHANGE – Global Change and Sustainability Institute, Lisboa, Portugal,
<sup>4</sup>Center for the Conceptual Foundations of Science, Parmenides Foundation, Pöcking, Germany,
<sup>5</sup>Department of Plant Systematics, Ecology and Theoretical Biology, Eötvös Loránd University, Budapest, Hungary,
<sup>6</sup>Konrad Lorenz Institute for Evolution and Cognition Research, Klosterneuburg, Austria

AgeingEvol.tar.gz contains the full source code

To build the program under linux or any compatible system using the GCC toolchain, issue the command `make` in the source directory.

The output contains: frequency of living individulas, average age of the population, average rate of aging of the population, minumum rate of aging in the population, maximum rate of aging in the population, average Hamming distance of the population from the actual target, number of 1s in the target.

The parameters of the model are the following (standard values are in brackets):
* `N`: size of the  grid (200)  
* `L`: total number of loci (100)  
* `LF`: number of fecundity loci (50)  
* `LA=L-LF`: number of senescence loci (50)  
* `AgeVal`: proportionality value of senescence (0.01)  
* `pflipfec`: per bit flip probability of fecundity allels (0.01)  
* `pflipage`: per bit flip probability of senescence allels (0.01)  
* `sel_reg`: selection regime, 0: directional, 1: stabilizing  
* `death_prob_baseline`: baseline death rate (0.05)  
* `Tfitness`: fitnes period dilution (10)  
* `prec`: probability of single point recombination (1/0)  
* `fitbase`: base of fitness (1.2)  
* `ner`: Moore neighbourhood radius (1)  
* `time_steps`: total time steps of the simulation (10000)  
* `print_mod`: writing out the statistics in every Nth steps (5)  
* `print_grid`: making snapshots of the grid in every print_mod time steps (0: no, 1: yes)  
* `aging_max`: maximum value of rate of aging for vizualization (0.3)  
