# Chatbot Deployment with Flask and JavaScript

In this tutorial we deploy the chatbot I created in [this](https://github.com/python-engineer/pytorch-chatbot) tutorial with Flask and JavaScript.

This gives 2 deployment options:

- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## ⚙️ Initial Setup:

This repo currently contains the starter files.

### Clone repo and create a virtual environment

```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```

### Install dependencies

```
$ (venv) pip install Flask torch torchvision nltk
```

### Install nltk package

```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```

Modify `intents.json` with different intents and responses for your Chatbot

### Run

```
$ (venv) python train.py
```

This will dump data.pth file. And then run
the following command to test it in the console.

```
$ (venv) python chat.py
```

Now for deployment follow my tutorial to implement `app.py` and `app.js`.

## 🔗 Live URL: <a href="https://searchdev-vuxm.onrender.com">🤖 Flask Chatbot using PyTorch 💬</a>

[![Render Status](https://api.netlify.com/api/v1/badges/1c7a3caa-d0f7-4e66-af82-49c8f6b5eed3/deploy-status)](https://app.netlify.com/sites/pymovie-joao/deploys)

## 📌 Tech Stack

[![HTML](https://img.shields.io/badge/html5%20-%23E34F26.svg?&style=for-the-badge&logo=html5&logoColor=white)](https://github.com/joao82)&nbsp;
[![CSS](https://img.shields.io/badge/css3%20-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white)](https://github.com/joao82)&nbsp;
[![JAVASCRIPT](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://github.com/joao82)&nbsp;
[![PYTHON](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/joao82)&nbsp;
[![FLASK](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://github.com/joao82)&nbsp;

<br>

## 📸 Overview

![Screenshot](./static/images/chatbot.gif?raw=true "Chatbot App")

## Watch the Tutorial

[![Alt text](https://img.youtube.com/vi/a37BL0stIuM/hqdefault.jpg)](https://youtu.be/a37BL0stIuM)

## ✏️ Note

In the video we implement the first approach using jinja2 templates within our Flask app. Only slight modifications are needed to run the frontend separately. I put the final frontend code for a standalone frontend application in the [standalone-frontend](/standalone-frontend) folder.

## 📌 Acknowledgments

- Course Instructor - [Hitch Cliff](https://github.com/hitchcliff/front-end-chatjs)
