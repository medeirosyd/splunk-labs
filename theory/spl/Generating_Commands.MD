| Command | Notes | Sample 1 | Sample 2 | Sample 3 | Sample 4 |
|---------|--------|----------|----------|----------|----------|
| datamodel | Report-generating |  |  |  |  |
| dbinspect | Report-generating |  |  |  |  |
| eventcount | Report-generating |  |  |  |  |
| from | Can be report-generating or event-generating depending on referenced dataset or knowledge object |  |  |  |  |
| gentimes | Event-generating |  |  |  |  |
| inputcsv | Event-generating (centralized) |  |  |  |  |
| inputlookup | Event-generating (centralized) when append=false (default) |  |  |  |  |
| loadjob | Event-generating (centralized) |  |  |  |  |
| makeresults | Report-generating |  |  |  |  |
| metadata | Report-generating. Fetches data from all peers, but subsequent commands run only on search head |  |  |  |  |
| metasearch | Event-generating |  |  |  |  |
| mstats | Report-generating, except when append=true |  |  |  |  |
| multisearch | Event-generating |  |  |  |  |
| pivot | Report-generating |  |  |  |  |
| rest |  |  |  |  |  |
| search | Event-generating (distributable) when first command; streaming (distributable) when used later in pipeline |  |  |  |  |
| searchtxn | Event-generating |  |  |  |  |
| set | Event-generating |  |  |  |  |
| tstats | Report-generating (distributable), except when prestats=true. With prestats=true, becomes event-generating |  |  |  |  |
| typeahead | Event-generating |  |  |  |  |
| walklex | Event-generating |  |  |  |  |
