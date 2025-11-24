index

noun

The repository for data. When the Splunk platform indexes raw data, it transforms the data into searchable events.

Indexes reside in flat files on the indexer.

There are two types of indexes:

Events indexes. Events indexes are the default type of index. They can hold any type of data.
Metrics indexes. Metrics indexes hold only metric data.

verb

In general, the act of processing raw data and adding the processed data to an index.

Specifically, indexing is the third segment of the data pipeline, in which the indexer takes parsed events and writes them to the search index on disk.
