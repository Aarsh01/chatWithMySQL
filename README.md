# MySQL Python Chatbot Mistral AI
Chatbots and natural language interfaces are becoming increasingly important in modern applications. By integrating these capabilities with database access, we can create powerful tools that allow users to interact with data in a more intuitive and conversational way.
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

Create your own .env file with the necessary variables:

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
2. Build the Chain:
   ![mysql-chains](https://github.com/Aarsh01/chatWithMySQL/assets/95579399/89ff0962-9c5f-4668-bed4-216ac3f715c3)

   a. Firstly to connect database and use the Langchain required pachages and build the chain(provided in the .png), I have shown the steps one by one in .ipynb file. -- can't able to use openai-api-key due to personal problem/error.
   b. Afterwards, Using the streamlit, I build the Python GUI App, following the same steps. -- Problem solved while using the langchain_groq package.

3. I used the LangChain wrapper of "sqlalchemy" to interact with the database. I also used the langchain package to create a custom chain that allowed me to chat with the database using natural language.






