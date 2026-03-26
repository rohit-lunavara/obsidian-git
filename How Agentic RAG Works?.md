---
tags:
  - fleeting
---
# References

> [!QUOTE] Original Capture
> Typical retrieval pipeline - one query and one retrieval, however there are several issues with this approach
> 	1. Ambiguous queries - Cant clarify or rewrite
> 	2. Scattered evidence - No concept of checking multiple pools of chunks
> 	3. False confidence - No mechanism to tell diff between relevant and actually correct
> 
> The system does not reflect what it retrieved
> 
> Agentic RAG has these capabilities - 
> 	1. Tool use and routing - Can search multiple places, multiple times
> 	2. Query refinement - Can rewrite ambiguous query if initial search returns weak results
> 	3. Self evaluation - Can examine the results and take different actions to remediate the issue
> 	   
> Trade-offs - 
> 	1. Latency - Standard RAG query (1-2s) vs Agentic RAG loop w/ 3-4 loops (10s+)
> 	2. Cost - Can multiply to 3-10x compared to standard RAG
> 	3. Debugging and predictability - Standard RAG is relatively deterministic vs Agentic RAG which introduces variability at each step
> 	4. Self-evaluator paradox - System can self-correct only if LLM is good at judging relevance - We're letting on LLM call judge another
> 	5. Overcorrection - Sometimes the agent will discard useful info to find something better, even if it doesnt exist
> 
> Direct factual lookups against a clean and single-source knowledge base don’t need a reasoning loop
> Neither do high-volume, low-complexity query patterns where latency and cost matter more than handling edge cases
> If most of the failures in an existing RAG system come from retrieval quality issues like bad chunking or stale data, fixing those will do more good than adding an agentic layer

https://blog.bytebytego.com/p/how-agentic-rag-works?utm_source=tldrdev