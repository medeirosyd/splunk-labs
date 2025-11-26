# LIMIT

The LIMIT command in Splunk is used to specify the maximum number of results to return from a search.

You can specify a limit using the required syntax limit=
followed by the desired number of results. For example,
search ... 

| limit=10
.
Alternatively, you can use the limit argument without specifying the =character, like search ... | limit 10 . However, using limit=10 is recommended as it makes the limit value explicit.

If you don't specify any limit, the command defaults to the first 10 results.

Note that you can also use an eval expression to determine the limit, such as search ... 

| head (some_condition)

Additionally, you can control how the last result in the result set is handled using the
keeplast
argument.
