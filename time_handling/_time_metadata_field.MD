# _time

When an event is processed by Splunk software, its timestamp is saved as the default field _time. This timestamp, which is the time when the event occurred, is saved in UNIX time notation. Searching with relative time modifiers, earliest or latest, finds every event with a timestamp beginning, ending, or between the specified timestamps.
For example, when you search for earliest=@d, the search finds every event with a _time value since midnight. This example uses @d, which is a date format variable.
