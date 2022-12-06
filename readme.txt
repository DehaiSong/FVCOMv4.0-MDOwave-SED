FVCOM-MDOwave coupled with FVCOM-Sediment 
Now the MDOwave can be coupled with the sediment module from FVCOM. 
Just uncomment FLAG_32 (and FLAG_33) with Flag_21 and one of the FLAG_211 Original sediment or CSTMS sediment to compile. 
Turn on the Sediment model in the casename_run.nml, like this: 
SEDIMENT_MODEL = T, 
SEDIMENT_MODEL_FILE = 'sed.inp', 
SEDIMENT_PARAMETER_TYPE = 'uniform', 
SEDIMENT_PARAMETER_FILE = none, 
BEDFLAG_TYPE = 'constant', 
BEDFLAG_FILE = 'none', 

A sed.inp file is given as an example.
Noted that the FVCOM-SWAVE has been completely removed from this version.