# TLDR

## Two parts

1. Observability by tracing/logging out data.
2. Perfroming evals on these datasets.

Agents/tools are (mathematically) a function with:

- input
- output
- context (optionally)
- metadata (model, temperature, etc.)

Each Agent has its own **observability** by exporting the above to a CSV that can then be analysed using a range of Eval Libraries like Evidently, DeepEval and Ragas, with or without references (ground truths).

![Log](./images/example_log_print.png)

> Add REFERENCE column to dataset and then do evals.

Advantages:

> Decouples app code and evaluation code.


> Portable Agent/Eval combinations.


> Evals are real time and support both developer and QA.


> Frictionless integration to existing apps and new ones.
