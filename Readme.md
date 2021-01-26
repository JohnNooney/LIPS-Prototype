# LIPS Prototype
This app's main function is to aid those with hearing impariments, and who rely on lip reading, to communicate effectively with those wearing a mask. Overall, this is a proof of concept and will be developed further as time goes on. 

This application is made in Unity and allows the user to speak into their computer's microphone which will then detect what the user is saying and relay that into a text transcript on the screen, all the while matching the phoenetic's and mouth models to the words. All of this coming together simulates the mouth movements of the user as they talk.

## Pre-requisites
You must have the windows 10 speech recognition turned on in order for this to detect your voice

Steps:
1. Select the Start button, then select Settings  > Time & Language > Speech.
2. Under Microphone, select the Get started button.

## Features
As of right now:
- speech to text through windows voice recognition engine
- text to phoenetic matching
- phoenetic to mouth model matching
- Chached data of the most common words in order to reduce searches for phonics matching
- web scraping from the https://dictionary.cambridge.org/ to get the phonics of the word if not found in cache

## Future Improvements
- Replace windows 10 speech recognition relibality with VOSK Speech-to-Text API
- Convert unity microphone clips into WAV format to communicate with API
- Create WebSocket Service to manage the incoming and outgoing data
  - outgoing: WAV files to API
  - incoming: Text transcript of WAV files
- User login and logout
- WebGL will be utilized to turn this into a web application
