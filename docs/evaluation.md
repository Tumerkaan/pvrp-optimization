# Evaluation and limitations

[Back to overview](../README.md)

## What is evaluated

| Dimension | Question |
| --- | --- |
| Service coverage | Are required visits represented with the intended frequency? |
| Daily capacity | Are visit-count and working-time constraints satisfied? |
| Workload balance | How uneven is work across the configured planning units? |
| Geographic overlap | How much do assigned service territories overlap under the chosen metric? |
| Search behavior | What changes under the same input, budget and initial solution? |

## Reading a result responsibly

The first gate is feasibility. Improvements in overlap or workload should be reported together with remaining violations. If a candidate still exceeds duration limits, it remains a diagnostic result rather than a deployment-ready plan.

Development notes document difficult instances with remaining duration violations. Consequently, this portfolio does not claim global optimality, universal feasibility or a production-ready scheduling service.

## Fair comparison protocol

For a future public benchmark, hold the input, constraints, runtime budget and warm-start conditions fixed. Record the solver revision, randomness settings when used, constraint violations and each objective independently. Report repeated runs where randomness affects the search. This protocol is a recommended reporting standard, not a new benchmark executed for this page.

## Evidence reviewed

This case study was prepared from the local project identity document, Streamlit UI source, UI documentation and development status notes. UI documentation describes an earlier solver variant; it must not be interpreted as the latest solver benchmark. No optimizer was run as part of publishing these pages.

## Next milestones

1. Select a redistributable synthetic instance.
2. Establish a reproducible feasibility baseline for that instance.
3. Publish a sanitized result table and route visualization.
4. Consider releasing a self-contained, reviewed code example.
