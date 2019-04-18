## Molecular Property 
- Molecular_Weight_Materials


## Molecular Property Counts
- Num_RotatableBonds_Materials
- Num_chiral_Centers_Materials

##  the number of hydrogen acceptors and/or donors
### key word: 得失氫 (氧化還原能力)
```
Calculates and outputs the counts of hydrogen bond donors and acceptors in the input molecules. 
```
- Num_H_Acceptors_Materials: number of heteroatoms (Oxygen, Nitrogen, Sulfur, or Phosphorus) with one or more lone pairs, excluding atoms with positive formal charges, amide and pyrrole-type Nitrogens, and aromatic Oxygen and Sulfur atoms in heterocyclic rings.
- Num_H_Donors_Materials: number of heteroatoms (Oxygen, Nitrogen, Sulfur, or Phosphorus) with one or more attached Hydrogen atoms.




## Balaban, Wiener, and Zagreb Index descriptors
key word: 圖論 大小 分支程度 彈性 形狀
```
The Balaban, Wiener and Zagreb indices are two-dimensional topological descriptors based on graph-theory concepts. They help to differentiate molecules according mostly to their size, degree of branching, flexibility, and overall shape.
See also:
Balaban, A. T., "Highly Discriminating Distance-Based Topological Index", Chem. Phys. Lett., 89, 399-404 (1982)
Wiener, H., "Structural Determination of Paraffin Boiling Points", J. Chem. Phys., 69, 17-20 (1947)
Muller, W. R., et al., "An Algorithm for Construction of the Molecular Distance Matrix", J. Comput. Chem., 8, 170-173 (1987)
Bonchev, D., "Information Theoretic Indices for Characterization of Chemical Structures", Chemometrics Series, ed. D.D. Bawden, Vol 5, New York: Research Studies Press Ltd. (1983)
```

- JX_Materials: Balaban JX descriptor
- JY_Materials: Balaban JY descriptor
- Wiener_Materials: Wiener Index
- Zagreb_Materials: Zagreb Index

##  the Chi Index descriptors
### key word: 圖論 大小 分支程度 彈性 形狀
```
The Chi Index descriptors are two-dimensional topological descriptors based on graph-theory concepts. They help to differentiate molecules according mostly to their size, degree of branching, flexibility, and overall shape.
See Also:
Kier, L.B., "A Shape Index from Molecular Graphs", Quant. Struct-Act. Relat., 4, 109-116 (1985)
Kier, L.B., "Indexes of molecular shape from chemical graphs" in Computational Chemical Graph Theory; Rouvray, D.H., Ed.; Nova Science: New York (1990).
Hall, L.H. and Kier, L.B., "The Molecular Connectivity Chi Indexes and Kappa Shape Indexes in Structure-Property Modeling", in Reviews in Computational Chemistry II., K.B. Lipkowitz and D.B. Boyd, editors, p. 367-422 (1991)(1987)
```
- CHI_0_Materials
- CHI_1_Materials
- CHI_2_Materials
- CHI_3_P_Materials
- CHI_3_C_Materials
- CHI_3_CH_Materials
- CHI_V_0_Materials
- CHI_V_1_Materials
- CHI_V_2_Materials
- CHI_V_3_P_Materials
- CHI_V_3_C_Materials
- CHI_V_3_CH_Materials

##  the Electrotopological State keys for the material
### key word: 電子相關拓樸
```
Calculates the sums of the Electrotopological State (E-state) values and/or the counts and/or the indicators of each atom type. The output can be as a number of individual properties, one for each atom type, or as a single property with an array of values. The type of output is controlled by What to Output:
See Also:
The Electrotopological State (E-State) descriptors calculated are defined by Kier and Hall:
Hall L., Mohney B., Kier L., J. Chem. Inf. Comput. Sci., 1991, 31, 76-82.
Hall L., Kier L., J. Chem. Inf. Comput. Sci., 2000, 40, 784-791).
```
- Estate_Keys_Properties: Calculate the E-state sums for all atom types and output them as individual properties.
- Estate_Counts_Properties: Calculate the E-state counts for all atom types and output them as individual properties.
- Estate_Indicators_Properties: Calculate the E-state indicators for all atom types and output them as individual properties.
- Estate_Keys: Calculate the E-state sums for all atom types and output them in one property as an array of double values.
- Estate_Counts: Calculate the E-state counts for all atom types and output them in one property as an array of integer values.
- Estate_Indicators: Calculate the E-state indicators for all atom types and output them in one property as an array of integer values.
- E-state keys are calculated for organic elements (C, N, O, P, S), halogens (F, Cl, Br, and I) and for Li, Be, B, Si, Ge, As, Se, Sn, and Pb.

