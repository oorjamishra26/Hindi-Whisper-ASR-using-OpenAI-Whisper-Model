# **Hindi Whisper ASR using OpenAI Whisper Model**

**Project Description:**

The code provided is part of a project aimed at transcribing Hindi audio data using machine learning models. The test audio (uploaded above) is one of the randomly selected hindi audio from kathbath dataset. Here's a brief overview of what the code accomplishes:

The project utilizes various Python libraries and tools to process audio data, convert it to text, and evaluate the accuracy of the transcription.

1. **Dependencies Installation:**
   - The code begins by installing necessary Python libraries such as `pyloudnorm`, `pydub`, `whisper`, `jiwer`, and mounts Google Drive to access data.

2. **Audio Data Processing:**
   - The code imports essential libraries for audio processing such as `numpy`, `matplotlib`, `librosa`, and `pydub`.
   - It defines functions to convert audio files from WAV to MP3 format, demonstrating usage of the `pydub` library.

3. **Loading Models:**
   - The `whisper` library is used to load a pre-trained machine learning model (`model_medium`) for transcribing audio. This model is specifically trained for medium-scale transcription tasks.

4. **Transcription Process:**
   - An audio file (`audioPathHindi`) is loaded from a specified directory and converted to MP3 format using `pydub`.
   - The transcribed audio is processed using the `whisper` library to pad or trim it to a fixed length.
   - The script then utilizes the `model_medium` to transcribe the audio into text, detecting the spoken language (in this case, Hindi).
   - The transcribed text is printed out.

5. **Evaluation:**
   - The code calculates the Word Error Rate (WER) between the actual ground truth text and the transcribed text using the `jiwer` library. This metric helps assess the accuracy of the transcription process.

6. **Result Output:**
   - The calculated WER percentage is printed out, providing insight into the accuracy of the transcription.
   - Additionally, the transcribed text is printed out to display the result of the transcription process.

**Note:** This README provides an overview of the code's functionality and purpose, focusing on the audio transcription process and evaluation. Additional details such as project usage, specific dependencies, and project context may be included in a complete project documentation.
