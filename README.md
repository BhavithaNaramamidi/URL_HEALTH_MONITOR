# URL_HEALTH_MONITOR
URL Health Monitor is a streamlined web application built with Python, Streamlit, and SQLite to check the status of multiple websites in real-time. It allows users to monitor the uptime and response time of URLs and visualize their performance history over time.

🔍 Features
🔗 Enter multiple URLs and check their status (UP/DOWN)

⚡ View response time in milliseconds

💾 Stores historical data using SQLite

📊 See uptime percentage and trends with real-time charts

🧠 Clean, minimal interface built with Streamlit

⚙️ Tech Stack
Python – Core programming language

Streamlit – For building the frontend UI

Requests – To perform HTTP health checks

SQLite – To store health metrics

Pandas + Matplotlib – For data handling and visualization

🚀 Getting Started
🔧 Run Locally (Without Docker)
bash
Copy
Edit
# 1. Clone the repository
git clone https://github.com/your-username/url-health-monitor.git
cd url-health-monitor

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the app
streamlit run app.py
Visit http://localhost:8501 in your browser.

🐳 Run with Docker (Optional)
bash
Copy
Edit
# Build the Docker image
docker build -t url-health-monitor .

# Run the Docker container
docker run -p 8501:8501 url-health-monitor
Then open: http://localhost:8501
