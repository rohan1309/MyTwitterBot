<h1>SpeakAndTweet</h1>
A command line utility that can be used to tweet an input from microphone. You'll never have to type again.!!!
<hr>

<h3>Requirements</h3><p><b>(As of now, the instruction set added is only for Ubuntu 14.04 and higher)</b></p>
To use all of the functionality of the library, you should have:
    
    Python 2.6, 2.7, or 3.3+ (required)
    PyAudio 0.2.11+ (required only if you need to use microphone input, Microphone)
    PocketSphinx (required only if you need to use the Sphinx recognizer, recognizer_instance.recognize_sphinx)
    Google API Client Library for Python (required only if you need to use the Google Cloud Speech API, recognizer_instance.recognize_google_cloud)
    FLAC encoder (required only if the system is not x86-based Windows/Linux/OS X)


<h4>Commands to run</h4>

    (required)sudo apt-get install python-pip (installs latest version of pip)
    (required)sudo apt-get install portaudio-dev  (installs developer tools forportaudio)
    (required)sudo apt-get install libasound-dev  (installs ALSA libraries)
    (required)sudo pip install twython  (installs twitter's twython API)
    (required)sudo pip install google-api-python-client
    (required)sudo pip install google-cloud
    (optional)sudo pip install speech_recognition    

<b>Note</b>-To correctly upgrade/install PyAudio, download and extract the 0.2.11 version from here http://www.portaudio.com/download.html
and run the following set of commands from inside the portaudio directory

    ./configure && make
    sudo make install
    sudo pip install pyaudio --upgrade (run this only if you have an older version of pyaudio)
    
<h4>Twitter Setup</h4>
     You need a valid twitter account to tweet and need to implement the following steps from your account.
     
     1) Go to https://apps.twitter.com
     2) Create a new app and generate your Consumer Key, Consumer Secret, Access token and Access token secret and replace these values under TwitterBot/letsTweet.py
     3) Save the changes.

<b>Note</b>-Tweets cannot be duplicated.

For language changes and other settings in speech to text conversions, view https://github.com/Uberi/speech_recognition/blob/master/reference/library-reference.rst
<br>
<h6>Finally, execute the letsTweet.py under MyTwitterBot/TwitterBot using command "python letsTweet.py".</h6>
<b><i>P.S.</b> Remember to say 'exit' if you want to quit without tweeting</i>
     
