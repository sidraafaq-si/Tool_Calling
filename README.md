Tool-Calling Assistant with OpenAI and Agents Library
This project demonstrates how to build a conversational AI assistant that uses tool calling (aka function calling) to dynamically invoke Python functions like fetching weather or generating random jokes. It uses the agents library with OpenAI's GPT models.

🔧 Features
✅ Built using agents framework
🛠️ Tool-calling support via @function_tool
🌦️ Weather data from WeatherAPI
😂 Random joke generation based on tool result
🧠 Example Usage
User:

"Tell me some jokes"

Assistant:

(Internally calls how_many_jokes() to get a random number, then responds with that many jokes)

🚀 Setup Instructions
1. Clone the repo and create a virtual environment
git clone https://github.com/your-username/tool-calling-assistant.git
cd tool-calling-assistant
python -m venv .venv
source .venv/bin/activate  # or `.venv\Scripts\activate` on Windows
2. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Set up environment variables
Create a .env file in the project root:

env
Copy
GEMINI_API_KEY=your_gemini_api_key_here
WEATHER_API_KEY=your_weatherapi_key_here
🧪 Run the Assistant
bash
Copy
Edit
uv run main.py
Make sure uv is installed. If not:

bash
Copy
Edit
pip install uv
📦 Dependencies
openai

requests

python-dotenv
