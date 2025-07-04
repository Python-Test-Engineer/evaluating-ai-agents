# Evaluating AI Agents

## Aim

This is a manual to establish EvalOps - a way of testing and evaluating Agentic systems.

## Agentic Evaluations

We can see an Agentic workflow:

![Agentic Evaluation](./images/agentic-rag-langchain.png)

A Unit Test in agentic terms is the smallest block of code that uses an llm to determine the ROUTE and the RESPONSE.

It may contain other deterministic functionality which we can test in the usual way, but this manual focusses on testing and monitoring Agentic systems.


## Patterns

### Routing

One fundamental pattern is ROUTING - does the Agent select the correct tool/function/skill with the correct inputs?

![Agentic Evaluation](./images/evaluating-ai-agents-1.png)

There is also NEXT - does the Agent select the correct next step where this is applicable?

![Agentic Evaluation](./images/evaluating-ai-agents-4.png)

### Output

For a given input, we will obtain an output. 

We may retrieve additonal context to support the generation of the output.

We will also have REFERENCES - ground truths.

We will have a matrix (context may or not exist):

INPUT - OUTPUT - CONTEXT - REFERENCE

We can then work out an evaluation.

We look for OMISSIONS - ADDITIONS - CONTRADICTIONS - COMPLETENESS as alternatives to traditonal F1 scores although these can be computed as well.

![Agentic Evaluation](./images/evaluating-ai-agents-2.png)

## Datasets

Our goal is to get a number of datasets:

INPUT - OUTPUT - CONTEXT - REFERENCE

TOOL_CALLED - ARGUMENTS - NEXT - EXPECTED

Oncce we have these there are many libraries or our own custom evaluations that we can use.

## Friction

The process needs to be frictionless for developers.

At an accessability talk, the speaker said 'How do you make a blueberry muffin?'. 

You put the blueberries in at the beginning and not stuff them in at the end.

This has been a priority in developing this Agentic Testing Framework.

