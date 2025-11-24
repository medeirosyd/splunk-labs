# distributed search

noun

A deployment topology that portions search management and search fulfillment/indexing activities across multiple Splunk Enterprise instances. In distributed search, a Splunk Enterprise instance, referred to as the search head, distributes search requests to other instances, called search peers, which perform the actual searching, as well as the data indexing. The search head merges the results back to the user.

Distributed search provides horizontal scaling, so that a single Splunk Enterprise deployment can search and index arbitrarily large amounts of data. Distributed search is also useful for correlating data across data silos.
