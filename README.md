GenAIChatBot
This repository hosts a simple website embedding an AI chatbot built with Gradio on Hugging Face Spaces. The chatbot uses OpenAI's gpt-3.5-turbo and Hugging Face's Mixtral-8x7B-Instruct-v0.1 models, allowing users to interact via a web interface.
File Structure
/GenAIChatBot
├── index.html      # HTML with Gradio web component
├── styles.css      # CSS for styling
└── script.js       # JavaScript for interactivity

Setup

Clone the Repo:
git clone https://github.com/<your-username>/GenAIChatBot.git
cd GenAIChatBot


Test Locally:

Use VS Code Live Server: Right-click index.html > "Open with Live Server" (http://localhost:5500).
Or use Python: python -m http.server 8000 and open http://localhost:8000.


Verify Gradio Embed:

Ensure index.html has:<div class="chat-bot-container">
    <gradio-app src="https://shini1803bsm-myfirstgenaiapp.hf.space"></gradio-app>
</div>





Deployment

Push to GitHub:
git add .
git commit -m "Add website files"
git push origin main


Enable GitHub Pages:

Go to repo Settings > Pages.
Set Source to main branch, folder / (root).
Access at https://<your-username>.github.io/GenAIChatBot.



Usage

Visit the deployed site.
Use the chatbot: Select "OpenAI" or "HuggingFace," enter a prompt, and adjust sliders (max_tokens, temperature, top_p).

Troubleshooting

Chatbot Not Loading: Ensure the Hugging Face Space (https://shini1803bsm-myfirstgenaiapp.hf.space) is public and running.
OpenAI Error: Verify OPENAI_API_KEY in Space settings; check billing at OpenAI.
Hugging Face Error: Confirm HF_TOKEN in Space settings; ensure model (mistralai/Mixtral-8x7B-Instruct-v0.1) is valid.
