# Chatbot Deployment with Flask and NLP ML

I have build a chatbot for college which is extrcated a data from college website from snjb.org
## Initial Setup:
app.py 
first install flask
then NLP librarie for lemmatization, stemming and remove stop words
then used a DL Models : Sequential
for static Questions stored data in intent.json

Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```

Now for deployment follow my tutorial to implement `app.py` and `app.js`.
