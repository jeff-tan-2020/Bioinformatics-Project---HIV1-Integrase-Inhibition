# Bioinformatics-Project---HIV1-Integrase-Inhibition

This project was started based on the tutorial by Chanin Nantasenamat from his video <a href="https://www.youtube.com/watch?v=jBlTQjcKuaY">Python for Bioinformatics - Drug Discovery Using Machine Learning and Data Analysis</a>.

This project focuses on the inhibition of HIV Integrase I, an enzyme in the HIV virus required for the integration of viral DNA into the host genome <a href="https://pubmed.ncbi.nlm.nih.gov/15134551/">[1]</a>. 

## Part 1: Data Collection
The data used for the project was obtained from the ChEMBL database 

## Part 2: Exploratory Data Analysis
Each drug was labelled as either active or inactive based on the IC50 standard values 
- Drugs with less than 1000 nM IC50 labelled as active
- Drugs with greater than 10000 nM IC50 labelled inactive

Chemical properties between the two classes were compared

1. [plot_bioactivity_class.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988939/plot_bioactivity_class.pdf)
2. [plot_ic50.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988941/plot_ic50.pdf)
3. [plot_LogP.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988942/plot_LogP.pdf)
4. [plot_MW.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988943/plot_MW.pdf)
5. [plot_MW_vs_LogP.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988944/plot_MW_vs_LogP.pdf)
6. [plot_NumHAcceptors.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988945/plot_NumHAcceptors.pdf)
7. [plot_NumHDonors.pdf](https://github.com/jeff-tan-2020/Bioinformatics-Project---HIV1-Integrase-Inhibition/files/6988946/plot_NumHDonors.pdf)

## Parts 3-6: Descriptor Calculation and Model Building

PaDEL-descriptor software<a href="https://pubmed.ncbi.nlm.nih.gov/21425294/">[2]</a>. was used to calculate molecular fingerprints to input into a Random Forest regressor model. This model was compared with other ML models. 

![regressor_comparison](https://user-images.githubusercontent.com/75536936/129493971-6dfc209b-f964-4149-a7e9-74a66216d9b5.jpg)


