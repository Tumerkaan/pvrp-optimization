# User walkthrough

[Back to overview](../README.md)

This is a description of the local interface, not a hosted live demo. No customer data or actual route screenshot is published here.

## Typical session

1. Upload the planning input containing service and scheduling requirements.
2. Optionally supply previous route outputs as warm starts.
3. Choose a time budget and workload/geometry preference.
4. Review daily visit limits, workday duration and lunch settings.
5. Run the solver and inspect constraint diagnostics before judging route quality.
6. Review the route output together with run metrics and configuration.

## Example interpretation

Imagine one candidate reduces geographic overlap but leaves a daily duration violation, while another improves duration feasibility without improving overlap. The first candidate is not automatically better. The current optimization phase and explicit constraints determine which result is useful.

This example is illustrative; it is not an experimental result.

## Why no screenshot yet?

Real planning outputs may contain locations or operational information. A public visual should be generated from an explicitly synthetic input and clearly labeled. Until then, the architecture diagram and this walkthrough communicate the workflow without exposing private data.
