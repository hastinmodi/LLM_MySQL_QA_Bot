# LLM_MySQL_QA_Bot

The objective of this project is to enable natural language interactions with a MySQL database. Users pose questions in everyday language, and our system responds by translating those queries into SQL statements, subsequently executing them on the MySQL database. AtliQ Tees, a T-shirt store, serves as our practical application scenario, managing inventory, sales, and discount information within the MySQL database. ([Reference](https://github.com/codebasics/langchain/tree/main/4_sqldb_tshirts))

## Installation

1.Clone this repository to your local machine using:

```bash
  git clone https://github.com/hastinmodi/LLM_MySQL_QA_Bot.git
```
2.Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
3.Acquire an api key through makersuite.google.com and put it in .env file:

```bash
  GOOGLE_API_KEY="your_api_key_here"
```
4.For database setup, run db_creation_atliq_t_shirts.sql in your MySQL workbench.

## Usage

1.Run the Streamlit app by executing:
```bash
streamlit run main.py
```

2.The web app will open in your browser where you can ask questions.

## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- langchain_helper.py: This has all the langchain code.
- .env: Configuration file for storing your Google API key.
- few_shots.py: Contains few shot prompts.
- db_creation_atliq_t_shirts.sql: SQL file containing the database creation script.