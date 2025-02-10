This project is an AI-powered auto-reply bot that interacts with chat messages using the OpenAI GPT-3.5-turbo model. The bot is designed to analyze chat history and generate appropriate responses based on predefined roles and contexts.

# Features
- Cursor Position Tracker: A script to continuously track and print the cursor position on the screen. Useful for identifying coordinates for automation tasks. Implemented in 01_get_cursor.py.
- OpenAI Integration: A script to interact with the OpenAI API, sending chat history and receiving AI-generated responses. Implemented in 02_openai.py.
- Automated Chat Interaction: A bot that automates the process of reading chat messages, generating responses using OpenAI, and sending replies. Implemented in 03_bot.py.

# Scripts
### 01_get_cursor.py
This script uses the pyautogui library to continuously print the current cursor position. It helps in identifying screen coordinates for automation tasks.

### 02_openai.py
This script sets up the OpenAI client and sends a predefined chat history to the GPT-3.5-turbo model. It receives and prints the AI-generated response.

### 03_bot.py
This script automates the process of interacting with chat messages:

- Clicks on the Chrome icon to open the browser.
- Selects and copies the chat history.
- Checks if the last message is from a specific sender.
- If true, sends the chat history to the OpenAI API and receives a response.

# Requirements
- Python 3.x
- pyautogui library
- pyperclip library
- openai library

# Usage
- Run 01_get_cursor.py to get the screen coordinates for automation.
- Update the coordinates in 03_bot.py as needed.
- Run 03_bot.py to start the automated chat interaction.
