# Resource alert response

1. Confirm the affected service, environment, alert duration, and recent deployments.
2. Check correlated MSPT, GC, CPU, disk latency, free space, and backend health signals.
3. Prefer reversible mitigations with a known owner; do not kill the JVM or delete world data as a first response.
4. Communicate player impact and next update time through the approved status channel.
5. Verify recovery against the triggering metric and representative gameplay.
6. Record cause, duration, and follow-up actions; tune alert thresholds only after evidence review.
