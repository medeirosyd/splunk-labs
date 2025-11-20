# erex

Use the erex command to extract data from a field when you do not know the regular expression to use. The command automatically extracts field values that are similar to the example values you specify.
The values extracted from the fromfield argument are saved to the field. The search also returns a regular expression that you can then use with the rex command to extract the field.

## Sample

... | erex monthday examples="7/01"

... | erex monthday examples="7/01, 07/02" counterexamples="99/2"

sourcetype=secure* port "failed password"

sourcetype=secure* port "failed password" | erex port examples="port 3351, port 3768" | top port

sourcetype=secure* port "failed password" | rex (?i)^(?:[^\.]*\.){3}\d+\s+(?P<port>\w+\s+\d+) | top port
