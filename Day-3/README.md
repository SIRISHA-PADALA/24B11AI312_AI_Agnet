Day 3: LangChain LCEL, Evaluation Harness and Agent Foundations

Project Title

StudyMate AI – Smart Study Planner

1. Project Overview

StudyMate AI is an AI-powered study assistant designed to help students organize their learning activities, create personalized study plans, understand subjects, manage time, revise important topics, and track their learning progress.

On Day 3, we enhanced StudyMate AI using LangChain Expression Language (LCEL), conversation memory, an evaluation harness, and basic agent foundations.

2. Objectives

- Integrate LangChain with the Groq LLM.
- Build an LCEL chain for handling student queries.
- Maintain conversation history to remember previous interactions.
- Create a CSV-based evaluation harness.
- Test AI responses using predefined test cases and keywords.
- Explore LangChain agent creation and invocation.

3. Technologies Used

- Python
- Google Colab
- LangChain
- LangChain-Groq
- Groq API
- GPT-OSS-120B
- CSV

4. Implementation

4.1 LangChain and Groq Integration

Installed the required LangChain packages and connected the Groq API using the "ChatGroq" model.

4.2 System Prompt Configuration

Created a StudyMate AI system prompt that defines the assistant's responsibilities, including:

- Creating personalized study plans.
- Explaining difficult subjects.
- Managing study time.
- Suggesting revision strategies.
- Providing motivation and study guidance.

4.3 LangChain Expression Language (LCEL)

Implemented an LCEL chain using:

- "ChatPromptTemplate"
- "MessagesPlaceholder"
- "ChatGroq"
- "StrOutputParser"

Connected these components using the LCEL pipe operator to process student questions and generate responses.

4.4 Conversation Memory

Implemented conversation history to maintain context between interactions.

The assistant can remember previously shared information, such as the student's name and subjects, and use it when answering follow-up questions.

4.5 Evaluation Harness

Created a CSV file named "studymate_test.csv" containing sample test cases and expected keywords.

Developed an evaluation process that:

- Reads test cases from the CSV file.
- Sends questions to the AI assistant.
- Checks whether expected keywords appear in responses.
- Calculates the overall pass percentage.

This helps perform basic testing of the assistant's responses.

4.6 Agent Foundations

Explored LangChain agent creation using "create_agent()".

Created and invoked a basic StudyMate AI agent with the configured language model and system prompt.

Tested the agent by requesting a three-hour study plan for Python and Data Structures.

5. Final Outcome

Successfully implemented the following Day-3 components:

- Groq LLM integration with LangChain.
- LCEL-based question-answering chain.
- Conversation history and memory.
- CSV-based evaluation harness.
- Basic LangChain agent creation and invocation.
- Generated a personalized three-hour study plan.

6. Conclusion

Day 3 helped strengthen StudyMate AI by introducing LangChain LCEL, conversation memory, response evaluation, and agent foundations. These concepts provide a foundation for developing a more intelligent and personalized study assistant.

Project: StudyMate AI – Smart Study Planner
Day: 3
