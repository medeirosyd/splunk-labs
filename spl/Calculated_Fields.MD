# Calculated fields

Calculated fields are fields added to events at search time that perform calculations with the values of two or more fields already present in those events. Use calculated fields as a shortcut for performing repetitive, long, or complex transformations using the eval command.

## Sample

[<window_app>]
EVAL-appLength = if(response_code=200,len(app),null)

EVAL-field = coalesce(field, <eval expression>)

EVAL-field = coalesce(<eval expression>, field)

[<foo>]
EVAL-x = x * 2
EVAL-y = x * 2

[<access_common>]
EVAL-response_time =  response_time/1000
EVAL-bitrate = bytes*1000/response_time
