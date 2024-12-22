# Speech-to-Speech Language Translation Application

This application is a **real-time speech-to-speech language translation tool** built using Python. It allows users to input speech in one language, translate it into another, and play the translated speech using text-to-speech (TTS). The user-friendly interface makes it easy to use for multilingual communication.

---

## Features

- **Real-time Speech Recognition:** Convert spoken input into text using Google Speech Recognition.
- **Language Translation:** Translate the recognized text into the desired language using the Google Translator API.
- **Text-to-Speech Output:** Play the translated text in the output language using `gTTS`.
- **Transliteration Support:** Convert text to native scripts for supported languages.
- **Interactive GUI:** Built with Tkinter, featuring dropdown menus for language selection, text display areas, and buttons for interaction.

---

## Technologies Used

- **Python:** The core programming language.
- **Tkinter:** For building the graphical user interface.
- **gTTS:** To convert translated text to speech.
- **Google Speech Recognition API:** For recognizing spoken input.
- **Google Translator API (via `deep_translator`):** For translating text between languages.
- **`playsound`:** To play the generated speech audio.
- **`threading`:** For managing background processes without freezing the GUI.

---

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/AyushKumarThakur21BCE3771/Speech-to-Speech-Language-Translation-Application.git
   cd speech-to-speech-translation
   ```

2. **Install Dependencies:**
   Use `pip` to install the required libraries:
   ```bash
   pip install tkinter gtts speechrecognition playsound deep-translator google-transliteration
   ```

3. **Run the Application:**
   ```bash
   python app.py
   ```

---

## How to Use

1. **Launch the Application:** Run the Python script to open the GUI.
2. **Select Languages:** Choose the input and output languages from the dropdown menus.
3. **Start Translation:**
   - Click the "Start Translation" button.
   - Speak into your microphone when prompted.
4. **Output:** The recognized text and its translation will appear in the text areas. The translated speech will also play automatically.
5. **Stop Translation:** Speak "stop" or "exit" to stop the process.

---

## Supported Languages

The application currently supports the following languages:
- **Input/Output Languages:** English, Hindi, Bengali, Tamil, Telugu, Kannada, Gujarati, Punjabi.

---

## Known Issues and Limitations

- **Internet Dependency:** Requires an active internet connection for speech recognition and translation.
- **Accuracy:** Translation and speech recognition accuracy may vary depending on the quality of the microphone and clarity of speech.
- **Temporary File Management:** Audio files are deleted after playback, but unexpected crashes may leave undeleted files.

---

## Future Enhancements

- Add support for more languages and scripts.
- Enhance error handling and retry mechanisms.
- Include visual feedback for real-time status (e.g., progress bars).
- Improve GUI design for better usability.