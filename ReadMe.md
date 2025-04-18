MediFriend: A Friend Indeed.

MediFriend is a user-friendly AI-powered Streamlit web application that translates natural language queries into SQL commands and retrieves information about doctors from a healthcare database. It's designed to help users get insights from medical data without writing any SQL code themselves.

🚀 Features
✅ Natural language to SQL conversion using Google Gemini Pro API

✅ Secure SQL execution with SQLite backend

✅ Interactive and responsive Streamlit UI

✅ Doctor-related insights: search by location, specialization, insurance provider, and rating

✅ Displays results in tabular format via pandas.DataFrame

✅ Stylish branding with logo and tagline

🧠 How It Works
User types a question in plain English (e.g., "List doctors in New York specializing in cardiology.").

The app uses the Gemini Pro model from Google’s Generative AI suite to convert the question into an SQL query.

The SQL query is executed on a local SQLite database (healthcare.db).

The result is displayed in a clean, scrollable table.

📦 Requirements
Install the dependencies using pip:

bash
Copy code
pip install -r requirements.txt

API Key Setup
This app uses the Google Generative AI (Gemini) API. To use it:

Generate your API key from Google AI Studio.

Create a .env file in the root directory with the following content:

ini
Copy code
API_KEY=your_api_key_here
Note: In this implementation, the key is hardcoded for testing:

python
Copy code
genai.configure(api_key="YOUR_KEY_HERE")

🛠️ Run the App
bash
Copy code
streamlit run app.py
Replace app.py with your actual file name if different.
