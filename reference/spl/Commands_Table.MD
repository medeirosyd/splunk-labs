| Command | Description | Related commands |
|--------|-------------|------------------|
| abstract | Produces a summary of each search result. | highlight |
| accum | Keeps a running total of the specified numeric field. | autoregress, delta, trendline, streamstats |
| addcoltotals | Computes an event that contains sum of all numeric fields for previous events. | addtotals, stats |
| addinfo | Add fields that contain common information about the current search. | search |
| addtotals | Computes the sum of all numeric fields for each result. | addcoltotals, stats |
| analyzefields | Analyze numerical fields for their ability to predict another discrete field. | anomalousvalue |
| anomalies | Computes an "unexpectedness" score for an event. | anomalousvalue, cluster, kmeans, outlier |
| anomalousvalue | Finds and summarizes irregular, or uncommon, search results. | analyzefields, anomalies, cluster, kmeans, outlier |
| anomalydetection | Identifies anomalous events by computing a probability for each event and then detecting unusually small probabilities. | analyzefields, anomalies, anomalousvalue, cluster, kmeans, outlier |
| append | Appends subsearch results to current results. | appendcols, appendcsv, appendlookup, join, set |
| appendcols | Appends the fields of the subsearch results to current results. | append, appendcsv, join, set |
| appendpipe | Appends result of subpipeline applied to current result set. | append, appendcols, join, set |
| arules | Finds association rules between field values. | associate, correlate |
| associate | Identifies correlations between fields. | correlate, contingency |
| autoregress | Sets up data for calculating the moving average. | accum, autoregress, delta, trendline, streamstats |
| bin (bucket) | Puts continuous numerical values into discrete sets. | chart, timechart |
| bucketdir | Replaces a field value with higher grouping (directory-like). | cluster, dedup |
| chart | Returns results in tabular output for charting. | bin, sichart, timechart |
| cluster | Clusters similar events together. | anomalies, anomalousvalue, cluster, kmeans, outlier |
| cofilter | Counts frequency of two fields occurring together. | associate, correlate |
| collect | Puts search results into summary index. | overlap |
| concurrency | Finds number of concurrent events based on duration. | timechart |
| contingency | Builds a contingency table for two fields. | associate, correlate |
| convert | Converts field values into numerical values. | eval |
| correlate | Calculates correlation between fields. | associate, contingency |
| datamodel | Examine/search data model datasets. | pivot |
| dbinspect | Returns metadata about specified index. |  |
| dedup | Removes subsequent duplicate results. | uniq |
| delete | Delete specific events or search results. |  |
| delta | Computes difference in field value between events. | accum, autoregress, trendline, streamstats |
| diff | Returns difference between two results. |  |
| erex | Extract fields based on example values. | extract, kvform, multikv, regex, rex, xmlkv |
| eval | Calculates expression and stores into field. | where |
| eventcount | Returns number of events in index. | dbinspect |
| eventstats | Adds summary stats to all results. | stats |
| extract (kv) | Extracts key-value pairs from events. | kvform, multikv, xmlkv, rex |
| fieldformat | Format how field is displayed. | eval, where |
| fields | Keep or remove fields. |  |
| fieldsummary | Summary info for fields. | analyzefields, anomalies, anomalousvalue, stats |
| filldown | Replaces NULL with last non-null value. | fillnull |
| fillnull | Replaces NULLs with specified value. |  |
| findtypes | Generates suggested eventtypes. | typer |
| folderize | Higher-level grouping (folder-like). |  |
| foreach | Run subsearch for each matching field. | eval |
| format | Formats subsearch results into one result. |  |
| from | Retrieves data from dataset, lookup, or saved search. |  |
| gauge | Makes results suitable for gauge visualizations. |  |
| gentimes | Generates time ranges. |  |
| geom | Adds geographic polygon JSON structure. | geomfilter |
| geomfilter | Filters map data by bounding box. | geom |
| geostats | Stats grouped into geographic bins. | stats, xyseries |
| head | Takes first N results. | reverse, tail |
| highlight | Highlight terms. | iconify |
| history | Returns search history. | search |
| iconify | Adds icons to fields. | highlight |
| inputcsv | Load CSV results. | loadjob, outputcsv |
| inputlookup | Load lookup table. | inputcsv, lookup, outputlookup |
| iplocation | Extract geographic info from IP. |  |
| join | Join subsearch results. | appendcols, lookup, selfjoin |
| kmeans | k-means clustering. | anomalies, cluster, outlier |
| kvform | Extract fields using a form template. | extract |
| loadjob | Load results from completed job. | inputcsv |
| localize | Returns time ranges found. | map, transaction |
| localop | Run commands locally. |  |
| lookup | Perform lookup. |  |
| makecontinuous | Makes x-axis continuous. | chart, timechart |
| makemv | Create multivalue field. | mvcombine, mvexpand, nomv |
| makeresults | Create empty results. |  |
| map | Looping search. |  |
| mcollect | Convert results to metrics (SH). | collect |
| metadata | Returns list of sources/sourcetypes/hosts. | dbinspect |
| metasearch | Retrieves event metadata. | metadata, search |
| meventcollect | Convert to metrics (indexers). | collect |
| mpreview | Preview metric data. | mcatalog, mstats |
| msearch | Alias for mpreview. | mstats |
| mstats | Metrics statistics. | stats, tstats |
| multikv | Extracts values from table-like events. |  |
| multisearch | Run multiple searches. | append, join |
| mvcombine | Combine events into multivalue field. | mvexpand, makemv |
| mvexpand | Expand multivalue into events. | mvcombine, makemv |
| nomv | Convert multivalue to single value. | makemv |
| outlier | Removes outliers. | anomalies, cluster, kmeans |
| outputcsv | Export to CSV. | inputcsv |
| outputlookup | Write to lookup. | inputlookup, lookup |
| outputtext | Output _raw as _xml. | outputcsv |
| overlap | Find overlapping summary events. | collect |
| pivot | Pivot from DM datasets. | datamodel |
| predict | Time series prediction. | x11 |
| rangemap | Assign RANGE label. |  |
| rare | Least common values. | sirare, stats, top |
| redistribute | Parallel reduce for high-cardinality. |  |
| regex | Filter by regex. | rex, search |
| reltime | Convert time diff to readable. | convert |
| rename | Rename fields. |  |
| replace | Replace values. |  |
| require | Fail search if no results. |  |
| rest | Call REST endpoints. |  |
| return | Return values from subsearch. | format |
| reverse | Reverse results. | head, sort, tail |
| rex | Regex extraction. | extract |
| rtorder | Order real-time events. |  |
| savedsearch | Load saved search results. |  |
| script (run) | Run external script. |  |
| scrub | Anonymize fields. |  |
| search | Search indexes. |  |
| searchtxn | Transaction search. | transaction |
| selfjoin | Join results with themselves. | join |
| sendalert | Trigger alert action. |  |
| sendemail | Email results. |  |
| set | Set operations. | append, join |
| setfields | Set fields for all results. | eval |
| sichart | Summary-index chart. | chart |
| sirare | Summary-index rare. | rare |
| sistats | Summary-index stats. | stats |
| sitimechart | Summary-index timechart. | chart |
| sitop | Summary-index top. | top |
| sort | Sort results. | reverse |
| spath | Extract JSON/XML. | xpath |
| stats | Statistical aggregations. | eventstats, top, rare |
| strcat | Concatenate strings. |  |
| streamstats | Streaming stats. | stats |
| table | Create table. | fields |
| tags | Add tags to fields. | eval |
| tail | Last N results. | head |
| timechart | Time series chart. | chart |
| timewrap | Wrap timechart. | timechart |
| tojson | Convert to JSON. |  |
| top | Most common values. | rare, stats |
| transaction | Group events into transactions. |  |
| transpose | Row-to-column. |  |
| trendline | Moving averages. | timechart |
| tscollect | Create tsidx files. | collect, stats |
| tstats | Stats over tsidx. | tscollect |
| typeahead | Typeahead metadata. |  |
| typelearner | Deprecated. | findtypes |
| typer | Identify eventtypes. | findtypes |
| union | Merge datasets. |  |
| uniq | Remove duplicates. | dedup |
| untable | Convert table to stats format. | xyseries |
| walklex | List indexed terms. | metadata, tstats |
| where | Filter results. | eval |
| x11 | Remove seasonality. | predict |
| xmlkv | Extract XML KV pairs. | extract |
| xmlunescape | Unescape XML. |  |
| xpath | Extract XML fields. |  |
| xyseries | Make graphable dataset. |  |

