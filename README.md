# Senticomment
Senticomment is a simple little hacked together script that applies basic sentiment analysis to downloaded YouTube comments. To set up:

## Installation of Libraries


It's recommended that you use [virtualenv](http://docs.python-guide.org/en/latest/dev/virtualenvs/) so that existing packages aren't tempered with.
You'll need Python 3 installed with pip. Run:

`pip install httplib2`

`pip install nltk`

`pip install csv`

`pip install google-api-python-client`

`pip install oauth2client`

You'll also need to install `vader`.

Just go into the python console, import `nltk` module and use it to download the vader data.

`import nltk`

`nltk.download('vader_lexicon')`

## Set Up Google Cloud
1. Go to [Google Cloud Console](https://console.cloud.google.com) and create a new project. 
2. Enable the YouTube Data API v3.
3. Create credentials (OAuth client ID, Application Type: Other) and download them to `client_secrets.json`.

## Running the Code
Run `python3 main.py --videoid={your video ID here}` to run the script and generate a CSV file.

## Examples
`python3 main.py --videoid=Zj8h3ZSc-Aw`

[Link to Interactive Histogram as of June 11, 2018](https://docs.google.com/a/college.harvard.edu/spreadsheets/d/e/2PACX-1vRXt_ciTLw3Ylp7_PqHQqOHS8rh-hiGAqA9i7BhbsrDvHuoyBWflibParlm6h9IpewF0CFQc6bTHHcx/pubchart?oid=1509344064&format=interactive)
