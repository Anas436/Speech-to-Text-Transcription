# Speech-to-Text-Transcription

``
A Speech-to-Text Transcription App in Python using the AssemblyAI API. In brief, AssemblyAI is a speech-to-text API that I have used for transcribing YouTube videos that we will download via the pytube Python library. Finally, I have deployed this as a command line tool and a web app using argparse and Streamlit, respectively.
``

![](https://github.com/Anas436/Speech-to-Text-Transcription/blob/main/demo.png)

# 1. Obtain the AssemblyAI API key

Obtain your free [AssemblyAI API key](https://www.assemblyai.com/?utm_source=youtube&utm_medium=social&utm_campaign=dataprofessor).

# 2. Running transcriber as command line tool

Firstly, copy and paste the AssemblyAI API key into the `api.txt` file (you can replace the text `replace_with_your_AssemblyAI_API_key` with your own API key).

Secondly, install prerequisite `pytube` library by typing the following:
```
pip3 install pytube
```

Thirdly, run the transcriber by typing the following (note that you can replace the URL with a YouTube video of your choice):
```
python3 transcriber.py -i "https://youtu.be/mkVjrB8g6mM"
```

# 3. Running transcriber as a Streamlit app
To recreate this web app on your own computer, do the following.

### Create conda environment (Optional)
Firstly, we will create a conda environment called *transcriber*
```
conda create -n transcriber python=3.7.9
```
Secondly, we will login to the *transcriber* environment
```
conda activate transcriber
```

###  Download GitHub repo

```
git clone https://github.com/Anas436/Speech-to-Text-Transcription
```

###  Pip install libraries
```
pip install -r requirements.txt
```

###  Launch the app

```
streamlit run app.py
```
