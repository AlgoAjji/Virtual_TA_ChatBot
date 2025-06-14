# 🎓 TDS Virtual TA

This project is a Virtual Teaching Assistant designed to support the **TDS (Tools for Data Science)** course of the **IIT Madras  BS Degree** program. It leverages FastAPI for backend services and integrates `promptfoo` for evaluation and testing of prompts.

## 📂 Repository

GitHub: [https://github.com/23f2000288/tds_virtual_ta.git](https://github.com/23f2000288/tds_virtual_ta.git)

---

## ⚙️ Setup Instructions

Follow these steps to get the project running locally:

### 1. Clone the Repository

```bash
git clone https://github.com/23f2000288/tds_virtual_ta.git
cd tds_virtual_ta
2. Create and Activate a Virtual Environment

# For Windows
python -m venv venv
venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate
```
3. Install Required Dependencies
```bash
pip install -r requirements.txt
```
## 4. Set Up Environment Variables
Create a .env file in the project root and add your API keys. For example:

```bash
API_KEY=your_openai_api_key_here
Make sure .env is not committed to version control (already included in .gitignore).
```
### 🚀 Running the Project
Open two terminal windows:

🖥️ Terminal 1: Start FastAPI Server
```bash

uvicorn main:app --reload
This runs the FastAPI backend on http://127.0.0.1:8000

🧪 Terminal 2: Run Prompt Evaluation
bash

npx promptfoo eval --config test.yaml --no-cache
This command evaluates prompts against the backend server using the configuration in test.yaml.

📁 Project Structure
```bash

tds_virtual_ta/
├── app.py               # FastAPI app entry point
├── requirements.txt      # Python dependencies
├── .env                  # Environment variables (not committed)
├── test.yaml             # Promptfoo evaluation config
└── ...                   # Additional scripts and modules
🧠 Features
Query answering based on scraped Discourse content

API-based architecture using FastAPI

Prompt evaluation and testing using promptfoo

🤝 Contributions
Feel free to fork the repository, raise issues, or submit pull requests!

📄 License
This project is open-source and available under the MIT License.