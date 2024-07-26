# QuickChatBot
A quick implementation of a intent chatbot


Clone repo and create a virtual environment
```
$ git clone https://github.com/ankur09011/QuickChatBot.git
$ cd QuickChatBot
$ python3 -m venv venv
$ . venv/bin/activate
```

Install dependencies

```
$ (venv) pip install Flask flask_cors torch torchvision nltk
```

## Note to intialise NLTK use externally, required only one time
```
import nltk
nltk.download('punkt')
```

Modify intents.json with different intents and responses for your Chatbot

```
$ (venv) python train.py
```

This will dump chat_model.pth file. And then run the flask app, it will host endpoint at 5555

```
$ (venv) python app.py
```

### Use frontend folder to test