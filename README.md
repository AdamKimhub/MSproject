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



