---
title: Optimal Service Rate Control Considering Patients’ Retrial
summary: We built a 2-dimensional queueing model to simulate such a circumstance, after treatment at the hospital, there is a certain probability that the patient will go back to the hospital for treatment. Under the long-run cost, we investigated how to optimally control the service rate of the hospital to minimize the overall cost.
# tags:
#   - Deep Learning
date: '2022-06-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: 1-page slide
  focal_point: Smart

url_code: 'https://github.com/fuyuyun99/Optimal-control/blob/main/MDP.Rmd'
url_pdf: 'https://github.com/fuyuyun99/Optimal-control/blob/main/slides(in%20Chinese).pdf'
url_slides: ''
url_video: 'https://www.bilibili.com/video/BV17s4y1Q7AE/?spm_id_from=333.999.0.0&vd_source=d41be1ecc37e7751c802a57b1f9793cd'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
We considered such a circumstance: patients come to the hospital for treatment with rate $\lambda$. There is only one server and first-come-first-served in the ordinary queue. This server serves at two different rates $\mu_h$ and $\mu_h$, wich can be dynamically adjusted based on the on-site situation. However, if the treatment is unsuccessful, patients have a probability of entering an orbit queue and each patient in the orbit queue will go back to the ordinary queue with rate $\lambda$ independently. 

In this model, cost happens in three places: a waiting cost $h$ for each patient in the ordinary queue, service cost rate $c_h$ or $c_l$ and a penalty cost $c_p$ for each entry into the orbit queue. 














