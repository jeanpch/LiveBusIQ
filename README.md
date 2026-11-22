# LiveBus — Real-Time Transit Radar for Garmin Watches

[![Garmin Connect IQ](https://img.shields.io/badge/Garmin%20Connect%20IQ-Download%20App-007CC3?style=for-the-badge&logo=garmin&logoColor=white)](https://apps.garmin.com/apps/bdcf21c2-42de-429b-9a2d-4250ac89a2b2)
[![Live Coverage Map](https://img.shields.io/badge/Live%20Coverage%20Map-Explore%20Networks-26A669?style=for-the-badge)](https://livebus.ploa33.workers.dev/map)

**Real-time public transit departures from any stop, right on your Garmin watch.**

> **Note:** This repository is the public showcase, documentation, and issue tracker for **LiveBusIQ**. The application and backend source code are maintained in a private repository.

---

### Live Links

* **Install on your watch:** [Garmin Connect IQ Store](https://apps.garmin.com/apps/bdcf21c2-42de-429b-9a2d-4250ac89a2b2)
* **Interactive network & stop coverage map:** [livebus.ploa33.workers.dev/map](https://livebus.ploa33.workers.dev/map) *(updated automatically in real time)*

---

### Highlights & Architecture

* **190+ Real-Time Transit Networks** — Live departures across France (RATP, SNCF, RTM, TCL, Tisséo…), UK (TfL, Manchester, Birmingham…), Germany (BVG, MVV, HVV…), Switzerland (SBB CFF FFS), Norway (Entur), Spain, Italy, Netherlands, Austria, North America, and more.
* **Garmin BLE Payload Engineering** — Strict `< 1,500 bytes` payload budget designed specifically for Garmin Bluetooth Low Energy transfers.
* **Sub-50 ms Edge Backend** — Powered by **Cloudflare Workers** + **Cloudflare D1** (SQLite spatial bounding-box indexing, Haversine ranking, 30s TTL edge caching with ~110 m spatial quantization).
* **Native Connect IQ App** — Built in **Monkey C** with Glance view and AMOLED display support.
* **Automated GTFS Sync** — Weekly scheduled ingestion of global transit feeds (GTFS / GTFS-RT / SIRI).

---

### Feedback & Network Requests

Missing a city or transit network, or spotted an issue?  
👉 **[Open an issue](https://github.com/jeanpch/LiveBusIQ/issues)** with the city and transit operator name.
