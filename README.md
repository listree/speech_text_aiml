# AI/MI for speech to text
### Requirement from TradeBees

Given a MP3 (or others) audio file with word reading (Chinese and English), the program can 
identify each word with Time offset (timestamp) values in the response text for your recognize request. 
Time offset values show the beginning and end of each spoken word that is recognized 
in the supplied audio.

The program must output words with timestamp in a sequence.  

### Instructions to use Google Speech
Install Library: pip3 install google-cloud-speech

Convert MP3: visit https://www.zamzar.com/convert/mp3-to-flac/

Upload File: https://console.cloud.google.com/storage/browser

Set Credential: export GOOGLE_APPLICATION_CREDENTIALS="gcp_credentials.json" 

Run Script: python3 measure.py --storage_uri "gs://tradebees/John-62-1.flac" > John-62-1.output

Check output: cat John-62-1.output

### References:

https://towardsdatascience.com/how-to-use-google-speech-to-text-api-to-transcribe-long-audio-files-1c886f4eb3e9

https://cloud.google.com/speech-to-text/docs/async-time-offsets

https://www.google.com/intl/en/chrome/demos/speech.html

https://speechnotes.co/

https://dictation.io/speech
