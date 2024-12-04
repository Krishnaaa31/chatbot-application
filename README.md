 Chatbot Using NLP

 Overview
This project implements a chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to understand user intents and provide appropriate responses based on predefined patterns and responses. It utilizes the **NLTK** library for natural language processing, **Scikit-learn** for machine learning, and **Streamlit** for creating an interactive web interface.

 Features
- Understands various user intents such as greetings, farewells, gratitude, and more.
- Provides relevant responses based on user input.
- Maintains a conversation history that can be viewed by the user.
- Highly customizable through the `intents.json` file.
- Built using Python and integrates cutting-edge libraries for NLP and machine learning.

 Technologies Used
- **Python**
- **NLTK** for natural language processing.
- **Scikit-learn** for machine learning.
- **Streamlit** for creating an interactive web interface.
- **JSON** for defining intents and responses.

 Installation and Setup

 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate   On Windows use `venv\Scripts\activate`
```

 3. Install Required Packages
```bash
pip install -r requirements.txt
```

 4. Download NLTK Data
Add this snippet to download necessary NLTK data:
```python
import nltk
nltk.download('punkt')
```

 5. Run the Application
To start the chatbot, run the following command:
```bash
streamlit run app.py
```
The application will open in your web browser. You can interact with the chatbot by typing your message into the input box and pressing Enter.

 Intents Data
The chatbot's behavior is defined in the `intents.json` file, which includes:
- **Tags**: Identifiers for different intents.
- **Patterns**: User input examples for each intent.
- **Responses**: Predefined chatbot replies for each intent.

You can customize the chatbot by editing this file to:
- Add new intents.
- Update existing patterns or responses.

 Conversation History
The chatbot automatically saves conversation history in a file named `chat_log.csv`. To view past interactions, use the "Conversation History" option in the Streamlit sidebar.

 Example Interaction
**User Input**: "Hi"  
**Chatbot Response**: "Hello! How can I assist you today?"

 Example `intents.json` Structure
```json
[
  {
    "tag": "greeting",
    "patterns": ["Hi", "Hello", "Hey", "What's up"],
    "responses": ["Hello!", "Hi there!", "Hey! How can I help?"]
  },
  {
    "tag": "goodbye",
    "patterns": ["Bye", "See you later", "Goodbye"],
    "responses": ["Goodbye!", "See you later!", "Take care!"]
  }
]
```

 Directory Structure
```
chatbot/
│
├── app.py               Main application file
├── intents.json         Intents and responses
├── chat_log.csv         Conversation history
├── requirements.txt     Dependencies
├── README.md            Project documentation
└── chatbot.ipynb        Optional Jupyter Notebook for training
```

 License
This project is licensed under the [MIT License](LICENSE).

 Acknowledgments
Special thanks to the open-source libraries that made this project possible:
- **NLTK** for NLP processing.
- **Scikit-learn** for machine learning.
- **Streamlit** for an interactive user interface.

---

This comprehensive file should serve as both documentation and guidance for your project. Let me know if further adjustments are needed!
