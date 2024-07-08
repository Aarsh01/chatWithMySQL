# MySQL Python Chatbot Mistral AI

## Features
- **Natural Language Processing**: Uses GPT-4 to interpret and respond to user queries in natural language.
- **SQL Query Generation**: Dynamically generates SQL queries based on the user's natural language input.
- **Database Interaction**: Connects to a SQL database to retrieve query results, demonstrating practical database interaction.
- **Streamlit GUI**: Features a user-friendly interface built with Streamlit, making it easy for users of all skill levels.
- **Python-based**: Entirely coded in Python, showcasing best practices in software development with modern technologies.

## Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

Create your own .env file with the necessary variables, including your OpenAI API key:

```bash
OPENAI_API_KEY=[your-openai-api-key]
GROQ_API_KEY=[your-groq-api-key]
```

## Usage
To launch the Streamlit app and interact with the chatbot:

```bash
streamlit run app.py
```

## Procedure
1. First of all, download the "Chinook" database. This is a sample database that represents a digital media store, including tables for artists, albums, media tracks, invoices, and customers. I will use this database to test my chatbot.
#### Creating a Database

Now, go to your terminal and log in to MySQL using the following command:
```bash
mysql -u root -p
```

Explain
You will be prompted to enter your password. Once you are logged in, you can create a new database using the following command:

```bash
CREATE DATABASE chinook;
USE chinook;
SOURCE <LOCATION>; --or the name of your SQL file to load the database
```
