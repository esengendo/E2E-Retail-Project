# IntelliQuery: End-to-End Text-to-SQL Conversion and Database Querying Application using Few Shot Prompting with Google Palm, LangChain, MySQL, and Streamlit

## Overview

This application showcases the integration of Few Shot Prompting using Google Palm, LangChain, MySQL, and Streamlit to enable natural language interactions with a Large Language Model (LLM) for generating and executing SQL queries. The application is particularly adept at extracting data from a backend SQL database using the "Retrieval Augmented Generation" (RAG) approach.

## Objective: 

I developed a seamless integration tool combining Google Palm and LangChain with my custom-built MySQL database for the Threadz E-Store, and Streamlit. This application is designed to enable intuitive and efficient data extraction using Few Shot Prompting. It focuses on streamlining both data querying and extraction processes, thereby enhancing the efficiency and intuitiveness of SQL database handling. This tool empowers users with streamlined access to essential data insights, simplifying the retrieval of critical data from SQL Databases.

## Features

- **Streamlit Web Interface**: User-friendly web interface for querying.
- **Natural Language Query Processing**: Google Palm facilitates natural language interactions.
- **Dynamic SQL Query Generation and Execution**: Automatically generate and execute SQL queries from user inputs.
- **MySQL Database Integration**: Connects to the Threadz T-Shirts database.
- **LangChain and Google Palm Integration**: Manages communication between the LLM, database, and the user.

## System Requirements

- Python 3.8 or later.
- MySQL Server (version 5.7 or later).
- Google Palm API access.
- Streamlit.
- LangChain and additional Python dependencies.

## Installation

1. **Clone the Repository**:
   ```
   git clone [repository URL]
   cd [repository directory]
   ```

2. **Install Dependencies**:
   ```
   pip install -r requirements.txt
   ```

3. **Database Setup**:
   my local MySQL Server has to be operational with the Threadz database.

4. **API Keys and Configuration**: 
   Set up your Google Palm API key in the environment variables.

## Usage

1. **Start the Streamlit App**:
   ```
   streamlit run app.py
   ```

2. **Interact via the Web Interface**:
   Use the Streamlit interface to submit queries and view responses.

## Main.py File Overview

The `main.py` file is the core of the application. It sets up the necessary components for interacting with the LLM and the MySQL database:

- **LangChain and GooglePalm Integration**: Sets up the LLM and configures it with Google Palm's API key.
- **Database Connection**: Establishes a connection to the MySQL database.
- **Embeddings and Vector Stores**: Utilizes HuggingFace embeddings and Chroma vector stores for processing and selecting examples.
- **Example Selector**: Sets up the SemanticSimilarityExampleSelector for choosing relevant examples.
- **Prompt Templates**: Defines the format for SQL queries and responses.
- **SQLDatabaseChain**: Integrates all components to create a chain that processes input questions, generates SQL queries, executes them, and returns answers.

The `main.py` file also includes a test run example, demonstrating how to use the chain to process a sample query.

## Additional References

For a deeper understanding of the concepts and integrations used in this application, refer to the following resources:

- [Few-Shot Prompting with CodeLlama, LangChain, and MySQL](https://medium.com/@yernenip/few-shot-prompting-with-codellama-langchain-and-mysql-94020ee16a08)
- [LangChain SQL Database Toolkit Documentation](https://python.langchain.com/docs/integrations/toolkits/sql_database)


## Contributions

I encourage contributions to this project. Feel free to submit pull requests or report issues on my GitHub repository.


## Contact

For support or inquiries, please contact [].

---
