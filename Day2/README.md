## Day 2

Email : yiserom817@careney.com
Splunk has 3 components, Forwarder, Indexer, and Search Head

Forward is an agent
Indexer is the database
Search head in the web

---

## Deployment Model

- Single Instance =
- Distributed
- Clustered

- **Forwarder IP**
  - The forwarder IP is the IP address of the machine where the Splunk Universal Forwarder is installed.
- **Receiving IP**
  - The receiving IP is the IP address of the Splunk Indexer/receiver that will receive the logs.

```bash
Linux Server
IP:
    192.168.1.20
        │
        │
        ▼Universal Forwarder
    192.168.1.20
        │
        │ TCP 9997
        ▼Splunk Indexer
    192.168.1.10
```

lorem10 hello World
