# HealthBot - Health-Based Telegram Chatbot

HealthBot is a Telegram chatbot designed to provide health-related information and assistance. It leverages the innovations from Large Language Models to understand user queries and provide accurate responses based on trusted health resources. This bot is intended to offer general health advice, answer medical questions, and promote well-being with easy-to-understand content.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [How it Works](#how-it-works)
6. [Training (Optional)](#training-optional)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction

HealthBot is a Telegram chatbot built with Python, utilizing the Telegram Bot API and NLP techniques to provide personalized health information. It aims to answer health-related queries, offer guidance on well-being, and connect users with healthcare resources. The bot can assist with general topics such as fitness, nutrition, mental health, symptoms, and more. 

## Features

- **Health Queries**: Answer questions about general health, symptoms, and wellness.
- **NLP-Powered**: Uses Natural Language Processing to understand user questions.
- **Interactive Responses**: Engages users with personalized responses and health advice based on the users queries.

## Installation

### Prerequisites

- Python 3.7 or higher
- A Telegram bot token from [BotFather](https://core.telegram.org/bots#botfather)

### Clone the Repository

```bash
git clone https://github.com/ugochi-okafor/cudos-health-chatbot/
cd healthbot
```

### Install Dependencies
Install all required dependencies using pip:

```bash
pip install -r requirements.txt
```

## Set Up Telegram Bot Token
- Create a new bot with BotFather on Telegram.
- Get the token and store it securely.
- Create a .env file in the root directory and add your bot token:

```bash
TELEGRAM_API_TOKEN=your-bot-token-here
```

## Usage
Once you've set up the bot, you can start it by running:

```bash
python main.py
```

The bot will start interacting with users on Telegram.


## How It Works
HealthBot works by using the Telegram Bot API to receive user input, process the query using Natural Language Processing (NLP), and then provide relevant information. Here’s a breakdown of how the bot operates:

1. User Input: Users send a message or command to the bot.
2. Message Processing: The message given is converted into embedding. WHich is a rich representation of a text document. 
3. Response Generation: The bot retrieves the relevant docuemnt, either from the medical vector databases, or generates a response using an LLM (e.g., GPT).
4. Response Delivery: The bot sends back the processed response to the user on Telegram.

This architecture ensures that the bot can handle a wide variety of health-related queries in real-time.
