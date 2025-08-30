# Rasa Chatbot

# 🤖 Rasa Chatbot

![Python](https://img.shields.io/badge/python-3.9+-blue)
![Rasa](https://img.shields.io/badge/rasa-3.6.21-orange)
![License](https://img.shields.io/badge/license-MIT-green)

---

## Description
This is a Rasa-based chatbot that can handle [your bot’s purpose, e.g., customer support, FAQs, etc.].  
The bot is trained with intents, entities, and stories defined in the `data/` folder.

## Features
- Intent recognition and entity extraction
- Conversational flow with stories and rules
- Custom actions and responses
- Easy to extend with new intents and stories

## How to Run Your Rasa Chatbot

Follow these steps to set up and run the bot locally:

## Installation
**1. Clone the repository:**
```bash
git clone https://github.com/atuli93/rasa-chatbot.git
cd rasa-chatbot
```

**2. Set up a Python virtual environment.**
```bash
python3 -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
```

**3. Install dependencies:**
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

**4. Train the Rasa model**
```bash
rasa train
```
- Models are stored locally in models/ and are not pushed to GitHub.


**5. Run the Bot**
- Chat in the terminal
```bash
rasa shell
```
- Run the Rasa server
```bash
rasa run
```
- Run custom actions (if any)
```bash
rasa run actions
```
- Test your bot
```bash
rasa test
```

💡 Tip: The models/ folder is ignored in Git. Every time you make changes to training data, run rasa train to generate an updated model.

--- 

# Project Structure
```rasa-chatbot/
├── .gitignore                 # Excludes virtual environments, models, cache, etc. from Git
├── README.md                  # Project overview, setup instructions, usage, etc.
├── config.yml                 # Rasa pipeline and policies configuration
├── domain.yml                 # Bot domain (intents, entities, slots, responses)
├── credentials.yml            # Messaging channel credentials (optional)
├── endpoints.yml              # Server endpoints for Rasa (optional)
├── data/                      # Training data
│   ├── nlu.yml                # NLU examples (intents, entities)
│   ├── stories.yml            # Conversation flows
│   ├── rules.yml              # Rules for bot behavior
│   └── responses.yml          # Optional: pre-defined responses
├── actions/                   # Custom Python actions
│   └── actions.py             # Action code for responses or external API calls
├── models/                    # Trained Rasa models (ignored in Git)
├── logs/                      # Logs generated during bot execution (optional)
├── .venv/                     # Python virtual environment (ignored in Git)
└── tests/                     # Optional test scripts or test data
```

---

# Contribution

**Contributions are welcome!**
**Please submit a pull request or open an issue for suggestions or bugs.**

# License

**This project is licensed under the MIT License.**

