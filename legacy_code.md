Damir shared this insightful blog in our CROZ-AI chat: https://martinfowler.com/articles/legacy-modernization-gen-ai.html.
 
It is the story of how Thoughtworks approaches modernizing legacy code with GenAI. They portray a fascinating approach to querying and reasoning about the code to modernize--what Kruno pointed out as a limited feature in the offerings we have been monitoring. 
 
What I liked in this blog is the following:
 
They start with a custom-first approach and consider what could make modernization expensive. They also offer a critical perspective and highlight areas where GenAI does not make sense because mature tools can still be more performant than a large language model in their tasks. 
The GenAI framework in the blog goes beyond translating an old COBOL chuck into the natural language. It offers a way to map customers' source code and its abstract syntax into a knowledge graph that links classes with methods and attributes. This "knowledge pipeline" then gets ingested into the "comprehension pipeline," which enriches the graphs with contextual (parsed) knowledge, tech stack, and customer heuristics. The outcome is an enriched knowledge graph that can be queried with an LLM. This offers a base for stakeholders (developers, business analysts, or product owners if necessary) to query the code, understand its purpose, understand how the modules combine in the monolithic application, etc. 
In their experience, GenAI can bring value to low-level requirements (e.g., extracting business rules and abstracting flowcharts). We also saw this with the WX code assistant and the solutions from the two start-ups. Kruno is quite skeptical about the value of this feature. I understand his points, especially in the case of single developers. However, GenAI may bring value when those low-level requirements must be performed at scale with thousands of lines of code and in tight time. It is my assumption. 
They are pretty open to being cautious about GenAI's value for more high-level abstract tasks. I think this is a fair point because it is an area with still a lot of research and experimentation but a consolidated method that could be brought into a stable product. They are working on this issue and point to GraphRAG from Microsoft (this project is gaining much interest in the LLM circles). I do not think it is the ultimate solution, and there are complementary fields, such as research on the chain of thoughts, multi-agentic models, and extension of context understanding. 
Overall, there are many points we can bring to the PoV discussion. We could even provide a quick snapshot of our code-modernization radar. 

New version for social media

---

🚀 **Legacy Code Modernization with GenAI!** 🚀

These days, I have the honor of working on a project I love: COBOL code modernization with genAI. I have been researching genAI solutions for COBOL code modernization. There are some challenges when working with COBOL. It is a legacy code with unique traits such as its verbose syntax, complex data structures, and reliance on specific hardware and operating systems, where AI code assistants may fall short if not fine-tuned properly. Even so, each enterprise environment may have developed its way of coding in COBOL, making it difficult for code-generation LLMs to drive suitable output. I found this blog about Thoughtworks' approach to modernizing legacy code using GenAI very insightful and close to what I learned in the field. Here's what stood out to me

1. Custom-First Approach: They emphasize starting with a custom-first approach, considering what could make modernization expensive. This critical perspective is refreshing, especially when they highlight areas where GenAI might not best fit, as mature tools can sometimes outperform large language models.

2. Innovative GenAI Framework: The blog goes beyond simple code translation. It describes a sophisticated process where customers' source code and its abstract syntax are mapped into a knowledge graph. This graph links classes with methods and attributes, creating a "knowledge pipeline" that feeds into a "comprehension pipeline." The result? An enriched knowledge graph can be queried with an LLM, helping stakeholders understand the code's purpose and how modules interact within a monolithic application.

3. Value in Low-Level Requirements: They demonstrate how GenAI can add value to low-level requirements, such as extracting business rules and abstracting flowcharts. While this is still a low-level task, GenAI can speed up developers when it needs to be performed across thousands of lines of code under tight deadlines. This is possibly the low-hanging fruit of COBOL code modernization and code explanation. 

4. Cautious Optimism for High-Level Tasks: They are open about GenAI's current limitations for high-level abstract tasks, acknowledging that this area is a work in progress and still requires much research and experimentation. However, they are actively working on solutions like GraphRAG from Microsoft, which is gaining interest in LLM circles. While not the ultimate solution, it complements ongoing research in areas like chain of thoughts, multi-agent models, and extended context understanding, giving us hope for future advancements.

COBOL developers and AI specialists, what is out there for legacy code?  

