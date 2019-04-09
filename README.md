# bedpe2tabix
### A simple R script for converting bedpe format to tabix, for visualization in WashU Epigenome Browser
You will need to have tabix installed on your system.

This script currently works for converting [MAPS](https://github.com/ijuric/MAPS/) output, since it requires a 'fdr' column. Or you can add a column 'fdr' to any bedpe file. I will update it later.

## To run:
```
bedpe2tabix.sh bedpe_filename tabix_filename
```