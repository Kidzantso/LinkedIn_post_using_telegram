# 🤖 LinkedIn Posts from GitHub with n8n

This n8n workflow automates the process of extracting content from a `README.md` file in a GitHub repository and sending it to Telegram — perfect for previewing or preparing LinkedIn posts.

## 🚀 Features

- 📂 Fetches a Markdown file (e.g., `README.md`) from a GitHub repo you choose
- 🧾 Extracts and parses the file content
- 🧠 (Optional) Sends the content to an AI model for summarization or formatting
- 💬 Sends the final message to your personal Telegram account

## 🧱 Workflow Structure

| Step | Node Name            | Description |
|------|----------------------|-------------|
| 1    | `Telegram Trigger`   | Starts the workflow when you send a message to your bot with the project name you want|
| 2    | `Get a file`         | Retrieves the Markdown file (binary) |
| 3    | `Extract from File`  | Converts the binary file into raw Markdown text |
| 4    | `Markdown`           | Converts Markdown to HTML (optional) |
| 5    | `Message a model`    | (Optional) Sends content to an AI model for enhancement |
| 6    | `Send a text message`| Sends the final message to your Telegram chat |

## 📦 Requirements

- An active [n8n](https://n8n.io) instance
- A Telegram bot created via [@BotFather](https://t.me/BotFather)
- Your Telegram Chat ID (retrievable via [@userinfobot](https://t.me/userinfobot))
- (Optional) OpenAI or other model credentials if using the AI node

## 🛠️ Setup Instructions

1. Clone this repo or import the workflow JSON into your n8n instance.
2. Set up your Telegram credentials and insert your Chat ID.
3. Configure the file source (e.g., GitHub URL or local path).
4. (Optional) Customize the AI message formatting.
5. Trigger the workflow by messaging your bot.

## 📌 Use Case

This workflow is ideal for developers who want to:
- Preview GitHub project descriptions before posting on LinkedIn
- Automate content formatting for social media
- Quickly test Markdown content via Telegram

## 📸 Demo

![image](https://github.com/user-attachments/assets/e8bda7d1-68b2-4d89-b8f7-b541ba886a68)

## 🧠 Author

**Nader Maged**  
Backend Developer | Automation Enthusiast  
[LinkedIn](www.linkedin.com/in/nader-maged) • [GitHub](https://github.com/Kidzantso)

---

