# 📬 Gmail Automation Agent
This project automates various Gmail management tasks, saving countless hours and freeing up storage space. Additional functionalities useful for students such as special handling of emails regarding internships/job opportunities or bank transactions have also been included.

Powered by CrewAI, a powerful multi-agent framework for orchestrating LLM-driven workflows, it enables seamless interaction with Gmail — such as reading, classifying, drafting, and managing emails.

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

You'll be prompted to enter the number of emails to process. (Up to user to select, with default being 5)

The application will:
1. 📥 Fetch your unread emails
2. 🔎 Categorize them by type and priority
3. ⭐ Apply appropriate labels and stars
4. ✏️ Generate draft responses for important emails
5. 🗑️ Clean up low-priority emails based on age
6. 🧹 Empty the trash to free up storage space


## Special Features

- **📅 Smart Deletion Rules**: 
  - Promotions or newsletters older than 7 days are automatically deleted
  - Receipts and important documents are archived instead of deleted

- **✍️ Smart Response Generation**: Responses are tailored to the email context and include proper formatting

- **Special Handling of Important Emails**: Specific treatment for certain emails (internship offers, bank transaction statements, travel bookings etc.) that would likely be useful to a student.

## Acknowledgement
This project was completed with reference to https://www.youtube.com/watch?v=zz0SA8xMBCo from The How-To Guy on Youtube. 

