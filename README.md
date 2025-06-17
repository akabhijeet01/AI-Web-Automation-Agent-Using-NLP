🕵️‍♂️ Browser MCP Agent
A powerful, interactive web-based agent built using Streamlit and MCP Agent, capable of navigating and interacting with websites using Puppeteer automation. It integrates OpenAI's LLMs to understand and execute natural language commands for intelligent web browsing.

🚀 Features
🌐 Web Navigation: Visit and explore any website through natural language prompts.

🖱️ Interaction: Click, scroll, and extract data from web pages.

🧠 NLP-Powered Reasoning: Uses OpenAI LLMs (via the MCP Agent) to interpret commands and plan browser actions.

🧾 Summarization: Extract and summarize web content using advanced language models.

📸 Screenshot Capabilities: Take snapshots of specific web elements.

🧠 Multi-step Task Execution: Follow complex, step-by-step instructions in natural language.

🧠 Natural Language Processing (NLP)
This project uses OpenAI's GPT models through the MCP Agent framework to:

Parse user commands in natural language (e.g., "Go to Wikipedia and summarize the page").

Translate those commands into actionable browser steps.

Generate human-readable summaries of web content.

Maintain conversational context to handle follow-up instructions.

The integration is powered by the OpenAIAugmentedLLM module with history tracking enabled, allowing contextual and coherent responses across multi-turn instructions.

🖼️ Demo UI
The app provides a simple Streamlit UI with:

A text input for your command.

A button to trigger the browser agent.

A markdown-based output panel to display results.

🧱 Project Structure
bash
Copy
Edit
📁 your-repo/
├── main.py              # Streamlit app and LLM integration
├── requirement.txt      # Required dependencies
🧑‍💻 How to Run
🔧 Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/browser-mcp-agent.git
cd browser-mcp-agent
Create a virtual environment and activate it:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirement.txt
Set your OpenAI API key:

bash
Copy
Edit
export OPENAI_API_KEY=your-key-here  # On Windows: set OPENAI_API_KEY=your-key-here
▶️ Run the App
bash
Copy
Edit
streamlit run main.py
💬 Example Commands
Try using commands like:

Go to wikipedia.org/wiki/computer_vision

Scroll down and summarize the page

Click on the link to object detection and take a screenshot

Navigate to Wikipedia, scroll and extract bullet points from the page

📦 Dependencies
streamlit >= 1.28.0

mcp-agent >= 0.0.14

openai >= 1.0.0

asyncio

⚠️ Notes
Ensure Puppeteer is set up and accessible via MCP Agent tools.

The OPENAI_API_KEY is required for NLP and summarization tasks to work.

