## Step 3 — Grafana dashboard

Grafana is running on port 3000. Click the **Traffic** tab above the terminal to open it:

{{TRAFFIC_HOST1_3000}}

The dashboard loads automatically — **no login required**.

You'll see:
- **Top Applications** bar chart — YouTube, Netflix, GitHub, Zoom, Spotify, TikTok and more
- **Bytes/sec per app** time-series graph — counters updating every 15 seconds
- **Engine stats** — flows active, classification rate, memory usage

### CLI deep-dive (optional)

Show the nDPI plugin version:

```
docker exec packetlens-vpp vppctl show ndpi version
```{{exec}}

Show the live flow table:

```
docker exec packetlens-vpp vppctl show ndpi flows
```{{exec}}

Show per-interface statistics:

```
docker exec packetlens-vpp vppctl show ndpi interfaces
```{{exec}}
