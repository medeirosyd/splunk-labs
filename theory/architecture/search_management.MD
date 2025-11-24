# search management

noun

The function of handling search requests and consolidating the results back to the user.

In the case of distributed searches, a dedicated Splunk Enterprise component, called the search head, handles search management. It distributes search requests across a set of search peers, which perform the actual searching, and then merges the results back to the user. In the case of a single-instance installation, one Splunk Enterprise instance handles search management along with the indexing and searching functions.
