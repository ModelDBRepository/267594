
This is the NEURON model code used in "Contrast-polarity specific mapping improves efficiency of neuronal computation for collision detection", available at https://doi.org/10.7554/eLife.79772. This model adapts previous LGMD models to investigate the influence of newly discovered ON excitation impinging on dendritic field C.

The modeling is described in Figure 7 and accompanying text in the article. There are in cluded scripts that reproduce the simulations of each figure panel named "Fig7B.hoc", "Fig7C.hoc", "Fig7D.hoc", and "Fig7E.hoc". There is also a simple gui window for loading each script created by "mosinit.hoc".

All model code was written in hoc and simulations were conducted in NEURON version 7.7, but we believe that nothing in the code is version specific.


Auto-launch or Compile special:
The LGMD model uses several custom .mod files for channels and currents. If the auto-launch link does not compile a special executable version of NEURON with the additional membrane mechanisms, use the mknrndll application or nrnivmodl binary as described below.

cd LGMD_2022       # change path to location on your computer with downloaded files
nrnivmodl ./mods   # compile special executable 
x86_64/special ./mosinit.hoc -    # execute Neuron and initialize

