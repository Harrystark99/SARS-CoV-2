# Preparation for docking

This section describes the process of charge enumeration (i.e. generation of all charge forms) from the initial set of ~42,000 candidate compounds, and 3D conformer generation, prior to performing docking.


## Live Resources

| usegalaxy.eu | 
|:--------:|
| [![Galaxy history](https://img.shields.io/static/v1?label=history&message=view&color=blue)](https://usegalaxy.eu/u/sbray/h/charge-enumeration) | 
| [![Galaxy workflow](https://img.shields.io/static/v1?label=workflow&message=run&color=blue)](https://usegalaxy.eu/u/sbray/w/charge-enumeration) | 


## Outline

- The initial candidate compounds in SMILES format are enumerated using Dimorphite-DL [1] and [RDKit](http://www.rdkit.org) to a total of around ~150,000 compounds.  
- For each of these, a three-dimensional structure is generated using OpenBabel [2] and saved in SD-format.
- The SD-file is split into chunks of 1,000 molecules each ready for docking.

## History and workflow

A Galaxy workspace (history) containing the most current analysis can be imported from [here](https://usegalaxy.eu/u/sbray/h/charge-enumeration).

The publicly accessible [workflow](https://usegalaxy.eu/u/sbray/w/charge-enumeration) can be downloaded and installed on any Galaxy instance. It contains version information for all tools used in this analysis.

 <p align="center">
  Preparation for docking
  <a href="https://usegalaxy.eu/u/sbray/w/charge-enumeration">   <img src="./w-ligand-enumeration.png" alt="Workflow preparation for docking" /></a> &nbsp;  
 </p>
 

## References

[1] Dimorphite-DL: an open-source program for enumerating the ionization states of drug-like small molecules,
Robb *et al.* [doi:10.1186/s13321-019-0336-9](https://doi.org/doi:10.1186/s13321-019-0336-9).

[2] Open Babel: An open chemical toolbox. O'Boyle *et. al* [doi:10.1186/1758-2946-3-33](https://doi.org/10.1186/1758-2946-3-33).
