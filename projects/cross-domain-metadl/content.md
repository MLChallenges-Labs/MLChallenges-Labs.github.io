## Competition Overview

Meta-learning aims to leverage experience from previous tasks to solve new tasks efficiently. Lately, meta-learning has contributed to making a lot of progress in few-shot learning for image classification problems. However, despite progress made, evaluation protocols have two common drawbacks:

- Even when evaluated on multiple domains (e.g., insect classification, texture classification, satellite images, etc.), models meta-trained on a given domain are meta-tested on the same domain (within domain few-shot learning).
- In the case of N-way k-shot problems, the number of ways N (number of classes) and shots k (number of training examples per class) is usually fixed.

This competition is part of the MetaDL Competition Series. Therefore, it is the continuation of our previous NeurIPS 2021 MetaDL Competition which tackled the within domain few-shot learning problem with a 5-ways 5-shots setting. The new Cross-Domain MetaDL competition is part of the NeurIPS 2022 Competition Track Program and is focused on cross-domain meta-learning for few-shot image classification using a novel "any-way" and "any-shot" setting. The goal of this competition is to meta-learn a good model that can quickly learn tasks from a variety of domains, with any number of classes also called "ways" (within the range 2-20) and any number of training examples per class also called "shots" (within the range 1-20). The novelties of Cross-Domain MetaDL with respect to the previous competition are as follows:

- **Protocol:** Still with code submission and one-chance blind testing on new datasets in the final phase. Closer to the real world scenario where the data may come from different domains (cross-domain) and not always with the same number of classes and examples per class (any-way any-shot setting).
- **Data:** We have extended the Meta-Album Dataset we started putting together last year. Therefore, in this competition, we use 30 datasets from 10 domains. They are all image classification datasets, with uniformly formatted 128x128 RGB images carefully resized with anti-aliasing filters.

## Prizes

This competition has a prize pool of €4000 distributed among 5 different leagues:

- **Participant of a rarely represented country league:** Be a participant of a group that is not in the top 10 most represented countries of Kaggle challenge participants.
- **Free-style league:** Submit a solution obeying basic challenge rules (pre-trained models allowed).
- **Meta-learning league:** Submit a solution that meta-learns from scratch (no pre-training allowed).
- **New-in-ML league:** Be a participant with less than 10 ML publications, none of which were ever accepted to the main track of a major conference.
- **Women league:** Special league to encourage women since they rarely enter challenges.

**NOTE:** For the leagues New-in-ML, Women, and Participant of a rarely represented country, in the case of teams, all team members must fulfill the specific requirements of the league to participate in it.

Entering multiple leagues is permitted. In addition, the top ranking participants will receive a certificate, and be invited to co-author a post-challenge analysis paper with the organizers, published in the NeurIPS proceedings of the competition track. Travel awards will also be distributed depending upon merit and needs to top ranking participants who want to attend NeurIPS in person, depending on availability.

## Competition Phases

- **Public phase (2 weeks):** The starting kit and 10 public datasets will be released for the participants to familiarize themselves with the problem and test their solutions on their computers or Google Colab.
- **Feedback phase (8 weeks):** Participants can use this CodaLab site to submit their solutions and receive feedback on the 10 hidden datasets. This CodaLab site is equipped with 10 identical computer workers. Each has the following configuration: 4 CPU cores, 1 Tesla T4 GPU, 16GB RAM, 120GB storage.
- **Final phase (4 weeks):** The last submission of each participant from the Feedback phase is blind-tested on 10 new hidden datasets to rank the participants and select the winners.

## Timeline

- **Jun 15, 2022:** Public phase starts.
- **Jul 1, 2022:** Feedback phase starts.
- **Sep 1, 2022:** Final phase starts.
- **Oct 1–15, 2022:** Notification of winners.

## Results

| League | Team | Average Normalized Accuracy | Prize |
|--------|------|-----------------------------|-------|
| Free-style | MetaBeyond | 0.699 ± 0.007 | 400 EUR |
| Free-style | EmmanuelPintelas | 0.682 ± 0.007 | 250 EUR |
| Free-style | CDML | 0.646 ± 0.007 | 150 EUR |
| Meta-learning | metaCD2 | 0.283 ± 0.007 | 400 EUR |
| Meta-learning | CDML | 0.265 ± 0.006 | 250 EUR |
| New-in-ML | metaCD2 | 0.566 ± 0.007 | 400 EUR |
| New-in-ML | MetaBeyond | 0.699 ± 0.007 | 250 EUR |
| Women | MetaBeyond | 0.699 ± 0.007 | 400 EUR |
| Rarely represented country | EmmanuelPintelas | 0.682 ± 0.007 | 400 EUR |
| Rarely represented country | metaCD2 | 0.566 ± 0.007 | 250 EUR |
| Rarely represented country | CDML | 0.646 ± 0.007 | 150 EUR |

Competition website: [Link](https://codalab.lisn.upsaclay.fr/competitions/3627#learn_the_details)

Competition report: [Link](https://drive.google.com/file/d/1PFOKzZ5SIyPFLom0hHNyA0uyeX_Ribne/view)

More details on the official website: [Link](https://metalearning.chalearn.org/)

## Credits

- Dustin Carrión-Ojeda
- Ihsan Ullah
- Sergio Escalera
- Isabelle Guyon
- Felix Mohr
- Manh Hung Nguyen
- Joaquin Vanschoren
