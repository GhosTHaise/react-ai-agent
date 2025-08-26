Here’s a polished **README.md** you can use for your GitHub project 👇

```markdown
# 🧭 AI Travel Guide Agent

An **AI-powered travel assistant** built with the [OpenAI API](https://platform.openai.com/) that follows a **Thought → Action → Observation → Answer** reasoning loop.  
The agent can answer travel-related questions by calling custom functions such as fetching the capital city, suggesting popular places, and listing other cities in a given country.

---

## ✨ Features

- 🧠 **Reasoning Loop** – Uses structured steps (`Thought → Action → Observation → Answer`) to simulate agent reasoning.  
- 🌍 **Travel Knowledge** – Retrieve:
  - The **capital city** of a given country.  
  - **Popular places** in a city worth visiting.  
  - **Other interesting cities** in a country.  
- 🤖 **Dynamic Interaction** – Combines reasoning with function-calling via OpenAI models.  
- ⚡ **Lightweight & Simple** – No external frameworks, just Python + OpenAI.  

---

## 📂 Project Structure

```

.
├── agent.py          # Main agent logic
├── .env              # Stores your OpenAI API key
├── requirements.txt  # Python dependencies
└── README.md         # Project documentation

````

---

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/ai-travel-agent.git
   cd ai-travel-agent
````

2. **Create a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set your OpenAI API key**
   Create a `.env` file and add:

   ```
   OPENAI_API_KEY=your_api_key_here
   ```

---

## ▶️ Usage

Run the agent by executing the script:

```bash
python agent.py
```

Example interaction:

```
Question: I want to visit Lithuania. I am interesting to see some good place there.
Thought: I should call get_capital_city function and give back the capital city.
Action: get_capital_city: Lithuania
PAUSE

Observation: A capital of Lithuania is Vilnius.

Answer: You should go to Vilnius and see fascinating places there! But do not forget to visit Kaunas, Klaipėda and Šiauliai!
```

---

## 🛠️ Functions

The agent has access to these functions:

* **`get_capital_city(country)`** → Returns the capital of the given country.
* **`get_popular_places(city)`** → Returns 4-5 popular tourist attractions in a city.
* **`get_other_cities_in_the_country(country)`** → Suggests other cities worth visiting in the country.

---

## 📌 Example Questions

* *"What places I can visit in France?"*
* *"What other cities in Japan should I visit?"*
* *"Tell me some popular places in London."*

---

## 📜 License

MIT License. Feel free to use and modify this project.

---

## 🚀 Roadmap

* [ ] Add more travel-related actions (restaurants, events, cultural insights).
* [ ] Integrate with a frontend (React/Next.js).
* [ ] Add memory for multi-session conversations.

---

👨‍💻 Built with ❤️ using Python & OpenAI.

```

---

Would you like me to also create the **`requirements.txt`** file (with `openai`, `python-dotenv`, etc.) so your users can set it up quickly?
```
