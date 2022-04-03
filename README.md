# BME580_Project
Code used for BME 580 Project (Spring 2022)
The attached code is an all incompassing code that performs all the tasks of our model building. There are two main packages that are needed for this
code to run correctly. First the user needs the GEOquery package which allows the code easy access to the raw gene expression data from the Gene Expression
Omnibus website which is an NIH sponsered omnibus. The user also need the limma package from Bioconductor. The limma package, or linear models for micro 
array data is designed to test for differential expression of genes measured via a micro array. This package is vital for finding key genes that are 
differently expressed in the study populations with and without osteoperosis. Tidyverse is also needed for some computations later on in the code.
With these packages installed the code will run on it own and perform leave one out cross validation on the gene expression data to test to see what the 
potential accuracy of a linear discriminant analysis model would be. The end result is an estimated accuracy of such a model tested 10 times in the LOOCV.

The raw gene expression data obtained from GEO is also attached as OP_data and was used in the code to extract said raw data in an easier way than through 
the GEOquery package
