| Command | Notes | Sample 1 | Sample 2 | Sample 3 | Sample 4 |
|---------|--------|----------|----------|----------|----------|
| addinfo | Distributable streaming |  |  |  |  |
| addtotals | Distributable streaming. A transforming command when used to calculate column totals (not row totals). |  |  |  |  |
| arules | Some work is distributable streaming on indexer/search head; remaining work centralized streaming on search head. |  |  |  |  |
| autoregress | Centralized streaming. |  |  |  |  |
| bin | Streaming if span is specified; otherwise dataset processing. |  |  |  |  |
| bucketdir | Distributable streaming by default; centralized streaming if local=true in commands.conf. |  |  |  |  |
| cluster | Streaming in some modes. |  |  |  |  |
| convert | Distributable streaming. |  |  |  |  |
| dedup | Distributable streaming in prededup phase; centralized streaming after merge; dataset processing when sortby or keepevents=true. |  |  |  |  |
| eval | Distributable streaming. |  |  |  |  |
| extract | Distributable streaming. |  |  |  |  |
| fieldformat | Distributable streaming. |  |  |  |  |
| fields | Distributable streaming. |  |  |  |  |
| fillnull | Streaming when field-list specified; dataset processing when no field-list. |  |  |  |  |
| head | Centralized streaming. |  |  |  |  |
| highlight | Distributable streaming. |  |  |  |  |
| iconify | Distributable streaming. |  |  |  |  |
| iplocation | Distributable streaming. |  |  |  |  |
| join | Centralized streaming when join-fields defined; dataset processing when no field-list. |  |  |  |  |
| lookup | Distributable streaming when local=false; orchestrating when local=true. |  |  |  |  |
| makemv | Distributable streaming. |  |  |  |  |
| multikv | Distributable streaming. |  |  |  |  |
| mvexpand | Distributable streaming. |  |  |  |  |
| nomv | Distributable streaming. |  |  |  |  |
| rangemap | Distributable streaming. |  |  |  |  |
| regex | Distributable streaming. |  |  |  |  |
| reltime | Distributable streaming. |  |  |  |  |
| rename | Distributable streaming. |  |  |  |  |
| replace | Distributable streaming. |  |  |  |  |
| rex | Distributable streaming. |  |  |  |  |
| search | Distributable streaming further down the pipeline; generating when first command. |  |  |  |  |
| spath | Distributable streaming. |  |  |  |  |
| strcat | Distributable streaming. |  |  |  |  |
| streamstats | Centralized streaming. |  |  |  |  |
| tags | Distributable streaming. |  |  |  |  |
| transaction | Centralized streaming. |  |  |  |  |
| typer | Distributable streaming. |  |  |  |  |
| where | Distributable streaming. |  |  |  |  |
| untable | Distributable streaming. |  |  |  |  |
| xmlkv | Distributable streaming. |  |  |  |  |
| xmlunescape | Distributable streaming by default; centralized streaming if local=true in commands.conf. |  |  |  |  |
| xpath | Distributable streaming. |  |  |  |  |
| xyseries | Distributable streaming when grouped=false; transforming when grouped=true. |  |  |  |  |
