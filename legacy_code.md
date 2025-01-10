 # Legacy code modernization

It mainly relate to three areas:
- re-platform
- understand
- refactor

 
**Legacy Code Modernization with GenAI!**
 
Original resource: https://martinfowler.com/articles/legacy-modernization-gen-ai.html.
 
It is the story of how Thoughtworks approaches modernizing legacy code with GenAI. They portray a fascinating approach to querying and reasoning about the code to modernize. 
 
What I liked in this blog is the following:
 
They start with a custom-first approach and consider what could make modernization expensive. They also offer a critical perspective and highlight areas where GenAI does not make sense because mature tools can still be more performant than a large language model in their tasks. 

The GenAI framework in the blog goes beyond translating an old COBOL chuck into the natural language. It offers a way to map customers' source code and its abstract syntax into a knowledge graph that links classes with methods and attributes. This "knowledge pipeline" then gets ingested into the "comprehension pipeline," which enriches the graphs with contextual (parsed) knowledge, tech stack, and customer heuristics. The outcome is an enriched knowledge graph that can be queried with an LLM. This offers a base for stakeholders (developers, business analysts, or product owners if necessary) to query the code, understand its purpose, understand how the modules combine in the monolithic application, etc. 

In their experience, GenAI can bring value to low-level requirements (e.g., extracting business rules and abstracting flowcharts). We also saw this with the WX code assistant and the solutions from the two start-ups. Some can be quite skeptical about the value of this feature. I understand the points, especially in the case of single developers. However, GenAI may bring value when those low-level requirements must be performed at scale with thousands of lines of code and in tight time. It is my assumption. 

They are pretty open to being cautious about GenAI's value for more high-level abstract tasks. I think this is a fair point because it is an area with still a lot of research and experimentation but a consolidated method that could be brought into a stable product. They are working on this issue and point to GraphRAG from Microsoft (this project is gaining much interest in the LLM circles). I do not think it is the ultimate solution, and there are complementary fields, such as research on the chain of thoughts, multi-agentic models, and extension of context understanding. 

**Other resources from Thoughtworks**

Link to the podcast with Erik Doernenburg: https://www.thoughtworks.com/insights/podcasts/pragmatism-in-practice/leveraging-AI-for-legacy-modernization?utm_source=linkedin&utm_medium=social-organic&utm_campaign=tech-to-know-vol-11-perspectives-edition_2024-11&utm_content=body-copy
 
Some points that stood out from the podcast: 
- They start with reverse engineering tools to parse large chunks of code and go through the first "understanding phase." They will save this information into a database (knowledge graph) and then use it in the query for the LLM.
- RAG is always an excellent strategy to give information about the client's specific "dialect" of COBOL. Fine-tuning may not be necessary. 
- LLM is helpful, for example, in summarizing an extensive source of information or checking for inconsistencies in code documentation across time. There is (and should not be) a single tool where you inject old COBOL and get new COBOL because there is context to understand. Plus, the developers need to undergo an iterative modernization process using multiple tools and do iterative test checking. 
- The podcast is a bit shallow on modernization for clients with on-prem requirements. It points to smaller LLMs that could run on-prem, but it seems it is still experimental for everyone as for end of 2024. 

