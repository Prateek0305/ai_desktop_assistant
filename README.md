# Erica – Voice Assistant in Python

Erica is a Python-based voice assistant that can perform a variety of tasks such as searching Wikipedia, opening websites, playing music, telling the time, and sending emails — all through simple voice commands.

## ✨ Features

- 🎤 **Voice Recognition** – Uses `speech_recognition` to understand your commands.
- 🗣 **Text-to-Speech** – Speaks responses using `pyttsx3`.
- 📚 **Wikipedia Search** – Fetches quick summaries from Wikipedia.
- 🌐 **Web Navigation** – Opens YouTube, Google, and custom URLs.
- 🎵 **Music Playback** – Plays songs from a specified local directory.
- ⏰ **Time Announcement** – Tells the current time.
- 📧 **Email Sending** – Sends emails using SMTP.

## 🛠 Installation

1. **Clone the repository** (or download the script):
   ```bash
   git clone https://github.com/yourusername/erica-voice-assistant.git
   cd erica-voice-assistant
2. Install dependencies:
   ```bash
   pip install pyttsx3 speechrecognition wikipedia

3. (Optional) Install PyAudio (required for microphone input):
   --Windows:
     ```bash
     pip install pipwin
     pipwin install pyaudio
     ```
    --Mac/Linux:
  ```bash
      pip install pyaudio
```
4. Run the script:
    ```bash
   python erica.py



##🚀 Usage

1. **Run the assistant**:  
   Run this command in your terminal: `python erica.py`
 ```
2. **Speak a command** when prompted.  
   Example commands:
    ```
   - `Wikipedia Albert Einstein`  
   - `Open YouTube`  
   - `Open Google`  
   - `Play music`  
   - `The time`  
   - `Open code`  
   - `Email to Prateek`
 ```
3. **Email Feature**:
 ```
   - When you say `Email to Prateek`, the assistant will ask:  
     *What should I say?*  
   - Speak your message, and it will send the email using the configured credentials.
 ```
4. **Exit the assistant**:
    ```
   - Close the terminal window or press `Ctrl + C`.

5. **Features**
```
- **Voice Recognition** – Listens to your voice commands using `SpeechRecognition`.
- **Wikipedia Search** – Fetches quick summaries from Wikipedia.
- **Web Navigation** – Opens YouTube, Google, or custom links in your browser.
- **Music Playback** – Plays music from a predefined local directory.
- **Time Announcements** – Tells you the current time.
- **Code Launcher** – Opens Visual Studio Code directly.
- **Email Sending** – Sends emails through Gmail SMTP by voice command.
- **Personalized Greeting** – Greets you based on the time of day.
```
## 📂 Project Structure

Erica-Voice-Assistant/
│
├── erica.py # Main Python script
├── README.md # Project documentation
├── requirements.txt # Python dependencies
└── assets/ # Optional folder for images, audio, etc.

## 📦 Requirements

- Python 3.6+
- `pyttsx3` – Text-to-speech conversion
- `speech_recognition` – Voice command recognition
- `wikipedia` – Fetch summaries from Wikipedia
- `smtplib` – Sending emails
- `webbrowser` – Open websites
- `os` & `datetime` – System operations and time

Install dependencies using:

```bash
pip install pyttsx3 SpeechRecognition wikipedia
```
🙌 Acknowledgements
```bash
pyttsx3 – Text-to-Speech engine
SpeechRecognition – Voice input handling
Wikipedia API – Wikipedia content fetching
Inspiration from classic JARVIS AI assistants
```
---

## 🤝 Contributing

Contributions are welcome!  
If you’d like to add new features, fix bugs, or improve documentation, follow these steps:

1. **Fork** the repository  
2. **Create** a new branch:  
   ```bash
   git checkout -b feature-name


    

