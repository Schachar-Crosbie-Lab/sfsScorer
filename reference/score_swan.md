# Run analysis on SWAN raw values to return t-scores

score_swan() returns gendered and non-gendered t-scores for the
Strengths and Weaknesses of ADHD Symptoms and Normal Behavior Rating
Scale (SWAN) assessment

**\[experimental\]**

## Usage

``` r
score_swan(df = NULL, file = FALSE, output_folder = NULL, ignore_check = FALSE)
```

## Arguments

- df:

  If you already have the SWAN data in your R environment, pass the
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

- ignore_check:

  Data are validated to look for missing or improperly formatted values
  before scoring. Errors are thrown when data aren't valid; however,
  this can cause issues in real data sets where data vary for good
  reasons. To skip the validation process, set ignore_check to TRUE. NAs
  will be returned where data are invalid

## Value

table with t-scores attached to raw swan values

## Examples

``` r
score_swan(df = validate_data)
#> Error: object 'validate_data' not found
score_swan(df = validate_date, ignore_check = TRUE)
#> Error: object 'validate_date' not found


```
