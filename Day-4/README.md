# StudyMate AI – Smart Study Planner
## Day 4: Building a Tool-Enabled AI Agent

### 1. Project Overview

StudyMate AI is an intelligent study assistant designed to help students organize their learning activities, manage study time, receive subject guidance, and track academic progress.

In Day 4, we upgraded the StudyMate AI assistant by integrating custom tools with an LLM-powered agent. The agent can understand student requests and select appropriate tools to perform study-related tasks.

### 2. Objectives

- Build an AI agent using LangChain and Groq.
- Provide subject-specific learning guidance.
- Generate study plans based on available study hours.
- Track student learning progress.
- Store study records in Google Sheets.
- Maintain conversation history during interaction.

### 3. Technologies Used

- **Python:** Main programming language.
- **Google Colab:** Development environment.
- **Groq API:** Provides access to the Large Language Model.
- **LangChain:** Agent creation and tool integration.
- **Pydantic:** Data validation.
- **Google Sheets:** Stores student study progress.

### 4. Implementation

**Step 1: API and Google Sheets Connection**

- Installed the required Python packages.
- Connected the Groq LLM using the API key.
- Authenticated the Google account.
- Created a Google Sheet named `StudyMate AI Progress`.
- Prepared columns for student name, subject, topic, study hours, and status.

**Step 2: Data Model and Subject Guidance**

Created a Pydantic model named `StudyProgress` to validate student study information.

Supported subjects:
- Python
- Data Structures
- Machine Learning
- Mathematics

Defined subject-wise topics and learning advice using a Python dictionary.

**Step 3: Custom Tool Creation**

Developed three custom tools:

1. `get_subject_guidance()` – Provides subject descriptions, important topics, and learning suggestions.
2. `create_study_plan()` – Creates a study plan based on subjects, available hours, and weak topics.
3. `log_study_progress()` – Validates study information and saves progress to Google Sheets.

**Step 4: Agent Creation**

- Created an AI agent using LangChain's `create_agent()`.
- Connected the Groq LLM with all three custom tools.
- Defined a system prompt describing the responsibilities of StudyMate AI.
- Implemented conversation history.
- Created a chat function to interact with the agent.

### 5. Workflow

Student Input → StudyMate AI Agent → Understand Request → Select Appropriate Tool → Execute Tool → Generate Response

For progress tracking, the workflow continues with:

Validate Student Data → Save Record to Google Sheets → Confirm Result

### 6. Sample Execution

**Test 1: Study Plan Generation**

Input:
"I have 3 hours today. Create a study plan for Python and Data Structures. My weak topics are loops and recursion."

Output:
The agent generated a three-hour study timetable containing Python practice, Data Structures, recursion, breaks, and revision.

**Test 2: Study Progress Tracking**

Input:
"I studied Python loops for 1 hour. My status is completed. Save my progress under the student name Sirisha."

Output:
"Your 1-hour session on Python loops has been logged successfully."

The agent reported successful logging. Google Sheets verification is required to confirm the record was actually stored.

### 7. Key Learnings

- Understanding tool-enabled AI agents.
- Creating custom tools using LangChain.
- Connecting an LLM with external tools.
- Validating structured data using Pydantic.
- Integrating Google Sheets with Python.
- Maintaining conversation history.
- Understanding how an AI agent selects tools based on user requests.

### 8. Conclusion

Day 4 successfully upgraded StudyMate AI from a basic conversational assistant into a tool-enabled AI agent.

The system can generate study plans, provide subject guidance, and record student learning progress using Google Sheets. This provides a foundation for developing a more personalized and intelligent study planning system.

### 9. Future Enhancements

- Generate more personalized study timetables.
- Track daily and weekly learning progress.
- Identify weak subjects automatically.
- Recommend revision schedules.
- Add progress charts and performance reports.
- Develop a user-friendly web interface.