## Graph-Theoretical InfoContent descriptors
### key word: 圖論  大小 分支程度 彈性 形狀 有先被分類!
```

The InfoContent descriptors are two-dimensional topological descriptors. Topological descriptors are based on graph-theory concepts. They help to differentiate molecules according to their size, degree of branching, flexibility, and overall shape.
In this particular approach, molecules are viewed as structures that can be partitioned into subsets of elements that are in some sense equivalent. The notion of equivalence depends on the particular descriptor.
See Also:
Bonchev, D., "Information Theoretic Indices for Characterization of Chemical Structures", Chemometrics Series, ed. D.D. Bawden, Vol 5, New York: Research Studies Press Ltd. (1983)
```

- IC_Materials: Information Content
- BIC_Materials: Bonding Information Content
- CIC_Materials: Complementary Information Content
- SIC_Materials: Structural Information Content
- IAC_Total_Materials: Total Information of Atomic Composition
- IAC_Mean_Materials: Mean Information of Atomic Composition
- V_ADJ_mag_Materials: Vertex Adjacency Magnitude
- V_DIST_mag_Materials: Vertex Distance Magnitude
- V_ADJ_equ_Materials: Vertex Adjacency Equality
- V_DIST_equ_Materials: Vertex Distance Equality
- E_ADJ_mag_Materials: Edge Adjacency Magnitude
- E_DIST_mag_Materials: Edge Distance Magnitude
- E_ADJ_equ_Materials: Edge Adjacency Equality
- E_DIST_equ_Materials: Edge Distance Equality


##  the Jurs Descriptors for the material
### key word: 結合 形狀和電子   部分電荷(atomic partial charges) 表面積
```
This set of descriptors combines shape and electronic information to characterize molecules. The set is based on work by Stanton and Jurs (1990). The descriptors are calculated by mapping atomic partial charges onto solvent-accessible surface areas of individual atoms.
Tip: Jurs descriptors should only be calculated for structures with charges assigned, any values for structures without assigned charges cannot be treated as reliable.
See Also:
The descriptors calculated are defined by Stanton and Jurs:
Stanton D., Jurs P., "Development and use of charged partial surface area structural descriptors in computer assisted quantitative structure property relationship studies", Anal. Chem., 1990, 62, 2323-2329.
```

