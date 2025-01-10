# Technical Debt - Mind the Gap!

## Resources

Why your company is struggling to scale up generative AI
https://www.economist.com/business/2024/11/04/why-your-company-is-struggling-to-scale-up-generative-ai
From The Economist 

https://allaboutdata.substack.com/p/making-ai-uncool-again-parte-1-il


Making the impact of technical debt visible: https://open.substack.com/pub/marvelousmlops/p/making-the-impact-of-technical-debt?utm_campaign=post&utm_medium=web (good blog about where the technical debt comes: new projects and interdependencies between existing projects)

Defining, Measuring, and Managing Technical Debt (ref: C. Jaspan and C. Green, "Defining, Measuring, and Managing Technical Debt," in IEEE Software, vol. 40, no. 3, pp. 15-19, May-June 2023, doi: 10.1109/MS.2023.3242137.): https://ieeexplore.ieee.org/document/10109339

Business causes to technical debt (2023): https://arxiv.org/pdf/2104.09330


## Some notes

This week, I read an intriguing article from The Economist about the challenges organizations face with AI projects, particularly their slow adoption or failure to take off. One topic that caught my attention was technical debt (for a great overview, check out Alberto Danese’s blog post). This is a crucial issue that companies often overlook during the initial discovery phase of AI solutions.

From my experience with generative AI Proof of Concepts (PoCs), I’ve learned an important lesson: while it’s beneficial to quickly prototype stand-alone solutions to understand AI’s potential, the PoC must also address two key aspects:

- Current Legacy Infrastructure: How will the AI solution interact with existing systems?
- Integration Solutions: What are the possible ways to integrate the AI project with the current infrastructure?

By considering these factors, we can limit the exponential growth of technical debt. Achieving a completely debt-free solution is rare, especially in complex and sometimes outdated infrastructures. 

