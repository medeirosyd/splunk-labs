| Command | Description | Related commands | Sample 1 | Sample 2 | Sample 3 | Sample 4 |
|--------|-------------|------------------|-----------|-----------|-----------|-----------|
| abstract | Produces a summary of each search result. | highlight |  |  |  |  |
| accum | Keeps a running total of the specified numeric field. | autoregress, delta, trendline, streamstats |  |  |  |  |
| addcoltotals | Computes an event that contains sum of all numeric fields for previous events. | addtotals, stats |  |  |  |  |
| addinfo | Add fields that contain common information about the current search. | search |  |  |  |  |
| addtotals | Computes the sum of all numeric fields for each result. | addcoltotals, stats |  |  |  |  |
| analyzefields | Analyze numerical fields for their ability to predict another discrete field. | anomalousvalue |  |  |  |  |
| anomalies | Computes an "unexpectedness" score for an event. | anomalousvalue, cluster, kmeans, outlier |  |  |  |  |
| anomalousvalue | Finds and summarizes irregular, or uncommon, search results. | analyzefields, anomalies, cluster, kmeans, outlier |  |  |  |  |
| anomalydetection | Identifies anomalous events by computing a probability for each event and then detecting unusually small probabilities. | analyzefields, anomalies, anomalousvalue, cluster, kmeans, outlier |  |  |  |  |
| append | Appends subsearch results to current results. | appendcols, appendcsv, appendlookup, join, set |  |  |  |  |
| appendcols | Appends the fields of the subsearch results to current results, first results to first result, second to second, etc. | append, appendcsv, join, set |  |  |  |  |
| appendpipe | Appends the result of the subpipeline applied to the current result set to results. | append, appendcols, join, set |  |  |  |  |
| arules | Finds association rules between field values. | associate, correlate |  |  |  |  |
| associate | Identifies correlations between fields. | correlate, contingency |  |  |  |  |
| autoregress | Sets up data for calculating the moving average. | accum, autoregress, delta, trendline, streamstats |  |  |  |  |
| bin (bucket) | Puts continuous numerical values into discrete sets. | chart, timechart |  |  |  |  |
| bucketdir | Replaces a field value with higher-level grouping, such as replacing filenames with directories. | cluster, dedup |  |  |  |  |
| chart | Returns results in a tabular output for charting. | bin, sichart, timechart |  |  |  |  |
| cluster | Clusters similar events together. | anomalies, anomalousvalue, cluster, kmeans, outlier |  |  |  |  |
| cofilter | Finds how many times field1 and field2 values occurred together. | associate, correlate |  |  |  |  |
| collect | Puts search results into a summary index. | overlap |  |  |  |  |
| concurrency | Uses a duration field to find the number of concurrent events for each event. | timechart |  |  |  |  |
| contingency | Builds a contingency table for two fields. | associate, correlate |  |  |  |  |
| convert | Converts field values into numerical values. | eval |  |  |  |  |
| correlate | Calculates the correlation between different fields. | associate, contingency |  |  |  |  |
| datamodel | Examine data model or dataset and search a data model dataset. | pivot |  |  |  |  |
| dbinspect | Returns information about the specified index. |  |  |  |  |  |
| dedup | Removes subsequent results that match a specified criteria. | uniq |  |  |  |  |
| delete | Delete specific events or search results. |  |  |  |  |  |
| delta | Computes the difference in field value between nearby results. | accum, autoregress, trendline, streamstats |  |  |  |  |
| diff | Returns the difference between two search results. |  |  |  |  |  |
| erex | Automatically extract fields based on example values. | extract, kvform, multikv, regex, rex, xmlkv |  |  |  |  |
| eval | Calculates an expression and puts the value into a field. | where | ... | eval full_name = first_name." ".last_name |  |  |  |
| eventcount | Returns the number of events in an index. | dbinspect |  |  |  |  |
| eventstats | Adds summary statistics to all search results. | stats |  |  |  |  |
| extract (kv) | Extracts field-value pairs from search results. | kvform, multikv, xmlkv, rex |  |  |  |  |
| fieldformat | Format how a field is displayed without changing underlying value. | eval, where |  |  |  |  |
| fields | Keeps or removes fields from search results. |  |  |  |  |  |
| fieldsummary | Generates summary information for fields. | analyzefields, anomalies, anomalousvalue, stats |  |  |  |  |
| filldown | Replaces NULL values with last non-NULL value. | fillnull |  |  |  |  |
| fillnull | Replaces NULLs with a specified value. |  |  |  |  |  |
| findtypes | Generates suggested eventtypes. | typer |  |  |  |  |
| folderize | Higher-level grouping (similar to bucketdir). |  |  |  |  |  |
| foreach | Runs a subsearch for each field that matches a wildcard. | eval |  |  |  |  |
| format | Formats subsearch results into a single result. |  |  |  |  |  |
| from | Retrieves data from a dataset (DM, CSV, lookup, saved search). |  |  |  |  |  |
| gauge | Makes results suitable for gauge visualizations. |  |  |  |  |  |
| gentimes | Generates time ranges. |  |  |  |  |  |
| geom | Adds geographic polygon structure JSON to events. | geomfilter |  |  |  |  |
| geomfilter | Filters map data by bounding box. | geom |  |  |  |  |
| geostats | Stats grouped into geographic bins. | stats, xyseries |  |  |  |  |
| head | Takes first N results. | reverse, tail |  |  |  |  |
| highlight | Highlights specified terms. | iconify |  |  |  |  |
| history | Returns search history. | search |  |  |  |  |
| iconify | Adds icons to fields. | highlight |  |  |  |  |
| inputcsv | Load CSV results. | loadjob, outputcsv |  |  |  |  |
| inputlookup | Load lookup table. | inputcsv, lookup, outputlookup |  |  |  |  |
| iplocation | Extract geographic info from IP. |  |  |  |  |  |
| join | Join subsearch results. | appendcols, lookup, selfjoin |  |  |  |  |
| kmeans | Performs k-means clustering. | anomalies, cluster, outlier |  |  |  |  |
| kvform | Extract fields using a form template. | extract |  |  |  |  |
| loadjob | Loads results of completed job. | inputcsv |  |  |  |  |
| localize | Returns time ranges found. | map, transaction |  |  |  |  |
| localop | Run commands locally instead of distributed. |  |  |  |  |  |
| lookup | Perform lookup. |  |  |  |  |  |
| makecontinuous | Makes x-axis continuous. | chart, timechart |  |  |  |  |
| makemv | Creates multivalue field. | mvcombine, mvexpand, nomv |  |  |  |  |
| makeresults | Create empty results. |  |  |  |  |  |
| map | Looping search for each result. |  |  |  |  |  |
| mcollect | Convert results to metrics (search head). | collect |  |  |  |  |
| metadata | Returns list of sources/sourcetypes/hosts. | dbinspect |  |  |  |  |
| metasearch | Retrieves event metadata. | metadata, search |  |  |  |  |
| meventcollect | Convert results to metrics (indexers). | collect |  |  |  |  |
| mpreview | Preview metric data. | mcatalog, mstats |  |  |  |  |
| msearch | Alias for mpreview. | mstats |  |  |  |  |
| mstats | Metrics statistics. | stats, tstats |  |  |  |  |
| multikv | Extracts values from table formatted events. |  |  |  |  |  |
| multisearch | Run multiple searches at once. | append, join |  |  |  |  |
| mvcombine | Combine events into multivalue field. | mvexpand, makemv |  |  |  |  |
| mvexpand | Expand MV field into separate events. | mvcombine, makemv |  |  |  |  |
| nomv | Turn multivalue field into single value. | makemv |  |  |  |  |
| outlier | Removes outliers. | anomalies, cluster, kmeans |  |  |  |  |
| outputcsv | Export to CSV. | inputcsv |  |  |  |  |
| outputlookup | Write to lookup table. | inputlookup, lookup |  |  |  |  |
| outputtext | Output _raw into _xml. | outputcsv |  |  |  |  |
| overlap | Find overlapping summary events. | collect |  |  |  |  |
| pivot | Pivot search against DM datasets. | datamodel |  |  |  |  |
| predict | Time series prediction. | x11 |  |  |  |  |
| rangemap | Assign a RANGE label. |  |  |  |  |  |
| rare | Least common values. | sirare, stats, top |  |  |  |  |
| redistribute | Parallel reduce for high-cardinality data. |  |  |  |  |  |
| regex | Filter by regex. | rex, search |  |  |  |  |
| reltime | Convert difference between now and _time to human readable. | convert |  |  |  |  |
| rename | Rename fields. |  |  |  |  |  |
| replace | Replace values. |  |  |  |  |  |
| require | Fail search if preceding commands return zero results. |  |  |  |  |  |
| rest | Call REST endpoints. |  |  |  |  |  |
| return | Return values from a subsearch. | format |  |  |  |  |
| reverse | Reverse order. | head, sort, tail |  |  |  |  |
| rex | Extract fields with regex. | extract |  |  |  |  |
| rtorder | Order real-time events. |  |  |  |  |  |
| savedsearch | Load results of saved search. |  |  |  |  |  |
| script (run) | Run external script. |  |  |  |  |  |
| scrub | Anonymize results. |  |  |  |  |  |
| search | Search indexes. |  |  |  |  |  |
| searchtxn | Transaction search. | transaction |  |  |  |  |
| selfjoin | Join results with themselves. | join |  |  |  |  |
| sendalert | Invoke alert action. |  |  |  |  |  |
| sendemail | Email search results. |  |  |  |  |  |
| set | Set operations. | append, join |  |  |  |  |
| setfields | Set fields for all results. | eval |  |  |  |  |
| sichart | Summary-index chart. | chart |  |  |  |  |
| sirare | Summary-index rare. | rare |  |  |  |  |
| sistats | Summary-index stats. | stats |  |  |  |  |
| sitimechart | Summary-index timechart. | chart |  |  |  |  |
| sitop | Summary-index top. | top |  |  |  |  |
| sort | Sort results. | reverse |  |  |  |  |
| spath | Extract from JSON/XML. | xpath |  |  |  |  |
| stats | Statistical functions. | eventstats, top, rare |  |  |  |  |
| strcat | Concatenate strings. |  |  |  |  |  |
| streamstats | Streaming stats. | stats |  |  |  |  |
| table | Create table. | fields |  |  |  |  |
| tags | Add tags to fields. | eval |  |  |  |  |
| tail | Last N results. | head |  |  |  |  |
| timechart | Time series chart. | chart |  |  |  |  |
| timewrap | Wrap timechart output. | timechart |  |  |  |  |
| tojson | Convert to JSON. |  |  |  |  |  |
| top | Most common values. | rare, stats |  |  |  |  |
| transaction | Group events into transactions. |  |  |  |  |  |
| transpose | Rows → columns. |  |  |  |  |  |
| trendline | Moving averages. | timechart |  |  |  |  |
| tscollect | Create tsidx files. | collect, stats |  |  |  |  |
| tstats | Stats over tsidx files. | tscollect |  |  |  |  |
| typeahead | Typeahead info. |  |  |  |  |  |
| typelearner | Deprecated. | findtypes |  |  |  |  |
| typer | Identify eventtypes. | findtypes |  |  |  |  |
| union | Merge datasets. |  |  |  |  |  |
| uniq | Remove duplicates. | dedup |  |  |  |  |
| untable | Convert table → stats-like format. | xyseries |  |  |  |  |
| walklex | List indexed terms. | metadata, tstats |  |  |  |  |
| where | Filter results. | eval |  |  |  |  |
| x11 | Remove seasonality. | predict |  |  |  |  |
| xmlkv | Extract XML KV pairs. | extract |  |  |  |  |
| xmlunescape | Unescape XML. |  |  |  |  |  |
| xpath | Extract XML fields. |  |  |  |  |  |
| xyseries | Make graphable dataset. |  |  |  |  |  |
