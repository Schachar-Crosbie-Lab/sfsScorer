# Clean File

This function runs checks to be sure that the file and non-test specific
data are formatted correctly

## Usage

``` r
clean_file(df = NULL, test = NULL, ignore_check = NULL)
```

## Arguments

- df:

  The df function allows you to point to a dataframe as opposed to a
  file

- test:

  Which questionnaire are we running#'

- ignore_check:

  Data are validated to look for missing or improperly formatted values
  before scoring. Errors are thrown when data aren't valid; however,
  this can cause issues in real data sets where data vary for good
  reasons. To skip the validation process, set ignore_check to TRUE. NAs
  will be returned where data are invalid

## Value

A clean data frame ready for t-scores
