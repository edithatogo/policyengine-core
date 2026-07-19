# Product Definition

PolicyEngine Core is the shared microsimulation engine used by PolicyEngine
country packages, applications, and APIs. It provides simulation, parameter,
variable, entity, holder, reform, tracing, and test-runner primitives.

## Users

- Maintainers of PolicyEngine Core and country packages.
- Developers building reforms, simulations, APIs, and analysis tools.
- Contributors extending or documenting stable engine behavior.

## Goals

- Preserve deterministic and explainable policy calculations.
- Maintain compatible, documented public interfaces across supported Python
  versions.
- Validate changes with focused tests and repository-wide hosted checks.
- Record fork governance work without implying upstream acceptance.

## Non-goals

- Country-specific policy implementation.
- Publishing releases or modifying the upstream repository from fork-local
  governance tracks.
- Treating controlled-fork evidence as independent verification.
