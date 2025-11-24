# universal forwarder

noun

A type of forwarder, which is a Splunk Enterprise instance that sends data to another Splunk Enterprise instance or to a third-party system.

The universal forwarder is a dedicated, streamlined version of Splunk Enterprise that contains only the essential components needed to forward data. The universal forwarder does not support python and does not expose a UI.

In most situations, the universal forwarder is the best way to forward data to indexers. Its main limitation is that it forwards unparsed data, except in certain cases, such as structured data. You must use a heavy forwarder to route event-based data.
