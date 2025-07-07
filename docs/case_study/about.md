# Case Study

## App 

This is a case study using a Deep Research clone app by Kody Simpson.

The repo is [https://github.com/Python-Test-Engineer/llm-evaluation-framework](https://github.com/Python-Test-Engineer/llm-evaluation-framework)

Located in src/deep_research it uses the OpenAI Agent SDK.

It enables us to use an actual app to set up Evals.

`uv run ./src/deep_research/main.py`

## First steps

- What does a satisified user look like?
- What would a disappointed user look like?
- How do we define a successful app from our point of view?

We need to make each agent self-evaluating. That is, we need to export to CSV input|output|context|tool_use|metadata.

Then we can add references if we have them and run our evals.

We will do this manually to get a sense of what we need to implement and if possible scale up with automations and LLM as judge.