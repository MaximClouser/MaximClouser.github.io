---
title: "RepoRover"
excerpt: "An LLM chatbot to help developers understand and explore GitHub repositories using 
language models. <br/><img src='/images/RepoRover.png' width='350px'>"
collection: portfolio
---
*Started during the Llama Hackathon, Spring 2024*  

### Overview  
Built using LangChain, OpenAi, and Streamlit, this tool assists developers in understanding GitHub repositories by exploring their file structure, readme files, and raw code with the help of LLMs. This project was motivated by the
challenges faced at a previous hackathon, where hackers found it difficult to quickly understand large and messy
repos before contributing to collect a bounty. Therefore, we decided to build the RepoRover which parses
a given repo and utilizes Retrieval-Augmented Generation (RAG) and LLMs to provide developers with information such as repo structure or which files they should consider for their specific contribution.

The RepoRover uses the GPT-3.5 Turbo model from OpenAI and implements RAG with the help of the LangChain framework and FAISS vector store, allowing the Rover to explore massive repositories while remaining within the context window and providing relevant information to users. This is acheived via a similarity search on a vector store of the repo contents against the user query, followed by a second LLM which can request code from specific files and provide short summaries. Finally, all of this information is passed to the Rover LLM which now has the most relevant information of the entire Repo and the user query.

### Live App and Code 
[Try the RepoRover.](https://reporover.streamlit.app/)  
[View the full project code on GitHub.](https://github.com/DevTechCollective/RepoRover)
