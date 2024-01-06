# Dataflow Batching

Processing data in chunks

## Working in batches

When processing large amounts or continuously updating data,
working in batches a number of benefits:

- provides visibility during a run instead of waiting until the end
- enables more tolerance for errors
- improves interactions with downstream systems
    - API calls do not need to be granular, they can be batched for efficiency
    - batch size can be tailored for optimal request processing
    - requests can be throttle to avoid overwhelming systems
- reduces memory size required for processing
- through tuning, can process data faster

## Standardized Approach

The goal of this repo is to gather designs, tools and templates for batch processing using dataflows.

Conventions included here will enable best practices to be built up.
Not only will this speed up projects leveraging them,
it will allow for integration of components which should lead to building momentum.

![Overview of batch processing with dataflows](docs/design/dataflow_batching_design_v1.drawio.svg)
