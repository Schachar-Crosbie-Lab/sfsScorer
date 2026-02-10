# Make Variables - Subset SWAN to subdomains.

Pass the root of the test with the question numbers to subset the SWAN.
1-9 = Inattentive. 10-18 = Hyperactive. Function to list all
questionnaire items (and not have to type them out) - used throughout a:
first item number (usually "1", but when referencing subdomains, or for
SWAN ODD, first item may be something other than 1 b: last item number
root: part of the item name that doesn't change (eg: for swan1 to
swan18, the root is "swan" )

## Usage

``` r
mkvars(a = NULL, b = NULL, root = "swan")
```

## Arguments

- a:

  First question of subset

- b:

  Last question of subset

- root:

  Root name of

## Value

A data frame ready for use or an error

## Author

Annie
