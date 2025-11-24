# data model acceleration

A data-summary-backed method of accelerating the datasets within data models, causing pivot searches on that dataset to run much faster than they would otherwise. The collection of summaries that a data model uses for acceleration is called the high performance analytics store.

There are two types of data model acceleration:

Persistent data model acceleration: When a data model is manually enabled for acceleration over a specific range of time and remains accelerated until it is disabled.
Ad-hoc data model acceleration: The automatic acceleration of data models that are not manually enabled for acceleration, creating a temporary summary that is deleted when the user leaves the Pivot Editor.
