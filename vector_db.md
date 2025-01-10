Someone may be familiar with my experience from last week: I was working on a RAG project and got stuck indexing the vectors on Milvus.

It reads trivial, but it is step one, and if it does not work, you will not progress further. What do you do? I went back to reading more about organizing vector indexing in popular db databases. 

This blog (https://thedataquarry.com/posts/vector-db-3/) by Prashanth Rao   and the rest of the series helped me think about the data structure, understand it, and determine the type of compression level that could be applied to the use case I was working on. Note: it is material from late 2023; Something may have changed within the providers, but the overall framework in the blog is still valid and rock solid. 

I found this blog (and the rest of the series) very insightful. 

Some additional information about indexing in vector db

https://cloud.google.com/bigquery/docs/vector-index

https://docs.llamaindex.ai/en/stable/understanding/indexing/indexing/
