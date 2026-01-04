# RAG AI Agent

This project is based on the https://www.youtube.com/watch?v=AUQJ9eeP-Ls .

What RAG does here?

In this context, RAG enhances the LLM’s responses by incorporating relevant information from a knowledge base, rather than depending only on the model’s pre-trained knowledge.

#### Tech Stack  

1. Python
2. Streamlit- for the frontend
3. Qdrant - as the vector database
4. Inngest- for  orchestration and observability
5. Lllamaindex- to connect the LLM
6. OpenAI- for the AI model 

#### Steps

1. Create a folder in the local machine with a suitable name.
   eg: RAGProductionApp
2. Open the created folder using the VS code.
3. Open the terminal in the VS code and initialize the project as below.

   ` uv init`
uv is a package manager and we can use the above command to initialize the project.

  *Additional*

    What 'uv init' does?
    
    inside a project folder, it:

      * Creates a pyproject.toml file
      → This becomes the main project configuration file.

      * Defines basic project metadata
      → Project name, version, Python requirements (if prompted).

      * Prepares the project for dependency management
      → Allows you to use uv add, uv remove, etc.

      * Makes the project uv-managed
      → uv now controls dependencies and environment setup.

4. Now we should to add the neccessary python packages into the project. It can be done using below command.
   
    `uv add fastapi inngest llama-index-core llama-index-readers-file python-dotenv qdrant-client uvicorn streamlit openai`

5. As we are using an Open AI model we need to create a key in the https://platform.openai.com/
6. Create a .env file in the project and specify the api key in that file.


   
