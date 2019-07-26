# bedpe2tabix
### A simple R script for converting bedpe format to tabix, for visualization in WashU Epigenome Browser
You will need to have tabix installed on your system.

This script converts bedpe formatted files into tabix which can be used on WashU Epigenome Browser. You need to input a bedpe file which also includes a column for interaction score. Currently score is considered to be a value in range of (0,1] with lower value representing higher score; similar to FDR. In the generated tabix file the score is converted using -log2(score).

You will need to provide the name of the bedpe file that should be converted to tabix, the desired name of the output tabix file, and also the name of the column that holds the interaction scores in the bedpe file. 

## To run:
```
Rscript bedpe2tabix.R -i bedpe_filename -t tabix_filename -s score_column_name
```
or
```
R CMD BATCH bedpe2tabix.R '--args -i bedpe_filename -t tabix_filename -s score_column_name'
```
or to print help, use:
```
Rscript bedpe2tabix.R -h
```
