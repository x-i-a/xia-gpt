# General AI Realization Approach
## Basic Conception
1. All activities are nothing but state-to-state transformations.
2. **Adequate context** and **strong inferential capabilities** ensure [almost](https://en.wikipedia.org/wiki/G%C3%B6del%27s_incompleteness_theorems) all state-to-state transformations.

## Strong Inferential Capabilities
When we fix context, the challenge then becomes possessing sufficient inferential capabilities. For example, as of today, the ranking is: Human > GPT-4 > GPT-3.5.

We just need a mechanism to escalate the task when the current inferential capacity is not enough. There are two main reasons:
* Context length is too large
* Cannot generate expected target state

## Adequate context
When we fix inferential capability, the challenge then becomes providing 'exact' context.
* Too much context might lead to memory issue. It is even true for human.
* Too less context increase the inferential difficulty. For example, by using the 5 Axioms of Euclidean geometry as context, all theorems of this axiomatic system could be proved but some of them are really complex.

## Reasoning Path
A reasoning path will translate a state-to-state problem into a lot of smaller state-to-state sub-problems. 
Each sub-problem is easier to resolve.

Two components are developed:
* `xia-composer` for following reasoning paths
* `xia-prompts` for generating reasoning paths (under development)

Many domains, especially software development, have explicit reasoning paths. Tasks of these domains could be executed without the help of `xia-prompts` 
