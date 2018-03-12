+++
title = "Knowledge Distillation (using Tensorflow)"
date = "2018-03-12"

summary = "Training a smaller neural model using soft targets obtained from a larger model"

tags = ["machine-learning", "natural-language-processing", "deep-learning"]

image_preview = "kdscores.png"


# Links (optional).
url_pdf = ""
url_preprint = ""
url_code = "https://github.com/DushyantaDhyani/kdtf"
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

url_custom = []

# Does the content use math formatting?
math = true

# Does the content use source code highlighting?
highlight = true

+++

This is an implementation for the basic idea behind Hinton's Knowledge Distillation Paper. We do not reproduce the exact results but rather show that the idea works.

While a few other implementations are available, the code flow is not very intuitive. Here we generate the soft targets from the teacher in an on-line manner while training the student network.

While this may not (or may) be a good way to implement the distillation architecture, it leads to a good improvement in the (small) student model.