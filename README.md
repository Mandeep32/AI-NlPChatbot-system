AI-NLP-Chatbot
An NLP based Chatbot over a simple fully connected neural network architecture using Tensorflow and tflearn. Trained over a custom dataset specified in the JSON file.

Prerequisites
Run pip install -r requirements.txt in your terminal to install all required libraries

Dataset
The dataset.json contains the intents on which the model is trained. Each pattern (sentence) and response is given a particular tag. The model classifies each input sentence under a tag and gives out a random answer corresponding to that tag. The json file can be formatted according to the user's requirements.

PyAudio
In Python versions above 3.6 PyAudio is not a supported library and installing PyAudio directly using
pip install pyaudio fails and needs to be installed separately.

Windows
For that, individually install the wheel file given (this is for Python 3.7, find suitable wheel files here) writing the following line in your terminal.
pip  install <.wh file name>

Ubuntu/Linux
$ sudo apt-get install python3-pyaudio

Execute Code
Run trainModel.py to train the Fully Connected Network on the dataset. You can change the number of epochs or layers accordingly, the current architecture gave good results with a ~95% accuracy on predicting tags.

Run textChatbot.py for text based chatbot with GUI incorporated

Run voiceBot.py for voice recognition based chatbot
