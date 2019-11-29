# Topic Modelling with LDA
The objective of this project is to explore topic modelling of text data gathered from TrustPilot about train service in Great Britain. The data is a small assortment of roughly 2,000 reviews. In this context a simple model for the topics is constructed using Latent Dirchelet Allocation, and then visualized with t-SNE. Comments are provided at the end of the notebook about further avenues for exploration.

## Setup
To setup and explore the content of this project simply set up a new Python 3.7 virtual environment and install a the requirements specified in the `requirements.txt` file. For example:
```
$ virtualenv --no-site-packages myvenv
$ source myvenv/bin/activate
$ pip3 install -r requirements.txt
```

## Contents
`lda_topic_identification.ipynb` contains the data exploration and topic modelling work.

`train_reviews.json` contains JSON blobs of individual train reviews, with fields:
* `date`: ISO format date and time of the review.
* `stars`: "Star" rating; between 1-5 plus extraneous information.
* `title`: User made title for their review.
* `text`: User review.
* `url`: URL at which the review is referenced by TrustPilot.