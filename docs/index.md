# TLDR

Agents/tools are (mathematically) a function with:

- input
- output
- context (optionally)
- metadata (model, temperature, etc.)

Each Agent contains its own **self-evaluation** by exporting the above to a CSV that can then be analysed using a range of Eval Libraries like Evidently, DeepEval and Ragas.

![Log](./images/example_log_print.png)

> Decouple app code and evaluation code.

> Portable Agent/Eval combinations.

> Evals are real time and support both developer and QA.

> Frictionless integration to existing apps and new ones.
