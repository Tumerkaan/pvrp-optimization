# Periodic Vehicle Routing Optimization

Personal operations-research project by Tumer Kaan Mutlu.

**Case study:** [Architecture and decisions](docs/architecture.md) | [Evaluation and limitations](docs/evaluation.md) | [User walkthrough](docs/demo.md)

## Why this project matters

A geographically compact route is not automatically a valid weekly plan. Recurring visits must fit service-frequency rules and each representative's available time. This project explores that tension through an experimental planning engine and a configurable interface, making constraint violations visible rather than hiding them behind a single objective score.

## My role

I worked on the Python planning workflow, solver experiments, constraint diagnostics and comparisons between candidate outputs. The interface exposes planning preferences and execution budgets so that experiments can be repeated under explicit settings.

## Problem

Plan recurring visits across multiple days while managing daily visit limits, service frequency, working-time constraints, geographic overlap and workload balance.

## Engineering approach

- Python-based neighborhood-search and large-neighborhood-search experiments.
- Feasibility-first evaluation: check service and capacity constraints before interpreting objective improvements.
- Workload and geographic-overlap diagnostics, with expensive geometry reserved for selected candidates.
- Streamlit interface for input upload, warm starts, time budgets and workload/geometry preferences.
- Versioned experiments and structured evaluation logs to compare candidate routes.

## Workflow

Input and constraints -> candidate assignment and routes -> feasibility checks -> neighborhood search -> route output and diagnostic metrics.

## Status and limitations

This is an ongoing experimental solver, not a claim of global optimality or feasibility for every instance. Some development instances require further duration-feasibility work. No production performance or universal improvement percentage is claimed here.

## Publication scope

This repository is a documentation-only portfolio overview. Solver source, input datasets, customer locations, raw logs and internal experiment history are not included. It is not an installable release. Any future runnable example will use reviewed synthetic data.

## Contribution

Problem modeling, Python solver experimentation, constraint diagnostics, objective comparison and a parameterized planning interface.

## Contact

[GitHub profile](https://github.com/Tumerkaan)
