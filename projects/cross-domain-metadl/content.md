## Competition overview

Meta-learning aims to leverage experience from previous tasks to solve new tasks efficiently. Lately, meta-learning has contributed a lot of progress in few-shot learning for image classification. However, evaluation protocols have had two common drawbacks:

- Even when evaluated on multiple domains (insect classification, texture classification, satellite images, and so on), models meta-trained on a given domain are meta-tested on the same domain, which is called *within-domain* few-shot learning.
- In N-way k-shot problems, the number of ways N (classes) and shots k (training examples per class) is usually fixed.

Cross-Domain MetaDL is the continuation of our NeurIPS 2021 MetaDL competition, which tackled the within-domain problem in a fixed 5-way 5-shot setting. The novelties are:

- **Protocol**: still code submission with one-chance blind testing on new datasets in the final phase, but closer to the real-world scenario where data comes from different domains and not always with the same number of classes and examples per class.
- **Data**: an extension of the Meta-Album dataset we started putting together the year before: 30 image classification datasets from 10 domains, uniformly formatted as 128×128 RGB images carefully resized with anti-aliasing filters.

## Prizes

The €4,000 prize pool was distributed among 5 different leagues:

- **Free-style league**: submit a solution obeying the basic challenge rules (pre-trained models allowed).
- **Meta-learning league**: submit a solution that meta-learns from scratch (no pre-training allowed).
- **New-in-ML league**: for participants with fewer than 10 ML publications, none ever accepted to the main track of a major conference.
- **Women league**: a special league to encourage women, who rarely enter challenges.
- **Rarely represented country league**: for participants from outside the top 10 most represented countries in challenge participation.

Entering multiple leagues was permitted. Top-ranking participants also received a certificate and were invited to co-author the post-challenge analysis paper published in the NeurIPS proceedings of the competition track, along with travel awards distributed on merit and need.

## Phases

- **Public phase (2 weeks)**: the starting kit and 10 public datasets were released so participants could familiarize themselves with the problem.
- **Feedback phase (8 weeks)**: participants submitted solutions and received feedback on 10 hidden datasets, on 10 identical workers (4 CPU cores, 1 Tesla T4 GPU, 16 GB RAM, 120 GB storage each).
- **Final phase (4 weeks)**: the last submission of each participant was blind-tested on 10 new hidden datasets to rank participants and select winners.

Public phase started June 15, 2022; feedback phase July 1; final phase September 1; winners were notified between October 1 and 15, 2022.

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

## Credits

Dustin Carrión-Ojeda, Ihsan Ullah, Sergio Escalera, Isabelle Guyon, Felix Mohr, Manh Hung Nguyen, Joaquin Vanschoren.
