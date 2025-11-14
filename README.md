Jarvis Voice Assistant

A simple Python-based voice assistant capable of listening to user commands, performing web searches, speaking responses, and executing basic tasks like opening websites or checking the time.

Features

Text-to-speech using pyttsx3

Speech recognition using Google Speech API

Greets the user based on time of day

Searches Wikipedia and reads results aloud

Opens common websites (YouTube, Google, StackOverflow)

Announces current time

Continuously listens for new commands

Requirements

Install the required dependencies before running the project.

pip install pyttsx3
pip install speechrecognition
pip install wikipedia
pip install comtypes


For speech recognition to work, install PyAudio:

Windows:

pip install pipwin
pipwin install pyaudio


Linux:

sudo apt-get install python3-pyaudio

How It Works

The assistant initializes a speech engine using pyttsx3.

It greets the user depending on the current time.

It listens using the system microphone and processes the speech into text.

Based on keywords in the user's command, it performs actions such as:

Searching Wikipedia

Opening websites

Telling the time

It continues running in a loop until stopped manually.

File Structure
jarvis.py
README.md

How to Run

Run the script directly from your terminal:

python jarvis.py


Ensure your microphone is enabled and functional.

Customization

Update the name "priyanga" in the script to personalize greetings.

Add more voice commands by extending the if/elif blocks.

Change the default voice by modifying the pyttsx3 voice index.

Limitations

Requires an active internet connection for speech recognition and Wikipedia search.

Accuracy depends on microphone quality and ambient noise.

License

This project is for educational purposes. You may modify and use it freely.
