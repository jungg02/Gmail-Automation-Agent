# Gmail Automation Agent
Automate Gmail tasks using CrewAI, a powerful multi-agent framework for orchestrating LLM-driven workflows.
This project enables seamless interaction with Gmail — such as reading, classifying, summarizing, and managing emails — powered by large language models and crewai_tools.

## Set Up Instructions
1) Clone the repository 
```bash
git clone https://github.com/jungg02/Gmail-Automation-Agent.git
cd Gmail-Automation-Agent
```

2) Create and Activate Virtual Environment
```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```
3) Install Dependencies
```bash
pip install uv
uv tool install crewai
crewai install # when running for the first time
```


## Features
- **📋Email Categorization**: Automatically categorizes emails into specific types (newsletters, promotions, personal, etc.)
- **🔔Priority Assignment**: Assigns priority levels (HIGH, MEDIUM, LOW) based on content and sender with strict classification rules
- **🏷️Smart Organization**: Applies Gmail labels and stars based on categories and priorities
- **💬Automated Responses**: Generates draft responses for important emails that need replies
- **🧹Intelligent Cleanup**: Safely deletes low-priority emails based on age and category
- **🗑️ Trash Management**: Automatically empties trash to free up storage space

## Usage

Run the application with:

```bash
crewai run
```

You'll be prompted to enter the number of emails to process (default is 5).

The application will:
1. 📥 Fetch your unread emails
2. 🔎 Categorize them by type and priority
3. ⭐ Apply appropriate labels and stars
4. ✏️ Generate draft responses for important emails
5. 🗑️ Clean up low-priority emails based on age
6. 🧹 Empty the trash to free up storage space


## 🌟 Special Features

- **📅 Smart Deletion Rules**: 
  - Promotions older than 2 days are automatically deleted
  - Newsletters older than 7 days (unless HIGH priority) are deleted
  - Receipts and important documents are archived instead of deleted

- **✍️ Smart Response Generation**: Responses are tailored to the email context and include proper formatting

- **💡 Creative Slack Notifications**: Fun, attention-grabbing notifications for important emails

- **🧵 Thread Handling**: Properly tracks and manages email threads to maintain conversation context


## Acknowledgement
This project was completed with reference to 

