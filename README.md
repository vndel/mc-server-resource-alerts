# Minecraft Server Resource Alerts

Starter alert definitions for host and JVM signals that affect Paper backends and Velocity proxies. Thresholds below are examples only: calibrate them from service baselines and test alert routing before production use.

## Alert design
- Alert on sustained symptoms and user impact, not a single transient sample.
- Separate warning from page-worthy conditions and include an actionable runbook link.
- Monitor MSPT, process health, heap/GC pauses, disk free space, and backend connectivity.
- Avoid labels containing player UUIDs, IP addresses, or other high-cardinality personal data.
- Review thresholds after workload, plugin, JVM, or hardware changes.

## Files
- `rules.yml`: illustrative Prometheus-style rules; validate syntax in your monitoring stack.
- `runbook.md`: initial response guidance.

These examples are not production-ready without local validation.