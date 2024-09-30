# MedVoice Avatar: Prescription to Speech with AI-Generated Avatars

### Description

**MedVoice Avatar** is an AI-powered application designed to convert medical prescriptions into lifelike speech using text-to-speech (TTS) models like Amazon Polly. This project also integrates with AI-generated avatars, allowing medical information to be presented in an interactive and engaging way. The tool currently supports creating videos where an avatar reads out the prescription text, making medical communication more accessible.

This project is a **work-in-progress** and is part of a **volunteer initiative** aimed at improving patient communication in healthcare settings through cutting-edge AI technologies.

---

### Key Features
- **Text-to-Speech (TTS)**: Converts prescription text into human-like speech using Amazon Polly.
- **Avatar Integration**: Avatars, generated using AI tools such as Artbreeder, are synced with audio output, providing a visual representation.
- **Prescription Processing**: Automatically processes medical prescription data and transforms it into spoken word.
- **Multiple Languages**: Currently supports English and Hindi, with the potential to expand to other languages.
- **User-Generated Avatars**: While we provide default avatars, users can also upload their custom avatars to personalize the output.

---

### Work in Progress
This project is under active development. Here are some of the upcoming features:
- **Character Limit Handling**: Amazon Polly has a limit of 3,000 characters per request. Currently working on strategies to combine audio files for longer prescriptions.
- **Further Avatar Customization**: Aim to improve avatar creation and make it a more seamless part of the pipeline without requiring external uploads.
- **Support for More Languages**: Expanding the TTS service to support more languages.
- **Performance Optimizations**: Currently, generating videos can take a significant amount of time. Working on optimizing this process to reduce the overall runtime.

---

### Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/medvoice-avatar.git
   cd medvoice-avatar
   
2. **Install Dependencies**:
   Use the following command to install the required Python libraries.

  ```bash
  pip install -r requirements.txt

3. **Set up Amazon Polly API**:
  To use Amazon Polly for TTS, ensure that you have the necessary access credentials. You can follow Amazon Polly’s setup guide [here](https://docs.aws.amazon.com/polly/).

4. **Run the Application**:
  Use the following command to process a prescription:

  ```bash
  python run.py --prescription_file prescription.txt --avatar avatar_image.jpeg

### How It Works
1. **Scan Prescription**: Upload a medical prescription in text form.
2. **TTS with Amazon Polly**: The text is processed by Amazon Polly, which converts the prescription text into speech.
3. **Avatar Creation**: The user can either upload a custom avatar or use a default AI-generated avatar.
4. **Video Generation**: The avatar is synchronized with the audio, and a video is generated showing the avatar reading out the prescription.

---

### Challenges
- **Amazon Polly Character Limit**: Amazon Polly has a character limit of 3,000 characters per request. To handle longer texts, we are working on splitting the text into chunks and combining the audio into one output.
- **Video Processing Time**: Video creation can take up to an hour depending on the avatar and audio length. Future updates will optimize this.

---

### To-Do List
- [ ] Improve avatar creation pipeline.
- [ ] Optimize video generation times.
- [ ] Add support for more languages.
- [ ] Handle longer prescriptions by combining smaller audio chunks.
- [ ] Incorporate feedback on avatar customization features.

---

### License
This project is licensed under the MIT License.
