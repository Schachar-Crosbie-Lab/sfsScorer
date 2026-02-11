# Run analysis on TOCS raw values to return t-scores

get_tocs_tscores() returns gendered and non-gendered t-scores for the
[Toronto Obsessive-Compulsive Scale (TOCS)
assessment](https://pubmed.ncbi.nlm.nih.gov/27015722/)

## Usage

``` r
get_tocs_tscores(file = NULL, output_folder = here::here())
```

## Arguments

- file:

  Pathway to formatted raw scores. If left blank file finder will pop up
  to allow you to select the file.

- output_folder:

  Output file pathway

  1.  Leave blank - This will output a csv file with the t-scores to
      your working directory

  2.  Specify a pathway - This will output a csv file to the specified
      pathway

  3.  Set to `NULL` - This will not output a csv file

## Value

table with t-scores attached to raw swan values
