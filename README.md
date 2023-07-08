# README.md
## Project Overview
This project aims to create a Slack bot that utilizes the OpenAI GPT-3.5-turbo model as an intelligent language model assistant. The bot can handle a wide range of tasks, such as answering simple questions, engaging in conversations, providing in-depth explanations, and offering insights on various topics.

The Slack bot is powered by langchain, a package that provides a chat framework for language model-based AI services. The project also makes use of Flask for the web server and the Slack Bolt Python package for easy interactions with the Slack API.

The following features are included in this project:

Conversation management with memory for context retention
Slack event handling for messages and mentions
Flexible conversation prompt template
OpenAI GPT-3.5-turbo as the language model

## Prerequisites
Python 3.6 or later
A Slack bot token
An OpenAI API key
A signing secret from your Slack app

## How to Deploy
### 1.Clone the repository
Clone the repository to your local machine:
```
git clone 
```
### 2.Install dependencies
Navigate into the cloned repository directory and install the necessary dependencies using 

```
cd <repository-directory>
pip install -r requirements.txt
```
### 3.Set up environment variables
change the .envexample file to .env at the root of your project and initialize the following environment variables:
```
SLACK_BOT_TOKEN=<Your Slack Bot Token>
OPENAI_API_KEY=<Your OpenAI API Key>
SIGNING_SECRET=<Your Slack App Signing Secret>
```
Replace <Your Slack Bot Token>, <Your OpenAI API Key>, and <Your Slack App Signing Secret> with your own values.

### 4.Start the server
Run the main script to start the server:The server will start running on http://localhost:5001.

### 5.Run your Ngrok instance to create a public URL for your local server
run it in terminal
```
ngrok http 3000
```
if ngrok not installed, install through following command in macos terminal:
```
brew install ngrok
```
### 6.Go to your Slack App's settings in the Slack API dashboard.
Set the Request URL under 'Event Subscriptions' to the https URL provided by ngrok, followed by /slack/events.
After setting up, you can interact with the bot in Slack by directly messaging the bot or mentioning the bot in a channel.
**Enjoy chatting with your new AI-powered Slack bot!**