Solvent accessible area
- Jurs_SASA_Materials: The total molecular solvent-accessible surface area.
Partial charged areas
- Jurs_PPSA_1_Materials: Partial positive surface area: the sum of the solvent-accessible surface areas of all positively charged atoms.
- Jurs_PNSA_1_Materials: Partial negative surface area: the sum of the solvent-accessible surface areas of all negatively charged atoms.
- Jurs_DPSA_1_Materials: Difference in charged partial surface areas: the partial positive surface area minus partial negative surface area (Jurs_PPSA_1_Materials - Jurs_PNSA_1_Materials).
- Total charge-weighted areas
- Jurs_PPSA_2_Materials: Total charge-weighted positive surface area: the partial positive surface area multiplied by the total positive charge.
- Jurs_PNSA_2_Materials: Total charge-weighted negative surface area: the partial negative surface area multiplied by the total negative charge.
- Jurs_DPSA_2_Materials: Difference in total charge-weighted surface areas: the total charge-weighted positive surface area minus total charge weighted negative surface area (Jurs_PPSA_2_Materials - Jurs_PNSA_2_Materials).
- Atomic charge-weighted areas
- Jurs_PPSA_3_Materials: Atomic charge-weighted positive surface area: the sum of the product of the solvent-accessible surface area and partial charge for all positively charged atoms.
- Jurs_PNSA_3_Materials: Atomic charge-weighted negative surface area: the sum of the product of the solvent-accessible surface area and partial charge for all negatively charged atoms.
- Jurs_DPSA_3_Materials: Difference in atomic charge-weighted surface areas: the atomic charge-weighted positive surface area minus the atomic charge-weighted negative surface area (Jurs_PPSA_3_Materials - Jurs_PNSA_3_Materials).
Fractional charged partial areas
- Jurs_FPSA_1_Materials: Fractional partial positive surface area: the partial positive surface area divided by the total molecular solvent-accessible surface area (Jurs_PPSA_1_Materials / Jurs_SASA_Materials).
- Jurs_FPSA_2_Materials: Fractional charge-weighted positive surface area: the total charge-weighted positive surface area divided by the total molecular solvent-accessible area (Jurs_PPSA_2_Materials / Jurs_SASA_Materials).
- Jurs_FPSA_3_Materials: Fractional atomic charge-weighted positive surface area: the atomic charge-weighted positive surface area divided by the total molecular solvent-accessible area (Jurs_PPSA_3_Materials / Jurs_SASA_Materials).
- Jurs_FNSA_1_Materials: Fractional partial negative surface area: the partial negative surface area divided by the total molecular solvent-accessible surface area (Jurs_PNSA_1_Materials / Jurs_SASA_Materials).
- Jurs_FNSA_2_Materials: Fractional charge-weighted negative surface area: the total charge-weighted negative surface area divided by the total molecular solvent-accessible area (Jurs_PNSA_2_Materials / Jurs_SASA_Materials).
- Jurs_FNSA_3_Materials: Fractional atomic charge-weighted negative surface area: the atomic charge-weighted negative surface area divided by the total molecular solvent-accessible area (Jurs_PNSA_3_Materials / Jurs_SASA_Materials).
Surface-weighted partial areas
- Jurs_WPSA_1_Materials: Surface-weighted partial positive surface area: the product of the partial positive surface area and the total molecular solvent-accessible surface area divided by 1000 (Jurs_PPSA_1_Materials × Jurs_SASA_Materials / 1000).
- Jurs_WPSA_2_Materials: Surface-weighted charge-weighted positive surface area: the product of the total charge-weighted positive surface area and the total molecular solvent-accessible area divided by 1000 (Jurs_PPSA_2_Materials × Jurs_SASA_Materials / 1000).
- Jurs_WPSA_3_Materials: Surface-weighted atomic charge-weighted positive surface area: the product of the atomic charge-weighted positive surface area and the total molecular solvent-accessible area divided by 1000 (Jurs_PPSA_3_Materials × Jurs_SASA_Materials / 1000).
- Jurs_WNSA_1_Materials: Surface-weighted partial negative surface area: the product of the partial negative surface area and the total molecular solvent-accessible surface area divided by 1000 (Jurs_PNSA_1_Materials × Jurs_SASA_Materials / 1000).
- Jurs_WNSA_2_Materials: Surface-weighted charge-weighted negative surface area: the product of the total charge-weighted negative surface area and the total molecular solvent-accessible area divided by 1000 (Jurs_PNSA_2_Materials × Jurs_SASA_Materials / 1000).
- Jurs_WNSA_3_Materials: Surface-weighted atomic charge-weighted negative surface area: the product of the atomic charge-weighted negative surface area and the total molecular solvent-accessible area divided by 1000 (Jurs_PNSA_3_Materials × Jurs_SASA_Materials / 1000).
Relative charges
- Jurs_RPCG_Materials: Relative positive charge: the charge of the most positive atom divided by the total positive charge.
- Jurs_RNCG_Materials: Relative negative charge: the charge of the most negative atom divided by the total negative charge.
- Jurs_RPCS_Materials: Relative positive charge surface area: the solvent-accessible surface area of the most positive atom divided by the relative positive charge.
- Jurs_RNCS_Materials: Relative negative charge surface area: the solvent-accessible surface area of the most negative atom divided by the relative negative charge.
Polar and apolar areas
- Jurs_TPSA_Materials: Total polar surface area: the sum of solvent-accessible surface areas of all polar atoms (either those for which the absolute value of the partial charge is greater than or equal to the Charge Threshold, or those in the Polar Atoms list, depending on the value of Use Polar Atoms.
- Jurs_TASA_Materials: Total apolar surface area: the sum of solvent-accessible surface areas of all apolar atoms (either those for which the absolute value of the partial charge is less than the Charge Threshold or those not in the Polar Atoms list, depending on the value of Use Polar Atoms).
- Jurs_RPSA_Materials: Relative polar surface area: the total polar surface area divided by the total solvent-accessible surface area (Jurs_TPSA_Materials / Jurs_SASA_Materials).
- Jurs_RASA_Materials: Relative apolar surface area: the total apolar surface area divided by the total solvent-accessible surface area (Jurs_TASA_Materials / Jurs_SASA_Materials).



## Kappa Shape Index descriptors and Molecular Flexibility
### key word: 圖論  大小 分支程度 彈性 形狀 
AM的是進階版 使用共價半徑 和 hybridization states來修正形狀
```
The Kier and Hall Shape indices are two-dimensional topological descriptors. Topological descriptors are based on graph-theory concepts. They help to differentiate molecules according mostly to their size, degree of branching, flexibility, and overall shape.
The Kappa Shape Indices compare the molecule graph with "minimal" and "maximal" graphs, where the meaning of "minimal" and "maximal" depends on the order n. This is intended to capture different aspects of the molecular shape.
The Alpha-Modified Kappa Shape Indices are refinements of the above shape indices that take into consideration the contribution covalent radii and hybridization states make to the shape of the molecule.
The Molecular Flexibility is a descriptor based on structural properties that restrict a molecule from being "infinitely flexible", the model for which is an endless chain of C(sp3) atoms. The structural features considered as preventing a molecule from attaining infinite flexibility are: (a) fewer atoms, (b) the presence of rings, (c) branching, and (d) the presence of atoms with covalent radii smaller than those of C(sp3).
See Also:
Kier, L.B., "A Shape Index from Molecular Graphs", Quant. Struct-Act. Relat., 4, 109-116 (1985)
Kier, L.B., "Indexes of molecular shape from chemical graphs" in Computational Chemical Graph Theory; Rouvray, D.H., Ed.; Nova Science: New York (1990).
Hall, L.H. and Kier, L.B., "The Molecular Connectivity Chi Indexes and Kappa Shape Indexes in Structure-Property Modeling", in Reviews in Computational Chemistry II., K.B. Lipkowitz and D.B. Boyd, editors, p. 367-422 (1991)(1987)

```

- Kappa_1_Materials:Shape index of order one
- Kappa_2_Materials:Shape index of order two
- Kappa_3_Materials:Shape index of order three
- Kappa_1_AM_Materials:Alpha-modified shape index of order one
- Kappa_2_AM_Materials:Alpha-modified shape index of order two
- Kappa_3_AM_Materials:Alpha-modified shape index of order three
- PHI_Materials: Molecular Flexibility


##  Subgraph Count descriptors
### key word: 圖論  大小 分支程度 彈性 形狀 
```
The Subgraph Count descriptors are two-dimensional topological descriptors based on graph-theory concepts. They help to differentiate molecules according mostly to their size, degree of branching, flexibility, and overall shape.
See Also:
Kier, L.B., "A Shape Index from Molecular Graphs", Quant. Struct-Act. Relat., 4, 109-116 (1985)
Kier, L.B., "Indexes of molecular shape from chemical graphs" in Computational Chemical Graph Theory; Rouvray, D.H., Ed.; Nova Science: New York (1990).
Hall, L.H. and Kier, L.B., "The Molecular Connectivity Chi Indexes and Kappa Shape Indexes in Structure-Property Modeling", in Reviews in Computational Chemistry II., K.B. Lipkowitz and D.B. Boyd, editors, p. 367-422 (1991)(1987)
```
- SC_0_Materials
- SC_1_Materials
- SC_2_Materials
- SC_3_P_Materials
- SC_3_C_Materials
- SC_3_CH_Materials


##  LogP and Molar Refractivity by the Ghose and Crippen method
### key word: octanol-water partition coefficient (LogP) and the molar refractivity (MR) 
 logP 看疏水性  MR看 分子體積和極性(polarizability)
```
Calculates the octanol-water partition coefficient (LogP) and the molar refractivity (MR) for the incoming molecules using the atom-based method published by Ghose and Crippen. LogP provides a measure of the hydrophobicity of the molecule, while MR contains information about molecular volume and polarizability.
Notes:
For more information on the ALogP method see Ghose, A.K., Viswanadhan V.N., and Wendoloski, J.J., Prediction of Hydrophobic (Lipophilic) Properties of Small Organic Molecules Using Fragment Methods: An Analysis of AlogP and CLogP Methods. J. Phys. Chem. A, 1998, 102, 3762-3772.
```
- ALogP_Materials: The Ghose and Crippen octanol-water partition coefficient.
- ALogP_MR_Materials: The Ghose and Crippen estimate of molar refractivity.
- ALogP98_Materials: Atom-type-based ALogP value, calculated using the published set of parameters from Ghose et al., 1998.

