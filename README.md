# 🌐 AI Voice & Text Translator

An AI-powered web application that demonstrates how speech processing and machine translation can be combined to translate languages through both **voice and text input**.

The project demonstrates an end-to-end language translation pipeline:

**Speech-to-Text → Language Processing → Machine Translation → Translated Text → Text-to-Speech**

---

## 🚀 Project Overview

Language barriers can make communication difficult in education, travel, healthcare, business, and everyday conversations.

This project provides a simple web-based translator that allows users to:

- Enter text manually
- Speak using a microphone
- Convert speech into text
- Translate text between supported languages
- View the translated result
- Listen to the translated text using text-to-speech

---

## ✨ Features

- 🎤 **Speech-to-Text**
  - Converts spoken input into text using the browser's Speech Recognition API.

- ⌨️ **Text Input**
  - Users can directly type the sentence they want to translate.

- 🌐 **Machine Translation**
  - Translates text from a selected source language to a target language using a machine translation service.

- 🔊 **Text-to-Speech**
  - Converts translated text into speech using the browser's SpeechSynthesis API when a suitable target-language voice is available.

- 🔄 **Language Selection**
  - Supports multiple languages including English, Telugu, Hindi, Tamil, Kannada, Malayalam, Spanish, French and German.

- 📋 **Copy Translation**
  - Allows users to easily copy the translated output.

- 🎨 **Modern Responsive UI**
  - Dark AI-themed interface with a clean and responsive design.

- 📊 **Translation Pipeline**
  - Visually demonstrates each stage of the translation process.

---

## 🧠 How It Works

### 1. User Input

The user provides input either by typing text or speaking through the microphone.

### 2. Speech-to-Text

For voice input, the browser's Speech Recognition API converts speech into text.

### 3. Language Processing

The application processes the input text and selected source and target languages.

### 4. Machine Translation

The input text is sent to a machine translation service, which generates the translated text.

### 5. Translated Output

The translated sentence is displayed on the webpage.

### 6. Text-to-Speech

The translated text can be converted into spoken audio using the browser's SpeechSynthesis API.

---

## 🔄 System Architecture

```text
              USER
                │
        ┌───────┴────────┐
        │                │
      TEXT             VOICE
        │                │
        │          Speech-to-Text
        │                │
        └───────┬────────┘
                │
                ▼
       Language Processing
                │
                ▼
       Machine Translation
                │
                ▼
        Translated Text
                │
                ▼
        Text-to-Speech
                │
                ▼
             🔊 AUDIO

🔬 Detailed Process
1. User Input

The user can provide input in two ways:

Type a sentence into the text box.
Speak through the microphone.

Example:

What are you doing?
2. Speech-to-Text

If the user speaks, the browser's Speech Recognition API captures the speech and converts it into text.

Voice Input
     ↓
Speech Recognition
     ↓
"What are you doing?"
3. Language Processing

The application processes the input text along with the selected source and target languages.

For example:

Source Language → English
Target Language → Telugu
4. Machine Translation

The source text is sent to a machine translation service.

What are you doing?
          ↓
  Machine Translation
          ↓
మీరు ఏమి చేస్తున్నారు?

This is the main translation component of the application.

5. Translated Output

The translated text is displayed on the webpage.

Source:
What are you doing?

Target:
మీరు ఏమి చేస్తున్నారు?
6. Text-to-Speech

The translated text can then be converted into spoken output using the browser's SpeechSynthesis API.

మీరు ఏమి చేస్తున్నారు?
          ↓
   Text-to-Speech
          ↓
        🔊 Audio

If a suitable target-language voice is not available on the device, the application displays an appropriate notification instead of using an unrelated voice.

🛠️ Technologies Used
Frontend
HTML5
CSS3
JavaScript ES6
Web APIs
Web Speech Recognition API
SpeechSynthesis API
Development Tools
Vite
Git
GitHub
Google Antigravity
AI / NLP Concepts
Machine Translation
Neural Machine Translation (NMT)
Natural Language Processing
Speech Processing
Speech-to-Text
Text-to-Speech
🖥️ Project Structure
AI-Voice-Text-Translator/
│
├── index.html
├── package.json
├── vite.config.js
│
├── src/
│   ├── css/
│   │   ├── main.css
│   │   └── pipeline.css
│   │
│   └── js/
│       ├── app.js
│       ├── languages.js
│       └── UI.js
│
└── README.md
🌍 Example
English → Telugu
Input
What are you doing?
Output
మీరు ఏమి చేస్తున్నారు?
Telugu → English
Input
మీరు ఏమి చేస్తున్నారు?
Output
What are you doing?
English → Hindi
Input
Where are you going?
Output
आप कहाँ जा रहे हैं?
🎯 Real-World Problem

People around the world speak different languages, creating communication barriers in:

Education
Healthcare
Travel
Business
Tourism
International communication

A real-time translation system can help people communicate across different languages.

🤖 How AI Helps

AI-based machine translation can analyze text in one language and generate an equivalent meaning in another language.

Speech processing allows spoken language to be converted into text, while Text-to-Speech allows translated text to be converted back into speech.

Therefore, the system combines:

Speech Processing
        +
Natural Language Processing
        +
Machine Translation
        +
Text-to-Speech
📊 Data Required

A machine translation system generally requires multilingual language data such as:

Parallel text datasets
Sentence pairs between languages
Vocabulary
Language rules and patterns
Speech/audio data for speech recognition systems

For this prototype, the actual translation is handled by the integrated machine translation service, while browser APIs are used for speech recognition and speech synthesis.

🌎 Real-World Application

A well-known real-world application of these technologies is Google Translate, which provides multilingual text and speech translation.

This project demonstrates a simplified educational version of the same overall concept:

Input
  ↓
Speech Processing
  ↓
Language Processing
  ↓
Machine Translation
  ↓
Translated Output
  ↓
Speech Output
💡 Benefits
Reduces language barriers
Supports both voice and text
Provides quick translation
Easy-to-use interface
Useful for multilingual communication
Demonstrates practical AI application
Can be extended to additional languages
⚠️ Limitations
Speech recognition accuracy can vary with pronunciation and background noise.
Translation quality depends on the underlying translation service.
Internet connectivity may be required for external translation services.
Text-to-Speech availability depends on the voices provided by the user's browser/device.
Some languages may not have suitable native voices available on every device.
Machine translation may not always preserve cultural context or exact meaning.
🔮 Future Enhancements

Future versions could include:

Automatic language detection
More language support
Conversation mode
Translation history
Offline translation
Mobile application
Improved speech recognition
Improved neural speech synthesis
Real-time conversation translation
Voice-to-voice translation
🎓 Academic Objective

The objective of this project is to demonstrate the practical application of Artificial Intelligence in Language and Translation, specifically:

Machine Translation
Speech Processing
Natural Language Processing
Speech-to-Text
Text-to-Speech

The prototype demonstrates how these technologies can work together to solve a real-world communication problem.

⭐ Project Summary

The AI Voice & Text Translator is a web-based AI prototype that combines speech processing and machine translation.

The complete workflow is:

🎤 Voice / ⌨️ Text
        ↓
📝 Speech-to-Text
        ↓
🧠 Language Processing
        ↓
🌐 Machine Translation
        ↓
📄 Translated Text
        ↓
🔊 Text-to-Speech

The goal is to demonstrate how AI can help bridge language barriers and enable easier communication between people who speak different languages.

👩‍💻 Author
Deekshita Gandham
B.Tech – Computer Science Engineering
AI/ML Track
