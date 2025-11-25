# table command

The table command is a transforming command in Splunk that returns a table formed by only the fields specified in the arguments. It displays columns in the same order as the fields are specified and uses the field names as column headers. Rows in the table represent individual events, and the command is used to retain data in a tabular format. The table command is similar to the fields command, but is specifically used when you want to retain data in a table format.

You can specify a list of valid field names as arguments, separated by spaces or commas, to include in the table. Wildcards can be used to specify fields with similar names. For example, "value*" would include all fields starting with "value".

The table command is a non-streaming command, and it's recommended to use it at the end of your searches to optimize performance. It doesn't allow field renaming, so if you need to rename a field, it should be done before piping the results to the table command.
