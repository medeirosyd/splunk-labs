# forwarder

noun

A Splunk Enterprise instance that forwards data to another Splunk Enterprise instance, such as an indexer or another forwarder, or to a third-party system.

There are three types of forwarders:

A universal forwarder is a dedicated, streamlined version of Splunk Enterprise that contains only the essential components needed to send data.
A heavy forwarder is a full Splunk Enterprise instance, with some features disabled to achieve a smaller footprint.
A light forwarder is a full Splunk Enterprise instance, with most features disabled to achieve a small footprint. The universal forwarder supersedes the light forwarder for nearly all purposes. The light forwarder has been deprecated as of Splunk Enterprise version 6.0.0.
The universal forwarder is the best tool for forwarding data to indexers. Its main limitation is that it forwards only unparsed data. To send event-based data to indexers, you must use a heavy forwarder.
