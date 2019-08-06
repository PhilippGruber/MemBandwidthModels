# PalladioMemoryBandwidthModels
The corresponding Palladio models to my bachelor thesis. 

# Index

24 refers to the 12 core machine
80 refers to the 40 core machine
As a bonus, the memtest model to simulate the Memtest in Palladio

Structure of the model name:

Matrix **z** Threads **y** CMNw **x**

z = [24,80] machine

y = [2..16] cores

x = [ε,L1,L2,All]

x specifies the grade of memory behavior modeling
* ε includes just L3 cache the main memory
* L1 includes the L1, L3 cache and main memory
* L2 includes The L2, L3 cache and the main memory
* All as it says includes the whole memory hierarchy
 
 Preferably stick to All, and if not needed specify in the SEFF the bytesize in the variable action of the corresponding memory hierarchy level to zero.
 
 If problems occur importing the models, it is maybe because of a newer (or older) Palladio version, we refer to https://sdqweb.ipd.kit.edu/wiki/PCM_4.1
 See section migrating, probably by the time a newer version will exist. 
