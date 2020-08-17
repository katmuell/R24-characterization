# R24-characterization
Analysis of biofilm and clumping data for replication of measurements related to our wild Akkermansia isolates.

# Biofilm Analysis
For biofilm assays, this code takes raw OD measurements from a plate reader and calculates the average OD for each isolate in each plate.
The mean is then used to calculate the fold change from BAA-835 and the fold change from the mean OD of the respective plate.
The output is a .csv file containing as a dataframe:
  Isolate
  Assay Plate
  Mean OD
  Fold change relative to BAA-835
  Fold change relative to assay mean

# Clumping Analysis
For clumping assays, this code takes raw OD measurements of the top and bottom portions of culture and filters out those wells with a bottom OD of < 0.1, signalling a lack of growth.
The bottom/top (BT) ratio for each culture is calculated and used to determine the average BT ratio for each isolate in each plate.
The mean is then used to calculate the fold change from BAA-835 and the fold change from the mean BT ratio of the repective plate.
The output is a .csv file containing as a dataframe:
  Isolate
  Assay Plate
  Mean BT ratio
  Fold change relative to BAA-835
  Fold change relative to assay mean
