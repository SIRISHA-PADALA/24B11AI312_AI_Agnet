# Day 2 – StudyMate AI: Smart Study Planner

## 1. Project Overview

StudyMate AI is an AI-powered study planning assistant designed to help students organize their study schedules, manage time effectively, understand difficult subjects, and achieve their academic goals.

It uses a Large Language Model (LLM) through the Groq API to provide personalized study guidance and interactive conversations.

## 2. Objectives

- Build an AI-powered study assistant.
- Understand and classify student queries.
- Extract important student information.
- Maintain conversation history using memory.
- Generate personalized study guidance.
- Create an interactive chat interface.

## 3. Technologies Used

- Python
- Google Colab
- Groq API
- OpenAI Python SDK
- GPT-OSS-120B Model
- IPyWidgets

## 4. Key Concepts Implemented

### 4.1 LLM Connection
Connected the Groq API using the OpenAI client to communicate with the language model.

### 4.2 Student Information
Created a `STUDY_INFO` dictionary to store student details, subjects, available study hours, weak topics, and learning goals.

### 4.3 System Prompt
Defined the role, responsibilities, and instructions of StudyMate AI.

### 4.4 Intent Classification
Implemented `classify_intent()` to identify the purpose of student queries, such as:
- Study planning
- Subject guidance
- Time management
- Revision
- Progress tracking
- Motivation

### 4.5 Information Extraction
Implemented `extract_student_info()` to extract important details such as student name, subjects, exam date, daily study hours, weak topics, and priorities.

### 4.6 Execution Logging
Used a decorator to measure and display the execution time of functions.

### 4.7 AI Agent
Created a `StudyMateAgent` class to manage conversations, classify user queries, generate responses, and maintain conversation history.

### 4.8 Conversation Memory
Tested the agent's ability to remember previously provided student information.

### 4.9 Interactive Chat Interface
Created an interactive chat interface using IPyWidgets with a text input, send button, and output area.

## 5. Final Outcome

Successfully developed a StudyMate AI prototype that can:
- Understand student queries.
- Identify the intent behind questions.
- Extract student information.
- Remember previous conversations.
- Provide personalized study plans and academic guidance.
- Interact with students through a chat interface.

## 6. Conclusion

Day 2 focused on building the core intelligence of StudyMate AI by implementing LLM integration, intent classification, information extraction, conversation memory, and an interactive chat interface.

The completed prototype provides a foundation for developing a smarter and more personalized AI study assistant.
