---
title: "Gradient Descent on Neural Networks Typically Occurs at the Edge of Stability" 

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Jeremy Cohen
- admin
- Yuanzhi Li
- Zico Kolter
- Ameet Talwalker

# Author notes (optional)

date: "2021-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).


# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent

# Publication name and optional abbreviated publication name.
publication: Published as a conference paper at ICLR 2021

abstract: We empirically demonstrate that full-batch gradient descent on neural network training objectives typically operates in a regime we call the Edge of Stability. In this regime, the maximum eigenvalue of the training loss Hessian hovers just above the numerical value 2/(step size), and the training loss behaves non-monotonically over short timescales, yet consistently decreases over long timescales. Since this behavior is inconsistent with several widespread presumptions in the field of optimization, our findings raise questions as to whether these presumptions are relevant to neural network training. We hope that our findings will inspire future efforts aimed at rigorously understanding optimization at the Edge of Stability.


# Summary. An optional shortened abstract.

tags: [Published as a conference paper at ICLR 2021]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: pdf
   url: https://arxiv.org/pdf/2103.00065.pdf
 - name: arXiv
   url: https://arxiv.org/abs/2103.00065 

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
---
