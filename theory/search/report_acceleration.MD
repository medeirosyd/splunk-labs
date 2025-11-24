# report acceleration

noun

A process in Splunk Enterprise that speeds up a transforming search or a report that takes a long time to finish because they run on large data sets. It creates a separate summary of the data on the indexer. It stores the summary data within ordinary indexes parallel to the bucket or buckets that cover the range of time over which the summary spans. Splunk Enterprise runs subsequent searches on the summary data, not on the _raw index, quickly returning the search results. Use Splunk Web to enable, review, and manage your report acceleration summaries.
