# eval command

The SPL2 eval command calculates an expression and puts the resulting value into a search results field.

## Sample usage

... | eval velocity=distance/time

... | eval error = if(status == 200, "OK", "Problem")

FROM all_month | eval Description=case(depth<=70, "Shallow", depth>70 AND depth<=300, "Mid", depth>300, "Deep") | stats count() min(Mag) max(Mag) by Description
