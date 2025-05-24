# 🌐 URL Health Monitor App (with Local LLM Summary)

This is a Streamlit-based web application that monitors the health (availability and response time) of one or more URLs. It logs results in a local SQLite database and optionally summarizes them using a locally running LLM like **TinyLlama via Ollama** — ensuring full privacy and offline functionality.

---

Features

-  Check the availability (UP/DOWN) of any URL
-  View response times and uptime percentages
-  Automatically generate summaries using a local LLM
-  Persistent logging using SQLite
-  View full check history
-  Clear all check logs with one click

---
## 🛠️ Installation & Usage

Step 1: Install Python Packages
pip install -r requirements.txt
Step 2: Start Ollama + Load Model
ollama run tinyllama
Make sure it's running on localhost:11434
Step 3: Run the Streamlit App
streamlit run app.py

Docker Usage 
If you prefer using Docker:
🧱 Build the image
docker build -t url-monitor .
▶️ Run the container
docker run -p 8501:8501 --add-host=host.docker.internal:host-gateway url-monitor
⚠️ Make sure ollama is installed on the host machine and running locally.

🧠 Local LLM Summary (llm_utils.py)
The app uses llm_utils.py to send data to a local LLM (like TinyLlama) and fetches natural language summaries. This is useful for users to understand large URL check results quickly.
