# rex

Use the SPL2 rex command to either extract fields using regular expression named groups, or replace or substitute characters in a field using sed expressions.

The rex command matches the value of the specified field against the unanchored regular expression and extracts the named groups into fields of the corresponding names.

## Sample usage

...| rex "expression | with pipe"

...rex field=clientip "(?<ipclass>\\d+)"

...rex field=clientip /(?<ipclass>\d+)/
