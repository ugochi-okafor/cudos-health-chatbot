# HealthBot - Health-Based Telegram Chatbot

HealthBot is a Telegram chatbot designed to provide health-related information and assistance. It leverages the innovations from Large Language Models to understand user queries and provide accurate responses based on trusted health resources. This bot is intended to offer general health advice, answer medical questions, and promote well-being with easy-to-understand content.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Set Up Telegram Bot Token](#set-up-telegram-bot-token)
5. [Usage](#usage)
6. [How It Works](#how-it-works)
7. [Creating Virtual Machine](#creating-virtual-machine)
8. [Deploying the Model](#deploying-the-model)

## Introduction

HealthBot is a Telegram chatbot built with Python, utilizing the Telegram Bot API and NLP techniques to provide personalized health information. It aims to answer health-related queries, offer guidance on well-being, and connect users with healthcare resources. The bot can assist with general topics such as fitness, nutrition, mental health, symptoms, and more. 

## Features

- **Health Queries**: Answer questions about general health, symptoms, and wellness.
- **NLP-Powered**: Uses Natural Language Processing to understand user questions.
- **Interactive Responses**: Engages users with personalized responses and health advice based on the users' queries.

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

1. **User Input**: Users send a message or command to the bot.
2. **Message Processing**: The message is converted into an embedding, which is a rich representation of a text document.
3. **Response Generation**: The bot retrieves the relevant document, either from the medical vector databases or generates a response using an LLM (e.g., GPT).
4. **Response Delivery**: The bot sends back the processed response to the user on Telegram.

This architecture ensures that the bot can handle a wide variety of health-related queries in real-time.

## Creating Virtual Machine

<b> Step 1:</b> Create a new GPU instance

<b> Step 2:</b> Select an Instance with a GPU

<b> Step 3:</b> Create an SSH public key using the following command

```bash
ssh-keygen -t rsa -b 4096 -f C:\Users\USER\.ssh\vm_key.pub
```

### Step 4: Copy the key

```bash
cat C:\Users\USER\.ssh\vm_key.pub
```

### Step 5: Paste the key

### Step 6: Deploy the instance

## Deploying the Model

### Step 1: Copy the IP Address of the Created Virtual Machine

### Step 2: Login to the Virtual Machine

```bash
ssh -i path_to_key root@IP_Address
```

### Step 3: Update the Virtual Machine

```bash
sudo apt update
```

### Step 4: Clone the GitHub Repository

```bash
git clone repo_path  # Update with the actual repository path
```

### Step 5: Install pip

```bash
sudo apt install python3-pip
```

### Step 6: Install the requirements.txt file

```bash
pip install -r requirements.txt
```

### Step 7: Create and Upload the .env File

```bash
nano .env
```

### Step 8: Paste .env File Content

```plaintext
HF_TOKEN=
BOT_TOKEN=
```

### Step 9: Run the Main File

```bash
python3 main.py
