# 🤖 Customer Service Bot

Welcome to the **Customer Service Bot** repository! This bot leverages artificial intelligence (AI) and machine learning to provide instant responses to customer queries through a business messenger. Built with Rasa, it can understand various forms of the same question, continuously learn from interactions, and offer 24/7 support.

---

## 🚀 Features
- 🧠 **AI-Powered Support:** Uses AI and machine learning to understand and respond to customer queries.
- 🔍 **Natural Language Processing (NLP):** Employs advanced NLP techniques with libraries like Rasa, Spacy, and NLTK.
- ⚡ **Instant Responses:** Recognizes and answers multiple forms of the same question quickly.
- 🌍 **24/7 Availability:** Provides round-the-clock support to customers.
- 🔄 **Continuous Learning:** The bot improves its responses over time by learning from previous interactions.
- 🗣️ **Custom Voice and Tone:** Easily trainable to reflect your preferred voice or text style.
- 📊 **Analytics Ready:** Track support metrics to understand customer needs and satisfaction.

---

## 🛠️ Built With
- **Rasa**: An open-source conversational AI framework.
- **Spacy**: Industrial-strength NLP library.
- **NLTK**: Natural Language Toolkit for linguistic data processing.
- **FuzzyWuzzy**: String matching library for improving query understanding.
- **Pandas**: Data analysis and manipulation library.

---

## 🏁 Getting Started

Follow these steps to set up and run the project on your local machine.

### ✅ Prerequisites
Install the required dependencies:
```bash
$ pip3 install rasa==1.10.8
$ pip3 install rasa[spacy]
$ python -m spacy download en_core_web_md
$ python -m spacy link en_core_web_md en
$ pip3 install pandas==1.1.0
$ pip3 install nltk==3.5
$ pip3 install fuzzywuzzy==0.18.0
```

### 🐍 Setting Up the Environment
1. **Create a Conda environment** and install the necessary libraries within it.
2. **Add the project's directory** to your Python environment variable:
   - Example: `PATH = D:\Projects...\Customer-Service-Bot`

### ⚙️ Extra Configuration
- **Set Console Channel Timeout**: Go to `Anaconda3\envs\{your_rasa_env}\Lib\site-packages\rasa\core\channels\console.py` and update `DEFAULT_STREAM_READING_TIMEOUT_IN_SECONDS=200`.

---

## 🤖 How to Train and Run the Bot

### 🏋️ Training
1. **Train with default Rasa configurations**:
   ```bash
   $ rasa train
   ```
2. **Train with Spacy configuration (faster)**:
   ```bash
   $ rasa train -c spacy_config.yml
   ```

### 🔧 Running the Bot
1. **Run the action server**:
   ```bash
   $ rasa run actions --actions actionserver.actions
   ```
2. **Run Rasa in debug mode** (for inspecting slot filling and entities):
   ```bash
   $ rasa shell --debug
   ```
3. **Run Rasa in normal shell**:
   ```bash
   $ rasa shell
   ```

---

## 📈 Usage and Benefits

Customer service chatbots help businesses deliver more efficient support:
- **Instant Resolutions**: Quickly respond to customer queries.
- **Seamless Hybrid Support**: Integrate with live chat for complex issues.
- **24/7 Availability**: Provide support around the clock.
- **Scalability**: Easily handle increasing volumes of customer queries.
- **Reduced Costs**: Lower customer service expenses by automating responses.
- **Increased Customer Satisfaction**: Minimize response times and improve support quality.

---

## 🌱 Roadmap
- [ ] **Multi-language support** 🌍
- [ ] **Integration with popular CRM systems** 📋
- [ ] **Voice-based interaction support** 🎤
- [ ] **Enhanced analytics and reporting** 📊
- [ ] **Integration with social media platforms** 📱

---

## 👥 Contributing
We welcome contributions! Here's how you can get involved:
1. **Fork the repository**.
2. **Create a new feature branch** (`git checkout -b feature/AmazingFeature`).
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`).
4. **Push the branch** (`git push origin feature/AmazingFeature`).
5. **Open a pull request**.

---

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgements
- **RASA**: For the conversational AI framework.
- **RASA Forums**: For community support and discussions.

Feel free to explore the project, suggest new features, or report issues! 🚀
