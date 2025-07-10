# TLDR

> Two decoupled parts - observability and evaluation.

## Observability

1. Observability by tracing/logging out data.
2. Performing evals on these datasets.

Agents/tools are (mathematically) a function with:

- input
- output
- context (optionally)
- metadata (model, temperature, etc.)

Each Agent has its own **self-reflection** by exporting the above to a CSV.

This CSV can then be analysed using a range of Eval Libraries like Evidently, DeepEval and Ragas, with or without references (ground truths).

![Log](./images/example_log_print.png)

## Evaluation

> Add REFERENCE column to dataset and then do evals.

Once we have our output dataset, we can add ground truths/references and then carry out evals using a range of libraries like Evidently.ai, (my favourite), RAGAS, DeepEval etc.

We can also create our own evals.

The log files are generated in real time enabling not just evaluation but also real time monitoring.

I have also found the log files very useful during development work and bug-fixing.

## Advantages

> Decouples app code and evaluation code.

> Portable Agent/Eval combinations.

> Evals are real time and support both developer and QA.

> Frictionless integration to existing apps and new ones.
