# Feature Selection with Principal Component Analysis (PCA)

An R script demonstrating how to do feature selection with PCA.

## Input:

- A CSV file with one feature per column and vectors on the rows (dataset<-"SampleDataSet.csv")
- The option to scale the data (scale_data<-T): the default is True 
- The option to center the data around 0 (center_data<-F): the default is False. This parameter is overwritten by scale_data (if scale_data is true)
- A threshold to select the Principal Components (PCs) explaining the
   covariance in the data: The default is 95% of the covariance
   (eigenvector_threshold<-0.95)
 - A threshold to select the features explaining the PCs: The default is 80% of the PCs
   (variables_threshold<-0.8)

*Other input parameters:*
 - An option to generate simulated data and demonstrate how the script works (demo<-F)
 - An option to generate a plot of the first two variables and the PC lines (plot<-F)

## Output:

A reduced-feature dataset in CSV format, with the columns ordered by their contributions to the PCs (output_dataset<-"SampleDataSet_reduced.csv").

## Examples:

The SampleDataSet.csv contains one example of environmental features (one for each column) associated to 1392 oceanic cells.
