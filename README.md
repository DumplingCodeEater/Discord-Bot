# Da Chin Discord Bot

This is a Discord bot with various functions, primarily serving as a YouTube audio music bot in voice channels.<br>
<br>
<p align="left">
<img src="https://github.com/user-attachments/assets/7ed6578c-eaec-4bb9-8ff7-bc5131aaec54" width="500" height="400">
</p>

## Table of Contents
1. [Features](#features)
2. [Prerequisites](#prerequisites)
3. [Setup and Installation](#setup-and-installation)
4. [License](#license)

## Features

- **Rainbow Text Animation**:<br>
  The ```$nay``` command creates a rainbow text animation with the provided username, displaying a colorful message in the chat.
- **Text-to-Speech (TTS)**:<br> The ```$tts``` command plays a text-to-speech message in the voice channel the user is in, converting the provided text into speech.
- **Play Audio from URL or File**:<br> The ```$urlplay_downloaded``` and ```$urlplay``` commands allow the bot to play audio from a downloaded file or a YouTube URL in the voice channel.
- **Search and Queue YouTube Videos**:<br> The ```$search``` command searches for a YouTube video based on the provided query and queues it in the playlist.
- **Pause and Resume**:<br> The ```$pause``` and ```$resume``` commands allow users to pause and resume the currently playing song.

## Prerequisites

- **[Python 3.10+](https://www.python.org/downloads/)**
- **[Docker](https://www.docker.com/products/docker-desktop/)**
- **Other Libraries/Dependencies**: Listed in `requirements.txt`

## Setup and Installation
### 1. Clone the Repository and Navigate to the project directory:
```bash
git clone https://github.com/DumplingCodeEater/Discord-Bot.git
cd Discord-Bot
```
### 2. Set Up Environment Variables:
Refer to the following site for help on getting a discord bot token: <a>https://www.writebots.com/discord-bot-token/</a>
- Option 1: Create a ```.env``` file in the root directory and add your discord bot token.
- Option 2: Add your discord bot token as a secret (if your server gives you an option to add secrets)

*Replace "your_discord_token" below with your actual discord bot token*
```env 
TOKEN = "your_discord_token"  
```
### 3. Run the Dockerfile:
```Dockerfile
docker build -t discord-bot .
docker run --env-file .env discord-bot
```
## License
Distributed under the MIT License. See LICENSE.txt for more information.
