# killercoda-packetlens

Interactive browser scenario for [Killercoda](https://killercoda.com) — run
**PacketLens** DPI inside FD.io VPP in about five minutes, with nothing to install.

The scenario starts the demo stack, watches VPP classify YouTube, Netflix, Zoom,
Spotify and eight other applications in real time, and opens a live Grafana
dashboard of per-application traffic counters.

## Layout

```
packetlens-demo/
├── index.json        Scenario definition
├── intro.md          Landing page
├── foreground.sh     Environment setup
├── step1/            Start the stack
├── step2/            Watch classification
├── step3/            Explore Grafana
└── finish.md         Wrap-up
```

## Related

- **[vpp-ndpi](https://github.com/packetlens/vpp-ndpi)** — the VPP plugin suite this demonstrates
- **[ndpi-observe](https://github.com/packetlens/ndpi-observe)** — TC/eBPF classifier, no VPP required
- **[vpp-rtp-asr](https://github.com/packetlens/vpp-rtp-asr)** — inline RTP tap with streaming speech recognition
- **[packetlens.dev](https://packetlens.dev)** — project site

> **Status: pre-production.** PacketLens is lab-validated on our own bench and not
> yet deployed in production. This scenario is a demonstration, not a benchmark.

## License

Apache 2.0. Built by [PacketFlow](https://packetflow.dev).
