# Speech_to_Speech_Language_Translator

# Problem Statement:

If we don’t know how to speak in any other country and we don’t understand their native language, then we can use this tool to overcome the problem. We can translate between all those languages which are present in google translator. We can Capture audio using the microphone and translate that audio into desired language, and get back audio output file.

#### Libraries used:
Requirements:
•	python==3.9
•	pip install googletrans ==3.1.0a0
•	pip install pyaudio
•	pip install SpeechRecognition
•	pip install gtts

•	googletrans: A Python library to interact with Google Translate API.
•	pyaudio: Provides Python bindings for PortAudio, which is used for audio input.
•	SpeechRecognition: Library for performing speech recognition.
•	gtts: Google Text-to-Speech, for converting text to speech.


#	Googletrans

1)	https://py-googletrans.readthedocs.io/en/latest/
2)	https://pypi.org/project/googletrans/
3)	https://www.geeksforgeeks.org/language-translator-using-google-api-in-python/ 

•	Googletrans is a free and unlimited python library that implemented Google Translate API. This uses the Google Translate Ajax API to make calls to such methods as detect and translate.
•	Google Translate Ajax API is part of Google APIs, designed for language detection and translation. 
•	Googletrans supports around 107 languages.
•	It can be utilized with Ajax and jQuery for translation services, though users have reported issues in the past .
•	The API returns detected language and confidence level or "error" in case of issues .
•	Developers can create translator applications using the Google AJAX API and JSON .
•	Additional tools like Googletrans, a Python library, implement the Google Translate Ajax API for free and unlimited translation calls .
•	The Google Translate Ajax API facilitates language detection and translation, commonly used in web development for multilingual applications.

Features:
•	Fast and reliable - it uses the same servers that translate.google.com uses
•	Auto language detection
•	Bulk translations
•	Customizable service URL
•	Connection pooling (the advantage of using requests.Session)
•	HTTP/2 support
•	Note on library usage
•	The maximum character limit on a single text is 15k.

#	Pyaudio: 

1) https://people.csail.mit.edu/hubert/pyaudio/docs/
2) https://pypi.org/project/PyAudio/

•	PyAudio provides Python bindings for PortAudio v19, the cross-platform audio I/O library. With PyAudio, you can easily use Python to play and record audio on a variety of platforms, such as GNU/Linux, Microsoft Windows, and Apple macOS.

# SpeechRecognition

1)	https://pypi.org/project/SpeechRecognition/
2)	https://www.geeksforgeeks.org/speech-recognition-in-python-using-google-speech-api/
3)	https://realpython.com/python-speech-recognition/

•	Library for performing speech recognition, with support for several engines and APIs, online and offline.
•	Speech Input Using a Microphone and Translation of Speech to Text: Allow Adjusting for Ambient Noise: Since the surrounding noise varies, we must allow the program a second or two to adjust the energy threshold of recording so it is adjusted according to the external noise level. Speech to text translation: This is done with the help of Google Speech Recognition. This requires an active internet connection to work. However, there are certain offline Recognition systems such as PocketSphinx, that have a very rigorous installation process that requires several dependencies. Google Speech Recognition is one of the easiest to use. You can now invoke recognize_google() to attempt to recognize(transcribe: audio to text) any speech in the audio. Depending on your internet connection speed, you may have to wait several seconds before seeing the result.
•	Recognizing speech requires audio input, and SpeechRecognition makes retrieving this input really easy. Instead of having to build scripts for accessing microphones and processing audio files from scratch, SpeechRecognition will have you up and running in just a few minutes.
•	The SpeechRecognition library acts as a wrapper for several popular speech APIs and is thus extremely flexible. One of these—the Google Web Speech API—supports a default API key that is hard-coded into the SpeechRecognition library. That means you can get off your feet without having to sign up for a service.
Requirements
•	Python 3.8+ (required).
•	PyAudio 0.2.11+ (required only if you need to use microphone input, Microphone).
•	PocketSphinx (required only if you need to use the Sphinx recognizer, recognizer_instance.recognize_sphinx)
•	Google API Client Library for Python (required only if you need to use the Google Cloud Speech API, recognizer_instance.recognize_google_cloud)
•	FLAC encoder (required only if the system is not x86-based Windows/Linux/OS X)
•	Vosk (required only if you need to use Vosk API speech recognition recognizer_instance.recognize_vosk)
•	Whisper (required only if you need to use Whisper recognizer_instance.recognize_whisper)
•	openai (required only if you need to use Whisper API speech recognition recognizer_instance.recognize_whisper_api)
•	The following requirements are optional, but can improve or extend functionality in some situations:If using CMU Sphinx, you may want to install additional language packs to support languages like International French or Mandarin Chinese.

#	Gtts:
1)	https://pypi.org/project/gTTS/
2)	https://gtts.readthedocs.io/en/latest/

•	gTTS (Google Text-to-Speech), a Python library and CLI tool to interface with Google Translate text-to-speech API
•	Write spoken mp3 data to a file, a file-like object (bytestring) for further audio manipulation, or stdout.It features flexible pre-processing and tokenizing.
•	Features:
•	Customizable speech-specific sentence tokenizer that allows for unlimited lengths of text to be read, all while keeping proper intonation, abbreviations, decimals and more;
•	Customizable text pre-processors which can, for example, provide pronunciation corrections;
