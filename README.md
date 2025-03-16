# audio-enhancer-transcription
Audio Enhancer AI optimizes audio quality and reduces noise to achieve the most accurate speech transcription possible. Using deep learning and OpenAI's Whisper, it enhances transcription fidelity, making it ideal for processing voice recordings in noisy environments.
#  Audio Enhancer & Transcriptor

##  Introduction

**Audio Enhancer & Transcriptor** is an advanced audio post-processing system designed to improve sound quality, reduce background noise, and achieve the most accurate speech transcription possible using **OpenAI's Whisper**.

This tool is ideal for those working with **podcasts, voice recordings, interviews, and automatic transcriptions**, ensuring enhanced audio quality and more precise speech-to-text conversion.

##  Objectives

- **Improve audio quality** by eliminating background noise and artifacts.
- **Obtain more accurate transcriptions** from voice recordings.
- **Automate the process** for a simple and efficient workflow.
- **Facilitate usage through a Jupyter Notebook interface**.

##  Requirements

Before using the project, ensure you have installed:

- **Python 3.8+**
- **Required libraries** (listed in `requirements.txt`)
- **OpenAI's Whisper model**
- **FFmpeg** (for handling audio files, installable via `apt-get install ffmpeg` or `brew install ffmpeg` on macOS)

##  Installation

Clone the repository and install the required dependencies:

```sh
# Clone the repository
git clone https://github.com/your-username/audio-enhancer-transcriptor.git
cd audio-enhancer-transcriptor

# Install dependencies
pip install -r requirements.txt
```

If you want to use Jupyter Notebook for interactive testing:

```sh
pip install notebook
jupyter notebook
```

##  Project Structure

```bash
📂 audio-enhancer-transcriptor
│── 📂 src                # Source code
│   │── enhance_audio.py  # Script for audio enhancement
│   │── transcribe.py     # Script for transcription
│── 📂 data               # Sample audio files
│── 📂 notebooks          # Jupyter Notebook for testing and demo
│── 📜 README.md          # Project documentation
│── 📜 requirements.txt   # Dependencies
│── 📜 LICENSE            # Open-source license
│── 📜 .gitignore         # Files to exclude
```

## 🎙 Processing Flow

The following diagram illustrates the audio processing flow within the project:



1. **Input Audio** - The original audio file is loaded.
2. **Noise Reduction** - A filter is applied to reduce background noise.
3. **Enhanced Audio** - A file with improved quality is obtained.
4. **Whisper Transcription** - The enhanced audio is processed with Whisper to generate a transcription.
5. **Final Transcript** - A text file with the most accurate transcription is obtained.

## 🎙 Execution

### 1️⃣ **Audio Enhancement**

To enhance an audio file and reduce background noise:

```sh
python src/enhance_audio.py --input data/audio.wav --output data/enhanced.wav
```

### 2️⃣ **Transcription with Whisper**

To transcribe an enhanced audio file:

```sh
python src/transcribe.py --input data/enhanced.wav
```

## 📄 License

This project is distributed under the **MIT License**.

---

📌 **Note:** If you need additional details or want to improve the README with more specific images/examples, feel free to suggest updates! 🚀
