# event

noun

A single piece of data in Splunk software, similar to a record in a log file or other data input. When data is indexed, it is divided into individual events. Each event is given a timestamp, host, source, and source type. Often, a single event corresponds to a single line in your inputs, but some inputs (for example, XML logs) have multiline events, and some inputs have multiple events on a single line.

When a successful search is run, it returns either events or results. Events are returned if the commands in the search only filtered the data. Results are returned if one of the commands in the search is a transforming command.

Similar events can be categorized together with event types.

As an example, events are generated when the following search is run in the Search app:

| makeresults count=10 
| head 4
