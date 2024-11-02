
# Pronunciation Assistant
The Pronunciation Assistant is a desktop application built to assist users in improving their pronunciation skills. Leveraging deep learning for speech recognition and object detection, along with natural language processing and text-to-speech features, this tool provides feedback on pronunciation, word meaning, and translations. 

## Features
- Speech Recognition: Uses Wav2Vec2 from the `transformers` library for accurate, real-time speech recognition.
- Pronunciation Feedback: Provides feedback on pronunciation accuracy to help users improve.
- Translation: Includes Google Translate integration to offer word translations.
- Text-to-Speech: Uses Google Text-to-Speech (`gTTS`) to play correct pronunciations.
- Object Detection: YOLO model integration for identifying objects based on user speech input.

## Getting Started

### Prerequisites
- Python 3.7+
- Libraries:
  - `transformers`
  - `speech_recognition`
  - `gTTS`
  - `nltk`
  - `torch`
  - `yolov5`
  - `tkinter` (for GUI)

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/pronunciation-assistant.git
   cd pronunciation-assistant
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python3 -m venv pronunciation_env
   source pronunciation_env/bin/activate
   ```

3. **Install Required Libraries**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Download Pretrained Models**:
   - **Wav2Vec2**: Download the pretrained Wav2Vec2 model from `transformers`.
   - **YOLO**: Download the YOLOv5 weights for object detection.

5. **Download NLTK Data**:
   ```python
   import nltk
   nltk.download('all')
   ```

## Usage
1. **Record and Analyze**:
   - Click the 'Record' button to capture audio.
   - The tool will analyze your pronunciation and provide feedback.

2. **Get Translations**:
   - Input a word to get its meaning and translations in various languages.

3. **Object Detection**:
   - Speak a word describing an object, and the app will identify it if present in the camera’s field of view.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## Acknowledgments
- Hugging Face for Wav2Vec2 model
- YOLOv5 team for object detection
- Google Translate API for translation assistance
- Google Text-to-Speech for TTS functionality
- NLTK for natural language processing tools
