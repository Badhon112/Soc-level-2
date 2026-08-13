1. Layout Options

- **Classic Dashboard**
  - Only Row-Column structure supported
  - Object are snap to row column structure.
- **Dashboard Studio**
  - Two different layout options, Absolute and grid.
  - Absolute layout has features like pixel-perfect placement, shapes, icons, and image uploading.
  - In Absolute layout we can use mouse or keyboard to drag and drop and resize objects

---

2. Source Code

- **Classic Dashboard**
  - Simple XML
- **Dashboard Studio**
  - JSON-formatted components, or stanzas

3. Visualization

After uploading the Kali_syslog.txt in splunk this the SPL(Search Processing Language) to get all the data

```bash

source="kali_syslog.txt" host="71f889c8eafa" sourcetype="Linux Log"

```
