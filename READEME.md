\# 🚀 Zero-Touch AI Content Pipeline



\[!\[n8n](https://img.shields.io/badge/Orchestration-n8n-FF6D5A?style=for-the-badge\&logo=n8n)](https://n8n.io/)

\[!\[OpenAI](https://img.shields.io/badge/Intelligence-GPT--4o-412991?style=for-the-badge\&logo=openai)](https://openai.com/)

\[!\[Slack](https://img.shields.io/badge/Review-Slack-4A154B?style=for-the-badge\&logo=slack)](https://slack.com/)

\[!\[LinkedIn](https://img.shields.io/badge/Deployment-LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin)](https://linkedin.com/)



\## 🌐 Project Overview



\*\*The Zero-Touch Content Pipeline\*\* is a fully automated Fan-Out architecture built in n8n. It completely eliminates the manual labor of repurposing, formatting, and distributing content across multiple social media and internal team platforms.



\### 🎥 Watch the Live Demo



\[!\[Watch the Demo](https://img.youtube.com/vi/BeHkGZ8wjb4/maxresdefault.jpg)](https://www.youtube.com/watch?v=\BeHkGZ8wjb4)



I engineered this solution to handle the entire content lifecycle autonomously. By simply dropping a YouTube link into a webhook, the system fetches the transcript, uses OpenAI to generate platform-specific drafts, archives the data, alerts the team across three different messaging apps simultaneously, and auto-publishes the final post to LinkedIn via OAuth 2.0.



\*\*The Result:\*\* A 30-minute manual copy-pasting chore reduced to a 3-second automated workflow.



\---



\## ⚙️ How It Works (The Pipeline)



1\. \*\*The Trigger:\*\* A custom webhook form accepts either a raw text paste or a direct YouTube URL.

2\. \*\*Data Fetching:\*\* If a URL is provided, n8n automatically calls the YouTube API to pull the video's transcript.

3\. \*\*AI Generation:\*\* The unstructured transcript is passed to an \*\*OpenAI\*\* agent. Using prompt engineering, it outputs a structured JSON payload containing highly optimized drafts for different platforms.

4\. \*\*Parallel Archiving:\*\* The data is instantly pushed and saved to a \*\*Notion Database\*\* and \*\*Google Sheets\*\*.

5\. \*\*Internal Fan-Out (Review):\*\* The workflow simultaneously routes the generated drafts to:

&#x20;  \* \*\*Slack:\*\* Via a secure Bot Token.

&#x20;  \* \*\*Telegram:\*\* Via a direct API mobile alert.

&#x20;  \* \*\*Discord:\*\* Via a webhook delivery.

&#x20;  \* \*\*Gmail:\*\* Emailed directly to the admin.

6\. \*\*Final Deployment:\*\* Bypassing manual entry entirely, the polished draft is published directly to a live \*\*LinkedIn\*\* feed using a secure OAuth 2.0 connection.



\---



\## 🏗️ Architecture \& Features



\* \*\*Parallel Fan-Out Execution:\*\* Hits 6 different APIs simultaneously without bottlenecking.

\* \*\*Dual-Path Routing:\*\* Built-in logic to handle both API data fetching (YouTube) and manual data entry (Text block) in the same workflow.

\* \*\*Secure Authentication:\*\* Utilizes a mix of API Keys, Webhooks, Bot Tokens, and full OAuth 2.0 handshakes to ensure maximum security.



\[!\[n8n Architecture Screenshot](./dashboard-screenshot.png)](./dashboard-screenshot.png)



\---



\## 📥 Setup Guide



\### Running Locally on n8n



1\. \*\*Download:\*\* Get the `n8n-workflow-blueprint.json` file from this repository.

2\. \*\*Import:\*\* Open your n8n instance > Workflows > Import Workflow.

3\. \*\*Credentials:\*\* You will need to authenticate the following nodes using your own credentials:

&#x20;  \* OpenAI API Key

&#x20;  \* Slack Bot Token (Needs `chat:write` scope)

&#x20;  \* Telegram Bot API Key

&#x20;  \* LinkedIn OAuth 2.0 (Client ID \& Secret)

&#x20;  \* Notion Internal Integration Secret

&#x20;  \* Google Workspace Service Account

4\. \*\*Run:\*\* Click "Execute Workflow" and trigger the webhook!



\---



\## 📬 Contact



\*\*\[Saad U Ahmed Khan]\*\* \*Expert in Workflow Automation, API Integration, and AI Orchestration.\*



\[https://shorturl.at/ourBN]

