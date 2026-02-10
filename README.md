# 🤖 Google Apps Script Telegram Bot Collection

A collection of lightweight, serverless Telegram bots designed to run entirely on **Google Apps Script**. This repository provides a framework for automating messages, integrating AI, and managing scheduled tasks without the need for a dedicated server.

## Features
- **Serverless Architecture:** Hosted on Google's infrastructure for 24/7 uptime.
- **Easy Integration:** Connects seamlessly with Telegram Bot API and third-party APIs (like Gemini or OpenAI).
- **Scheduled Tasks:** Built-in triggers for automated daily or interval-based broadcasting.
- **Low-Code:** Minimal setup required—ideal for personal automation and small teams.

## Prerequisites
- A **Google Account** (to access Google Sheets and Apps Script).
- A **Telegram Bot Token** (obtainable from [@BotFather](https://t.me/botfather)).
- A **Chat ID** (the unique identifier for your chat, group, or channel).

## Setup Instructions

1. **Prepare the Script:**
   - Open a new [Google Sheet](https://sheets.new/).
   - Go to **Extensions** > **Apps Script**.
   - Copy the code from any `.gs` file in this repository and paste it into the editor.

2. **Configure Credentials:**
   - Locate the configuration section at the top of the script.
   - Enter your `TELEGRAM_TOKEN`, `CHAT_ID`, and any required `API_KEYS`.

3. **Authorize and Run:**
   - Click the **Save** icon.
   - Select the main function and click **Run**.
   - Review and grant the necessary permissions when prompted by Google.

4. **Set Up Automation (Triggers):**
   - Click the **Triggers** icon (the clock/alarm icon) on the left sidebar.
   - Click **+ Add Trigger**.
   - Choose the function you want to automate.
   - Set the event source to **Time-driven**.
   - Select your preferred frequency (e.g., "Minutes timer" or "Day timer").

## File Structure
- `*.gs`: Core logic files for specific bot functions.
- `appsscript.json`: Manifest file for script configuration.

## Security Note
Do not commit your real tokens or API keys to public repositories. Use **Script Properties** (`PropertiesService`) within the Apps Script environment to store sensitive information securely if sharing your code.
