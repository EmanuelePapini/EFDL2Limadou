# EFDL2Limadou
EFD-01 L2 -> L2Limadou data processor (Limadou Scienza+ project) 

This repository contains the python script `efd01_reprocesstoL2Limadou.py`, implementing the correction procedures for removing the data jumps that are present in Level 2 (L2) public data of EFD-01 from the CSES-01 mission, namely in the electric field timeseries (also known as waveforms) collected in the ULF and ELF.

Details of the correction procedure are explained in [1](#csespy).

### Dependencies ###
The package has been written and tested in python3.12.

Dependencies: numpy, scipy, h5py, pandas, termcolor, 
Optional: apexpy (if one wants to use --add_mag_coords option)


### Install ###

Simply download the files and install the dependencies.


### Usage ###

To process a Level 2 EFD-01 HDF5 file and generate a correcte HDF5 file, run:

```bash
python efd01_reprocesstoL2Limadou.py --input /input_folder/CSES_01_EFD_2_L02_A1_031190_20180826_095004_20180826_102510_000.h5 
```

The above command will save the corrected file in `./CSES_01_EFD_2_L02_A1_031190_20180826_095004_20180826_102510_000_Limadou.h5`.

You can see all available options by running:

```bash
python efd01_reprocesstoL2Limadou.py --help
```


### Contacts ###

This software has been written and is maintained by Emanuele Papini - INAF (emanuele.papini@inaf.it).

Please feel free to contact us would you need any help and to report bug issues.

### Acknowledgements ###

We acknowledge financial support from the Italian Space Agency under the contract ASI “LIMADOU Scienza+” n° 2020-31-HH.0.

Would you use the EFDL2Limadou data processor for a scientific publication, please add a link to this repository and properly reference our [publication](#csespy) and the following zenodo link listed below.


## References

<a name="csespy">1) [E. Papini et al.](https://mdpi.com) Remote Sensing, XXX, pages XXX, 2025. doi: XXXXXX </a>
