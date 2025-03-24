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
1. `_id`: This is the cif id of a crystalline strcture.
2. `energy`: This is the energy of the crystal structure.
3. `fermi_level`: 
4. `total_mag`:
5. `base`: One hot encoded.
6. `cell`
7. `vacancy_sites` and `substituiton_sites`
8. `dataset_material`: for stratification
9. `formation_energy`
10. `formation_energy_per_site`
11. `energy_per_atom`
12. `E_1`
13. `norm_homo`
14. `norm_lumo`
