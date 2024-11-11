---------------------------------------------------------------------------
NON CODE SPECS
---------------------------------------------------------------------------
`ProjectReport.pdf` is the report for ML4CPS Project 2 (Odd Sem 2024).

'feature_category_dict.json` contains the category mapping for each feature, for eg: {"Socio-demographic": ["Number of Households", "Average persons per household", ...], ...}

`public_hospital_locs.csv` contains the locations of hospitals obtained from Google Maps. 

---------------------------------------------------------------------------
CODE SPECS
---------------------------------------------------------------------------

Code Description:
----------------------
The entirety of the code is in the folder `code`, which contains all of the code and a folder named `data` containing all the project data in its original form (all the original excel workbooks). The `data` folder is left empty at the time of submission due to being identical to original dataset. Copy over all the excel sheets into this folder to run the `1_preprocess.ipynb` notebook.

The data within `data` is fed to the `1_preprocess.ipynb` notebook to format and prepare the suburb data for downstream tasks. Output is saved to `combined_data.csv`.

`2_locations.ipynb` is for approximating the relative location of the suburbs w.r.t. Melbourne GPO. It saves the location-appended dataset to `combined_data_with_loc.csv`. 

`PartA_full.ipynb` contains all the relevant analysis for the Part A of the project.

`access_to_healthcare.ipynb` contains the hospital related analysis conducted in Part B.

`socio_demographic.ipynb` comprises of the socio-demographic analysis carried out in Part B of the project.

-----------------------------
Versions and Dependencies:
-----------------------------

Python Version: 3.12.3

Major Dependencies:

numpy
pandas
matplotlib
seaborn
scikit-learn
scipy
geopandas
pysal
esda
