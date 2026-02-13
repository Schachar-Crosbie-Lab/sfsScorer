# Run analysis on TOCS raw values to return t-scores

score_tocs2() returns gendered and non-gendered t-scores for the
[Toronto Obsessive-Compulsive Scale (TOCS)
assessment](https://pubmed.ncbi.nlm.nih.gov/27015722/)

**\[experimental\]**

## Usage

``` r
score_tocs2(df = NULL, file = FALSE, output_folder = NULL, max_missing = 0)
```

## Arguments

- df:

  If you already have the TOCS-2 data in your R environment, pass the
  dataframe to this parameter

- file:

  If you prefer scoring a spreadsheet...

  1.  TRUE - This will pop-up a finder to allow you select a file

  2.  Specify a pathway

- output_folder:

  Output file pathway

  1.  Leave blank - This will output a csv file with the t-scores to
      your working directory

  2.  Specify a pathway - This will output a csv file to the specified
      pathway

  3.  Set to `NULL` - This will not output a csv file

- max_missing:

  By default, 0 items are allowed to be missing on the TOCS. Any
  questionnaire with 1 or more missing, will not be scored. If you'd
  like to adjust this number, change the max_missing value. This will
  use a prorated score to generate t-scores. Please be aware that
  missingness can induce issues when analyzing.

## Value

table with t-scores attached to raw swan values
