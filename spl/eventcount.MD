# eventcount

Returns the number of events in specified indexes.

## Sample usage

| eventcount summarize=false index=_audit index=main

| eventcount summarize=false index=_* report_size=true

| eventcount summarize=false index=*

| eventcount summarize=f list_federated_remote=t index=access_* index=federated:access_*
