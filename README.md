# AI Doctor 2.0: Medical Chatbot with MultiModal LLM

**AI Doctor 2.0** is an advanced medical assistant project that integrates **Vision and Voice** capabilities to create an interactive diagnostic experience. Using a MultiModal Large Language Model (LLM), this system can analyze medical images and communicate with patients via speech-to-text and text-to-speech technologies.

---

## 🚀 Key Features

* 
**Multimodal Analysis:** Analyzes medical images (e.g., skin conditions) using Llama 3/4 Vision models.


* 
**Voice Interaction:** Patients can record their symptoms, which are transcribed into text using OpenAI Whisper.


* **Persona-Driven Responses:** The "Doctor" responds in a professional, concise manner, providing differentials and remedies without technical jargon.
* 
**Audio Feedback:** Converts the AI's medical advice back into speech using high-quality voices from ElevenLabs or gTTS.



---

## 🛠️ Tools and Technologies

The project is built using a modern AI stack optimized for performance and open-source flexibility:

| Category | Technology Used |
| --- | --- |
| **Inference Engine** | <br>**Groq** (for fast AI response times) 

 |
| **Vision Model** | **Llama 4 Scout** (via Groq) |
| **Speech-to-Text** | <br>**OpenAI Whisper-large-v3** 

 |
| **Text-to-Speech** | <br>**ElevenLabs** & **gTTS** 

 |
| **UI Framework** | <br>**Gradio** 

 |
| **Language** | <br>**Python** 

 |

---

## 🏗️ Technical Architecture

The project is divided into four distinct phases:

1. 
**Phase 1: The Brain:** Setting up the Multimodal LLM (Llama 4) and image encoding (Base64) to process visual data.


2. 
**Phase 2: Patient's Voice:** Capturing audio through a microphone and transcribing it using Whisper-large-v3.


3. 
**Phase 3: Doctor's Voice:** Implementing text-to-speech logic to provide vocalized medical advice.


4. 
**Phase 4: The Interface:** Bundling all components into a user-friendly Gradio web application.



---

## 📂 Project Structure

* **`gradio_app.py`**: The main entry point that launches the web UI and orchestrates the data flow between voice and vision modules.
* **`brain_of_the_doctor.py`**: Handles image conversion and interaction with the Groq-hosted Llama models.
* **`voice_of_the_patient.py`**: Contains logic for audio recording and transcription.
* **`voice_of_the_doctor.py`**: Manages the conversion of text responses into playable audio files.
* 
**`requirements.txt`**: Lists all necessary Python dependencies, including `groq`, `elevenlabs`, `gradio`, and `speechrecognition` .



---

## 🔧 Setup and Installation

1. 
**Prerequisites:** Ensure you have Python 3.10+ and `ffmpeg` installed on your system .


2. **Environment Variables:** Create a `.env` file and add your API keys:
* `GROQ_API_KEY`
* `ELEVEN_API_KEY`


3. **Install Dependencies:**
```bash
pip install -r requirements.txt

```


4. **Run the App:**
```bash
python gradio_app.py

```



---

## 📈 Future Potential

* 
**Advanced Models:** Transitioning to state-of-the-art paid vision models for higher diagnostic accuracy.


* 
**Fine-tuning:** Training the vision model specifically on medical datasets to improve specialized image recognition.


* 



Would you like me to help you draft a specific **system prompt** for a different medical specialty, such as dermatology or pediatrics?
