---
title: "On the Maximum Hessian Eigenvalue and Generalization"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jeremy Cohen
- Zachary Lipton

# Author notes (optional)

date: "2022-05-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).


# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent

# Publication name and optional abbreviated publication name.
publication: Preprint

abstract: The mechanisms by which certain training interventions, such as increasing learning rates and applying batch normalization, improve the generalization of deep networks remains a mystery. Prior works have speculated that “flatter” solutions generalize better than “sharper” solutions to unseen data, motivating several metrics for measuring flatness (particularly $\lambda_{max}$, the largest eigenvalue of the Hessian of the loss); and algorithms, such as Sharpness-Aware Minimization (SAM) [1], that directly optimize for flatness. Other works question the link between $\lambda_{max}$ and generalization. In this paper, we present findings that call $\lambda_{max}$’s influence on generalization further into question. We show that (1) while larger learning rates reduce $\lambda_{max}$ for all batch sizes, generalization benefits sometimes vanish at larger batch sizes; (2) by scaling batch size and learning rate simultaneously, we can change $\lambda_{max}$ without affecting generalization; (3) while SAM produces smaller $\lambda_{max}$ for all batch sizes, generalization benefits (also) vanish with larger batch sizes; (4) for dropout, excessively high dropout probabilities can degrade generalization, even as they promote smaller $\lambda_{max}$; and (5) while batch-normalization does not consistently produce smaller $\lambda_{max}$, it nevertheless confers generalization benefits. While our experiments affirm the generalization benefits of large learning rates and SAM for minibatch SGD, the GD-SGD discrepancy demonstrates limits to $\lambda_{max}$’s ability to explain generalization in neural networks.

# Summary. An optional shortened abstract.
summary: ' '

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: pdf
   url: https://arxiv.org/pdf/2206.10654.pdf
 - name: arXiv
   url: https://arxiv.org/abs/2206.10654

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
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
---
