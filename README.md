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

## Installation
1. Clone the repository:
```bash
git clone https://github.com/atuli93/rasa-chatbot.git
cd rasa-chatbot
```

2. Create and activate a virtual environment:
```bash
python3 -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

# Training the Bot

## Train the Rasa model with:
```bash
rasa train
```
- Models are stored locally in models/ and are not pushed to GitHub.


# Running the Bot

## Start the Rasa shell:
```bash
rasa shell
```
**For testing with a local action server:**
```bash
rasa run actions
```


# Folder Structure

rasa-chatbot/
├── data/               # Training data (NLU & stories)
├── actions/            # Custom actions
├── models/             # Trained models (not tracked in Git)
├── config.yml          # Pipeline and policies configuration
├── domain.yml          # Intents, entities, slots, responses
├── README.md           # Project documentation
├── .gitignore          # Ignore cache, virtualenv, models



# Contribution

**Contributions are welcome!**
**Please submit a pull request or open an issue for suggestions or bugs.**

# License

**This project is licensed under the MIT License.**

