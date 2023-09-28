**# smartSense_Assignment2**

Problem Statement: 
Train a model to summarize and extract key points from the podcast.

**APPROACH**

Three podcasts were given to me in mp3 format, and I had to initially try to read the file and convert it into wav format so as to easily convert into a txt file

Here, I faced the issue in the first step of reading through the mp3 as my laptop got stuck and also even after multiple tries using multiple methods the file was not found.
So I couldn't go forward with coding down the rest of the solution as the code was continuously resulting in error and this could be because the mp3 has some problem, I have also added a the code I used with which even now I am getting error in reading the file

```python
import speech_recognition as sr
import soundfile as sf
import os
mp3_file = "C:\\Users\\madha\\OneDrive\\Desktop\\LLM\\VMP4732384152.mp3"

try:
    audio, sample_rate = sf.read(mp3_file)
    print("Audio data loaded successfully.")
except Exception as e:
    print(f"Error loading audio: {e}")

from pydub import AudioSegment


mp3_file = "C:\\Users\\madha\\OneDrive\\Desktop\\LLM\\VMP4732384152.mp3"
wav_file = "C:\\Users\\madha\\OneDrive\\Desktop\\LLM\\voice.wav"  # Output WAV file path

# Convert the MP3 file to WAV format using pydub
audio = AudioSegment.from_mp3(mp3_file)
audio
```
This was constantly giving errors
