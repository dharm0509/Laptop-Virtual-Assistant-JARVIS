# Laptop-Virtual-Assistant-JARVIS
This project is a desktop voice assistant inspired by J.A.R.V.I.S. from Iron Man.
It uses speech recognition, text-to-speech, and a modern web-based GUI built with Eel. The assistant runs two processes: one for GUI and interaction, and another for hotword detection.

🚀 Features
1. Modern GUI using Eel (Python + HTML/JS)

2. Multitasking with multiprocessing: one for the assistant, one for hotword

3. Speech-to-text (listen and respond)

4. Text-to-speech responses

5. Command execution module

6. Hotword detection module

7. Automatically opens in Microsoft Edge app mode

🗂️ Project Structure

.
├── run.py                   # Main entry point with multiprocessing \n
├── main.py                  # Starts the Eel web app \n
├── sooha.db                 # Database (usage assumed in engine module) \n
├── engine/ \n
│   ├── features.py          # Speech features (hotword, speak, etc.) \n
│   └── command.py           # Custom command logic \n
├── www/
│   └── index.html           # Web UI for the assistant \n
Note: Actual contents of engine/ and www/ folders are assumed based on usage.

🔧 Requirements
Install dependencies:
pip install eel pyttsx3 SpeechRecognition
Also ensure you have:
Microsoft Edge (optional; used to open GUI in app mode)
Microphone (for voice input)

🧠 How it Works
run.py launches two separate processes:

1. One runs the GUI and assistant (main.py)
2. Another listens for hotword using microphone input

When the assistant starts, it opens index.html in a browser app window.
Voice commands are processed, and the assistant responds using TTS.

🏁 How to Run
python run.py
This starts both assistant and hotword listener.
GUI will automatically open in Microsoft Edge.
Use your voice to interact!


⚠️ Notes
The assistant expects certain directories (engine/, www/) and files (index.html, database, etc.).
You can change browser or port in main.py.


📌 To-Do Ideas
1. Add chatbot integration (e.g., ChatGPT API)

2. Add system-level controls (volume, brightness)

3. Add music or app launching

4. Enhance GUI with animations

🧑‍💻 Author
Dharm Rathod
BTech CSE-AIML | PPSU College
