# Day 1 – LLM Connection and API Testing





### 1. Installing and Importing LangChain Groq
- Installed the `langchain_groq` package.
- Imported `ChatGroq` to connect with Groq-hosted language models.

### 2. LLM Connection
- Connected to the Groq API using an API key.
- Stored and accessed the API key securely through Google Colab Secrets.
- Initialized the LLM using the `ChatGroq` class.
- Used the `openai/gpt-oss-120b` model with temperature set to 0.

### 3. System Prompt Implementation
- Created a system prompt for a Sweet Crumbs Home Bakery assistant.
- Defined the assistant's responsibilities and response rules.
- Set instructions to provide polite and short responses.
- Added business rules such as 24-hour advance notice for orders and eggless cake availability.

### 4. LLM Interaction and Testing
- Created an `ask()` function to send user questions to the LLM.
- Used `llm.invoke()` to generate responses.
- Tested the assistant with a customer question about receiving an order the next day.
- Observed how the LLM follows the instructions provided in the system prompt.

### 5. Prompt Guard Testing
- Imported the Groq client.
- Tested the `meta-llama/llama-prompt-guard-2-22m` model.
- Explored prompt injection detection using an instruction designed to override previous instructions.

## Learning Outcomes
- Understood how to connect an LLM using an API.
- Learned how to use LangChain with Groq.
- Practiced securely accessing API keys through Colab Secrets.
- Understood system prompts and their role in controlling LLM responses.
- Learned basic LLM interaction and testing.
- Explored prompt injection detection using Prompt Guard.

## Technologies Used
- Python
- Google Colab
- LangChain
- Groq API
- ChatGroq
- LLM (GPT-OSS-120B)
- Groq Prompt Guard

## Task Notebook
`agenticAI_Day1_task_1.ipynb`
