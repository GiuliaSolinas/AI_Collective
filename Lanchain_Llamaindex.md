# LangChain and other existing frameworks to organize LLM workflow.

There are multiple frameworks helpful to organize the workflow for NLP-LLM-based development. 

**Introduction**

Solutions for prototyping with no-code design: *LangFlow*. It chains prompts and organizes a basic workflow. It is not suitable for deployment. It can run locally, too. 

Code-based frameworks: 
- *LangChain*: Build abstractions about the workflow, create memory pipeline for long-term context interactions, prompt templates, chains, indexes, reasoning agents for dynamic workflows. 
- *LangGraph*: to manage multi-agents in a structured workflow. It is based on three core components: states, nodes, edges (they can make decisions on which notes to take notes and they can go back and forth). 
- *LangSmith*: for LLM experiment tracking and deployment. It is designed to understand token costs and number of calls. LangFuse is an alternative open-source solution.

This YouTube [video](https://youtu.be/ldBsvhjEREc?si=z9V3s99bRcqQ3CJi) summarizes the frameworks listed above neatly.

Key takeaways: 
- Define the prototyping requirements and the timing needed to see first results.
- Sketch the architecture to design the system's components. Ask yourself strategic questions, such as "how complex should the system be?" or "Should the system only retrieve information on spot or based on long-term queries?" 
- Track the experiments to understand costs and efficiency of the system. 

**LangChain and LlamaIndex**

These are two popular open-source frameworks that can be use used for developing RAG use cases. LlamaIndex is mainly targeting use cases that require fast and precise information retrieval. LangChain supports multi-modal and multi-agent solutions for complex queries and interactions. 

Resources

- Comparison between LangChain and LlamaIndex (from Datacamp blog): https://www.datacamp.com/blog/langchain-vs-llamaindex
- Summary of the two frameworks with the two (from Medium blog): https://medium.com/@tam.tamanna18/langchain-vs-llamaindex-a-comprehensive-comparison-for-retrieval-augmented-generation-rag-0adc119363fe

Both blogs concludes that the choice between one framework over the other one depends on the use case specifics. In general, users can follow the following recommendation:

- Choose LlamaIndex if your primary need is data retrieval and search capabilities for applications that handle large volumes of data that require quick access.
- Choose LangChain if you need a flexible framework to support complex workflows where intricate interaction and context retention are highly prioritized.

Note for myself: I find it interesting the option of organizing the documents' hierarchical structure with LlamaIndex with composed retrievers and nodes. Nodes structure enables the organization of indexed data into trees with tree indexes. 

One example

```
from llama_index import GPTTreeIndex

# Create an index
index = GPTTreeIndex(documents)
query_engine = index.as_query_engine()

```

