# source type

noun

A default field that identifies the data structure of an event. A source type determines how the Splunk platform formats the data during the indexing process.

Example source types include access_combined and cisco_syslog.

The Splunk platform comes with a large set of predefined source types, and it assigns a source type to your data. You can override this assignment by assigning an existing source type or creating a custom source type.

The indexer identifies and adds the source type field when it indexes the data. As a result, each indexed event has a sourcetype field.

Use the sourcetype field in searches to find all data of a certain type (as opposed to all data from a certain source).
