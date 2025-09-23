# EFDL2Limadou
EFD-01 L2 -> L2Limadou data processor (Limadou Scienza+ project) 

This repository contains the python script `efd01_reprocesstoL2Limadou.py`, implementing the correction procedures for removing the data jumps that are present in Level 2 (L2) public data of EFD-01 from the CSES-01 mission, namely in the electric field timeseries (also known as waveforms) collected in the ULF and ELF.

Details of the correction procedure are explained in [1](#references).

### Dependencies ###
The package has been written and tested in python3.8, should be compatible with python <3.13, due to requirement from numba.

Dependencies: numpy, scipy, h5py, pandas, termcolor, 
Optional: apexpy (if one wants to use --add_mag_coords option)


### Install ###

Simply download the files and install the dependencies.

### Examples ###


### Contacts ###

This software has been written and is maintained by Emanuele Papini - INAF (emanuele.papini@inaf.it).

Please feel free to contact us would you need any help and to report bug issues.

### Acknowledgements ###

We acknowledge financial support from the Italian Space Agency under the contract ASI “LIMADOU Scienza+” n° 2020-31-HH.0

Would you use the EFDL2Limadou data processor for a scientific publication, please add a link to this repository and properly reference our publication and the following zenodo link.


## References

1) [E. Papini et al.](https://mdpi.com) Remote Sensing, XXX, pages XXX, 2025. doi: XXXXXX
