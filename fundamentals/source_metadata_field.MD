# source

noun

A default field that identifies the source of an event, that is, where the event originated. In the case of data monitored from files and directories, the source consists of the full pathname of the file or directory. In the case of a network-based source, the source field consists of the protocol and port, such as UDP:514.

Each event has a source field. The indexer generates the source field at index time. Searches often use the source as a criterion.
