This repository is set up to build a machine learning model similar to CGCNN to deal with 2D crystalline materials with point defects.

The model is to identify patterns that exist between the properties of a defective 2D material and its influence on the band gap of the material.

These properties are:
1. The host material of the crystalline materal.
2. The type of defect sites in the crystalline material.
2. The number of defect sites in the crystalline material.
3. The configuration/ arrangement of defect sites in the crystalline material.

## Details of what each file does
### `combine.py`
This python file combines the `descriptor.csv` file with the `defects.csv` file while also doing some calculatons to extract vital features of each defective structure. 

These features are:
1. `_id`: Ccif id of a crystalline strcture.
2. `energy`: Total potential energy of the crystal structure as reported by VASP(given in eV).
3. `fermi_level`: Fermi level of the crystalline structure given in eV
4. `total_mag`: Total magnetisation of the crystalline material
5. `base`: Host material of the crystalline material
6. `cell`: Supercell size
7. `vacancy_sites` and `substituiton_sites`: defect type identification
8. `dataset_material`: Type of dataset material(high density dataset+host material or low density + host material)[Essential for splitting the data]
9. `formation_energy`: defect formation energy
10. `formation_energy_per_site`: defect formation energy divided by the number of defect sites
11. `energy_per_atom`: Total potential of the system divide by the number of atoms(given in eV)
12. `E_1`: Energy of the first Kohn-sham orbital of the structure with defects
13. `norm_homo`: Normalized value of highest occcupied molecular orbital
14. `norm_lumo`: Normalized value of lowest unoccupoed molecular orbital.
