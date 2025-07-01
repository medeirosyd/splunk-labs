# Step-by-Step Splunk Ingestion

---

## 1. Data enters Splunk through inputs

- Splunk listens or watches for incoming data through inputs.
- Inputs can be:
  - **File monitor** (reads from files or directories on disk)
  - **TCP/UDP listener** (receives data over network ports)
  - **HTTP Event Collector** (receives data via HTTP/S requests)
  - **Scripted input or modular input)

👉 At this point, data is raw — it is just a stream of bytes.

---

## 2. Data passes to the input queue

- The input queue is the first buffer that temporarily holds data as Splunk processes it.
- **Purpose:** Smooth data flow and prevent overload.

---

## 3. Data enters the parsing pipeline

- Splunk breaks the data into individual events.
- Timestamps are extracted (or assigned if missing).
- Metadata is assigned:
  - **host**: originating system
  - **source**: file path, port, or input name
  - **sourcetype**: data format type that tells Splunk how to parse it
- Configuration files that can influence parsing:
  - `props.conf` — controls how data is broken into events and timestamp extraction
  - `transforms.conf` — used for advanced processing, such as masking or routing

---

## 4. Data enters the parsing queue

- After event breaking and metadata assignment, data enters the parsing queue.
- Another buffer to handle flow before indexing.

---

## 5. Data enters the indexing pipeline

- Splunk compresses the raw event data.
- Splunk generates index files (TSIDX) that map keywords, metadata, and locations.

---

## 6. Data enters the indexing queue

- The final buffer before data is written to disk.
- Prevents bottlenecks between parsing and storage.

---

## 7. Data is written to index buckets

- Splunk writes the data to disk in indexes.
- The data is stored in **buckets**:
  - **Hot:** Receiving active data.
  - **Warm:** Recently indexed data, no longer being written to.
  - **Cold:** Older data moved for storage efficiency.
  - **Frozen:** Data that will be deleted or archived.
- Each bucket contains:
  - Raw data (compressed)
  - TSIDX files (for fast search)

---

## Summary pipeline flow

`Input → Input queue → Parsing pipeline → Parsing queue → Indexing pipeline → Indexing queue → Disk (bucket in an index)`

---

## Technical note

Splunk ingestion is designed for high performance. Each queue prevents data loss and balances the flow. The entire process ensures that raw machine data is transformed into structured, searchable events stored efficiently on disk.