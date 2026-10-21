# Telemetry Notes

Telemetry sampling interval: 30s

- Sampling runs on a fixed 30-second cadence so numbers stay comparable across runs.
- Every emitted data point carries a source label so we can split results per environment later.
- Sampling overhead is negligible at this interval, but bumping it lower should be a deliberate decision, not an accident.
- Interval changes must be announced in the changelog so dashboards don't silently shift.
