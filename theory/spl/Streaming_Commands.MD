| Command | Notes | Example 1 | Example 2 | Example 3 |
|---------|--------|---------|---------|---------|
| addinfo | Distributable streaming |  |  |  |
| addtotals | Distributable streaming. A transforming command when used to calculate column totals (not row totals). |  |  |  |
| arules | Some of the work is distributable streaming running on the indexer or the search head. The rest is centralized streaming on the search head. |  |  |  |
| autoregress | Centralized streaming. |  |  |  |
| bin | Streaming if specified with span. Otherwise dataset processing. |  |  |  |
| bucketdir | Distributable streaming by default; centralized streaming if local=true in commands.conf. |  |  |  |
| cluster | Streaming in some modes. |  |  |  |
| convert | Distributable streaming. |  |  |  |
| dedup | Distributable streaming pre-dedup; centralized streaming after merging; becomes dataset-processing with sortby or keepevents=true. |  |  |  |
| eval | Distributable streaming. |  |  |  |
| extract | Distributable streaming. |  |  |  |
| fieldformat | Distributable streaming. |  |  |  |
| fields | Distributable streaming. |  |  |  |
| fillnull | Streaming when field-list is specified; dataset processing when no field-list. |  |  |  |
| head | Centralized streaming. |  |  |  |
| highlight | Distributable streaming. |  |  |  |
| iconify | Distributable streaming. |  |  |  |
| iplocation | Distributable streaming. |  |  |  |
| join | Centralized streaming when join fields are defined; dataset processing when no field-list. |  |  |  |
| lookup | Distributable streaming when local=false (default); orchestrating when local=true. |  |  |  |
| makemv | Distributable streaming. |  |  |  |
| multikv | Distributable streaming. |  |  |  |
| mvexpand | Distributable streaming. |  |  |  |
| nomv | Distributable streaming. |  |  |  |
| rangemap | Distributable streaming. |  |  |  |
| regex | Distributable streaming. |  |  |  |
| reltime | Distributable streaming. |  |  |  |
| rename | Distributable streaming. |  |  |  |
| replace | Distributable streaming. |  |  |  |
| rex | Distributable streaming. |  |  |  |
| search | Distributable streaming if not first command; generating when first in the pipeline. |  |  |  |
| spath | Distributable streaming. |  |  |  |
| strcat | Distributable streaming. |  |  |  |
| streamstats | Centralized streaming. |  |  |  |
| tags | Distributable streaming. |  |  |  |
| transaction | Centralized streaming. |  |  |  |
| typer | Distributable streaming. |  |  |  |
| where | Distributable streaming. |  |  |  |
| untable | Distributable streaming. |  |  |  |
| xmlkv | Distributable streaming. |  |  |  |
| xmlunescape | Distributable streaming by default; centralized streaming if local=true in commands.conf. |  |  |  |
| xpath | Distributable streaming. |  |  |  |
| xyseries | Distributable streaming when grouped=false (default); transforming when grouped=true. |  |  |  |
