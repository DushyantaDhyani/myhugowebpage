+++
title = "Event & Participant Extraction from News Articles (Automatic Timeline Generation of News Events)"
date = "2018-01-08"

summary = "Extract events in News articles and their participants using a conditional random field classifier and extensive feature engineering"

tags = ["machine-learning", "natural-language-processing"]

image_preview = "ukp_timeline_gen.png"


# Links (optional).
url_pdf = "/files/ukpreport.pdf"
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = "https://www.ukp.tu-darmstadt.de/research/past-projects/structuring-story-chains/"
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

url_custom = [{name = "Dataset ECB+", url = "http://www.newsreader-project.eu/results/data/the-ecb-corpus/"}, {name = "Dataset TimeML", url = "http://www.timeml.org/timebank/timebank.html"}]

# Does the content use math formatting?
math = true

# Does the content use source code highlighting?
highlight = true

+++

The larger aim of the project is to create a chronological ordering of important sub-events (and their participants) involved in a bigger event. I worked on the task of creating a strong baseline model for identifying important events in news articles and their associated participants. We used articles from the ECB+ Corpus and Timebank Corpus. We performed extensive feature engineering using syntactic and semantic features that were then used with a CRF Classifier to achieve the following F-1 scores:

- Event Extraction
	- ECB+ Corpus \- 73.02 %  
	- TimeBank Corpus \- 80.78% 

- Participants 
	- ECB+ Corpus \- 56.51%