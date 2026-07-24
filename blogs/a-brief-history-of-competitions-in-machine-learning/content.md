## A brief history of competitions in machine learning

Challenges have played a crucial role in the evolution of AI and predictive modeling, involving a stated problem, competitors, public dataset, and scoring methodology (Liberman, 2010; Donoho, 2017).
In her NeurIPS 2022 keynote talk, Isabelle Guyon presents the rich history of competitive machine learning, serving as a primary inspiration for the historical overview that follows.

## Genesis

The idea of leveraging a community of experts and non-experts to solve a scientific problem has been around for hundreds of years.
The long history of scientific challenges begin with the brachistochrone problem, presented by Johann Bernoulli in 1696 as a challenge to the best mathematicians (Herrera, 1994; Bernoulli, 1696). The problem seeks to find the curve of quickest descent, where an object under gravity travels between two points in the shortest possible time. This optimal curve is called the “brachistochrone” curve. Five prominent mathematicians submitted solutions to the challenge: Johann Bernoulli himself (anonymously), Jakob Bernoulli (his brother), Isaac Newton, Gottfried Wilhelm Leibniz and Guillaume de l’Hôpital, although there may have been others who attempted to solve the problem. Leibniz proposed all the received solutions (Leibniz, 1697). The brachistochrone problem was related to mathematics, physics, and engineering. Similarly, machine learning (ML) challenges often cut across multiple domains, and solutions may require knowledge and expertise from various fields. This interdisciplinary approach can lead to more robust and innovative solutions.

Another early example of crowd-sourced challenge is the 1714 British Board of Longitude Prize, which was to be awarded to the person who could solve arguably the most important technological problem of the time: to determine a ship’s longitude at sea (Sobel, 2005). After challenging many established scientists of the time, the prize was awarded to John Harrison for his invention of the marine chronometer. There are two important take home messages from the Longitude Prize example. One is the fact that the winner of the prize was John Harrison, an unknown carpenter and clock-maker, and not a more recognized scientist of that era. The second key idea is that the problem was posed as an open participation challenge, what we refer to today as crowdsourcing. When it comes to novel problems, it is possible that the breakthroughs do not come from other the most established experts in a field.

## Computer science era

Obviously, the earliest challenges do not include machine learning benchmarks, since this discipline had yet to come into existence, and its birth occurred in the twentieth century. Before the 1950s, researchers had discovered and refined statistical techniques, establishing the foundation for future developments.

In 1950, Alan Turing proposed the Turing Test, a measure of a machine’s ability to exhibit intelligent behavior indistinguishable from that of a human. While not a machine learning challenge in the modern sense, it set an early standard for evaluating artificial intelligence.

In the 1950s, pioneering machine learning research was carried out using light algorithms, and by the 1960s, Bayesian methods were introduced for probabilistic inference within the field. However, the 1970s marked an “AI winter”, characterized by pessimism regarding the effectiveness of machine learning. This period of stagnation was followed by a revival in the 1980s, triggered by the discovery of the modern backpropagation algorithm.

Before the 1990s, datasets were exceedingly scarce, often consisting of what we now refer to as “toy data”. It was common to primarily demonstrate new algorithms using synthetic data or small datasets. One such dataset remains commonly used in many introductory machine learning tutorials. This dataset is the Iris dataset (Fisher, 1936), which presents a 3-class classification challenge involving three distinct types of Iris flowers. Remarkably, these classes can be effectively separated using a linear discriminant classifier, commonly known as Fisher’s linear discriminant, employing just four features: petal length and width, as well as sepal length and width. Each class in the dataset comprises 50 examples.

## 1990’s

The 1990’s marked a shift from knowledge-driven to data-driven approaches in machine learning, with a focus on analyzing large datasets. 

This era witnessed the rise of support-vector machines (SVMs), recurrent neural networks (RNNs), and an increase in computational complexity through neural networks.

An important landmark in ML dataset availability was the creation of the UCI ML repository in 1987 by David Aha and his students. The initial datasets were also rather small in size, with the number of examples ranging from 50 to a few hundred and the number of features not exceeding 100. The initial datasets were all tabular dataset, that is tables with samples in lines and features in columns. Raw data, like images, sound, text, video, appeared only later. These datasets were widely used in NeurIPS papers during the 1990’s and as you can imagine people started overfitting them. Even more concerning, people started reporting results only on the subset of datasets that made their algorithms shine. This was denounced with humor in a joke paper submitted to NeurIPS in 2002, “Data Set Selection”, pretending to give a theoretical backing to the bad habit of dataset selection (LaLoudouana and Tarare, 2002).
The 1990’s were marked also by the appearance of systematic benchmarks like the EU project Statlog (King et al., 1995). A consortium of 13 institutions worked together to compare a large number of methods on a large number of datasets, mostly coming from the UCI ML repository. They produced a ranking of algorithms for each dataset. The algorithms included classical statistics (linear and quadratic discriminant, logistic regression, KNN, BN), machine learning (decision tree, rule-based) and neural networks (MLP).

Interestingly, they made a methodology statement:

> “The Project laid down strict guidelines for the testing procedure. First an agreed data format was established, algorithms were “deposited” at one site, with appropriate instructions […]. Each dataset was then divided into a training set and a testing set, and any parameters in an algorithm could be “tuned” or estimated only by reference to the training set. Once a rule had been determined, it was then applied to the test data. This procedure was validated at another site by another (more naive) user. This ensured that the guidelines for parameter selection were not violated, and also gave some information on the ease-of-use for a non-expert in the domain.’’ — Michie et al. (1994)

The methodology described by the Statlog authors encapsulates crucial principles of machine learning. They separate the data into training and testing sets, which allows for the evaluation of a model’s performance on unseen data. They ensure that model parameters are tuned only with reference to the training set, preventing overfitting. They also apply replication and validation procedures, enhancing the robustness of their findings and preventing over-optimization. By storing algorithms at a single site, they enable standardization and comparison, contributing to the development of robust and reproducible machine learning research and practices.

In 1997, the inaugural KKD Cup was organized (Parsa, 1997; Kohavi et al., 2000). Hosted by the Association for Computing Machinery (ACM), this annual competition in Knowledge Discovery and Data Mining is often regarded as the pioneering modern machine learning contest. It continues to be held annually to this day. In the first edition, participants were tasked with classifying anonymous Microsoft web page users. Over the years, the KDD Cup has tackled a variety of problems from different domains. Challenges have ranged from predicting protein structures, to network intrusion detection, to recommendation systems, and more.
Similarly, the National Institute of Standards and Technology (NIST) held their first Speaker Recognition Challenge in 1996 (Martin and Przybocki, 2001). This series of challenges, focused on automatic speaker recognition technology, has received significant appreciation from the research community and continues to be held to this day (S. et al., 2020).

## 2000’s

As the field entered the 2000’s, we observed a rise in popularity of techniques like support-vector machines, kernel methods, and unsupervised learning.
In these years, people from the NeurIPS community started focusing more on raw data, as opposed to data preprocessed as nice tables.

In the realm of image recognition, many datasets relating to Optical Character Recognition (OCR) were collected. OCR is the technology used to convert different types of documents, such as scanned paper documents, PDF files or images captured by a digital camera, into editable and searchable data. There was also an increased interest in datasets for face and object recognition, along with video datasets designed to recognize human actions.
In the field of speech recognition, the Linguistic Data Consortium popularized various datasets (Cieri and Liberman, 2000; Maeda and Strassel, 2004). This organization also provided several extensive text corpora for language study, significantly contributing to language research and natural language processing.
Researchers also started to explore other forms of sensor data, including Electroencephalogram (EEG) data, which captures electrical activity in the brain. Additionally, the first datasets representing graph data began to emerge, opening new possibilities for research and algorithm development in the field of graph theory and network analysis.

The 2000’s were marked by the notable Netflix Prize (Bennett and Lanning,
2007). Announced in 2002 and launched in 2006, this competition continued with various rounds until 2009. Hosted by Netflix, an online movie rental service, its aim was to enhance their movie recommendation algorithm. A grand prize of $1,000,000 awaited the team or individual capable of achieving a 10% improvement over Netflix’s existing recommendation system.
This decades also witnessed the DARPA Challenge, a series of autonomous vehicle competitions organized by the Defense Advanced Research Projects Agency (DARPA). These competitions, initiated in 2004, were designed to promote the development of autonomous ground vehicles to navigate complex terrains without human intervention. The challenges varied in complexity, from navigating desert terrains to urban settings, pushing the boundaries of robotics, machine learning, and computer vision. The advancements from these challenges have significantly impacted the automotive industry, paving the way for the recent growth in autonomous vehicle research (Thrun et al., 2006).

## 2010’s

The 2010’s marked the rise of deep learning, which made machine learning an essential component of various software services and applications used widely across industries.
At the dawn of our millennium, the euphoria of “big data’” led industry leaders to believe that all problems could eventually be solved by adding in more data. Peter Norvig, Director of Research at Google, is often quoted for having said in 2011:

> “We don’t have better algorithms, we just have more data”

However, this simplistic idea has back-fired, with several embarrassing failures of algorithms making racist or sexist decisions (Zou and Schiebinger, 2018). This prompted Peter Norvig to revise his claim in 2017 to the following:

> “More data beats clever algorithms, but better data beats more data”

These are also the years where the first systematic competitions platform appeared, as Kaggle (Goldbloom and Hamner, 2010) was launched in 2010 and CodaLab Competitions (Pavao et al., 2023a) in 2013.
There was a noticeable trend of an increasing number of challenges being organized in conjunction with scientific conferences. ChaLearn, a non-profit organization focused on organizing machine learning challenge, was founded in 2011. At that time, the researchers behind ChaLearn had already organized many challenges, for instances the Feature Selection Challenge at NIPS 2003 (Guyon et al., 2004), the Performance Prediction Challenge at WCCI 2006 (Guyon et al., 2006a), and the Active Learning Challenge at AISTATS 2010 (Guyon et al., 2011). They pursue this efforts by hosting a variety of challenges, covering diverse areas like computer vision through the “Looking at People’’ series, neurology, causal discovery, automated machine learning and physics.

This period also saw a rise in interest in the area of ethics in AI and algorithmic fairness, as the awareness of the societal implications of AI grew. More recently, there has been a growing emphasis on the need for explainable and interpretable AI, particularly given the opaque nature of many deep learning models. Despite the challenges, the progress made in these years set the stage for many exciting developments in machine learning that we are witnessing today.

## 2020’s

And there we are now in the 2020’s, hopefully at the beginning of maturity in Machine Learning.
The center piece is going to be peer review of datasets and benchmarks, which should become a standard and that NeurIPS is strongly encouraging by establishing the NeurIPS D&B track. 
This decade also brings with it a stronger focus on the robustness and reproducibility of machine learning models, underlining the importance of understanding and documenting every step of the machine learning pipeline from data collection to model deployment. The growing popularity of initiatives like PapersWithCode and HuggingFace underscores this point. These platforms facilitate the reuse of state-of-the-art machine learning algorithms, promoting greater accessibility and efficiency in the field.
Competitions continue to demonstrate their efficiency in driving innovation and solving long-standing problems, as illustrated by the CASP14 competition, where DeepMind’s AlphaFold 2 achieved breakthrough accuracy in protein structure prediction (Jumper et al., 2021b,a).


2022 was a big year for competitive machine learning, with a total prize pool of more than $5,000,000 across all platforms, as highlighted by Carlens
(2023). Hundreds of competitions were organized, and the range of machine learning problem studied was wider than ever: computer vision, natural language processing, sequential decision-making problems, robotics, graph learning, optimization, automated machine learning, audio processing, security, meta-learning, causal inference, time-series forecasting, and more, with applications in all fields.
In today’s landscape, there are dozens of platforms, as discussed in ML platforms.

## Conclusions and perspectives

Crowdsourced scientific competitions have a rich history that spans from the Enlightenment period to the present day. They have shown there efficiency in solving diverse problems, from recommender systems and autonomous driving to natural language processing and image recognition. The landscape of machine learning competitions is rapidly expanding, with an increasing number of challenges organized each year (Pavao, 2023b). This trend shows how the organisation of competitions is a promising avenue for making progress in the field of artificial intelligence. As we continue to push the boundaries of what ML models can achieve, it is crucial to develop robust methodologies for evaluating the solutions they produce. Specifically, there is a need to consider the societal impacts of deployed AI technologies and to effectively evaluate complex models, such as large language models (LLMs), as discussed in “Beyond Accuracy: Exploring Exotic Metrics for Holistic Evaluation of Machine Learning Models”. By doing so, we can ensure that the advancements in AI contribute positively to society and are aligned with ethical standards.

## References

Mark Liberman. Fred Jelinek. Computational Linguistics, 36(4) :595–599, 12 2010. ISSN 0891–2017. doi : 10.1162/coli_a_00032. URL https://doi.org/10.1162/coli_a_00032.

David Donoho. 50 years of data science. Journal of Computational and Graphical Statistics, 26(4) :745–766, 2017. doi : 10.1080/10618600.2017.1384734. URL https://doi.org/10.1080/10618600.2017.1384734.

M Herrera. Galileo, bernoulli, leibniz and newton around the brachistochrone problem. Rev Mexicana Fis, 40(3) :459–475, 1994.

J Bernoulli. A new problem to whose solution mathematicians are invited. Acta Eruditorum, 18 :269, 1696.

G. W. Leibniz. Leibniz’ participation his solution and those of j. bernoulli and marquis de l’hospital, to the problem published by j. bernoulli, and at the same time, the solutions to his second problem. Acta Eruditorum Lipsi, page 201, 1697.

Dava Sobel. Longitude : The true story of a lone genius who solved the greatest scientific problem of his time. Macmillan, 2005.

R. A. Fisher. The use of multiple measurements in taxonomic problems. Annual Eugenics, 7(Part II) :179–188, 1936.

Doudou LaLoudouana and Mambobo Bonouliqui Tarare. Data set selection. Neural Information Processing Systems (NIPS), 2002.

R.D. King, C. Feng, and A. Sutherland. Statlog : Comparison of classification algorithm on large real-world problems. Applied Artificial Intelligence, 9(3) : 289–333, 1995. doi : 10.1080/08839519508945477. URL https://doi.org/10.1080/08839519508945477.

D. Michie, D.J. Spiegelhalter, and C.C. Taylor. Machine Learning, Neural and Statistical Classification. 1994.

Ismail Parsa. Kdd-cup-97 : A knowledge discovery and data mining tools competition talk. Newport beach, CA, USA, 1997. URL http://www-aig.jpl.nasa.gov/public/kdd97/.

Ron Kohavi, Carla E Brodley, Brian Frasca, Llew Mason, and Zijian Zheng. Kdd-cup 2000 organizers’ report : Peeling the onion. Acm Sigkdd Explorations Newsletter, 2(2) :86–93, 2000.

A. Martin and M. Przybocki. The nist speaker recognition evaluations : 1996–2001. In A Speaker Odyssey, A Speaker Recognition Workshop, 2001. URL https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=151520.

S., C. Greenberg, E. Singer, D. Reynolds, L. Mason, and J. Hernandez-Cordero. The 2019 nist speaker recognition evaluation cts challenge. In The Speaker and Language Recognition Workshop : Odyssey 2020, 2020. URL https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=929506.

Christopher Cieri and Mark Liberman. Issues in corpus creation and distribution : The evolution of the linguistic data consortium. In Proceedings of the Second International Conference on Language Resources and Evaluation, LREC 2000, 31 May — June 2, 2000, Athens, Greece. European Language Resources Association, 2000. URL http://www.lrec-conf.org/proceedings/lrec2000/html/summary/209.htm.

Kazuaki Maeda and Stephanie M. Strassel. Annotation tools for large-scale corpus development : Using AGTK at the linguistic data consortium. In Proceedings of the Fourth International Conference on Language Resources and Evaluation, LREC 2004, May 26–28, 2004, Lisbon, Portugal. European Language Resources Association, 2004. URL http://www.lrec-conf.org/proceedings/lrec2004/summaries/761.htm.

James Bennett and Stan Lanning. The netflix prize. 2007. URL https://api.semanticscholar.org/CorpusID:9528522.

Sebastian Thrun, Michael Montemerlo, Hendrik Dahlkamp, David Stavens, Andrei Aron, James Diebel, Philip Fong, John Gale, Morgan Halpenny, Gabriel Hoffmann, Kenny Lau, Celia M. Oakley, Mark Palatucci, Vaughan R. Pratt, Pascal Stang, Sven Strohband, Cedric Dupont, Lars-Erik Jendrossek, Christian Koelen, Charles Markey, Carlo Rummel, Joe van Niekerk, Eric Jensen, Philippe Alessandrini, Gary R. Bradski, Bob Davies, Scott Ettinger, Adrian Kaehler, Ara V. Nefian, and Pamela Mahoney. Stanley : The robot that won the DARPA grand challenge. J. Field Robotics, 23(9) :661–692, 2006. doi : 10.1002/rob.20147. URL https://doi.org/10.1002/rob.20147.

James Zou and Londa Schiebinger. Ai can be sexist and racist — it’s time to make it fair, 2018.

Anthony Goldbloom and Ben Hamner. Kaggle. 2010. URL https://www.kaggle.com/.

Adrien Pavao, Isabelle Guyon, Anne-Catherine Letournel, Dinh-Tuan Tran, Xavier Baro, Hugo Jair Escalante, Sergio Escalera, Tyler Thomas, and Zhen Xu. Codalab competitions : An open source platform to organize scientific challenges. Journal of Machine Learning Research, 24(198) :1–6, 2023a. URL http://jmlr.org/papers/v24/21-1436.html.

Isabelle Guyon, Steve Gunn, Asa Ben-Hur, and Gideon Dror. Result analysis of the nips 2003 feature selection challenge. In L. Saul, Y. Weiss, and L. Bottou, editors, Advances in Neural Information Processing Systems, volume 17. MIT Press, 2004. URL https://proceedings.neurips.cc/paper/2004/file/5e751896e527c862bf67251a474b3819-Paper.pdf.

Isabelle Guyon, Amir Reza Saffari Azar Alamdari, Gideon Dror, and Joachim M. Buhmann. Performance prediction challenge. 2006a.

Isabelle Guyon, Gavin C. Cawley, Gideon Dror, and Vincent Lemaire. Results of the active learning challenge. In Isabelle Guyon, Gavin C. Cawley, Gideon Dror, Vincent Lemaire, and Alexander R. Statnikov, editors, Active Learning and Experimental Design workshop, In conjunction with AISTATS 2010, Sardinia, Italy, May 16, 2010, volume 16 of JMLR Proceedings, pages 19–45. JMLR.org, 2011. URL http://proceedings.mlr.press/v16/guyon11a/guyon11a.pdf.

John Jumper, Richard Evans, Alexander Pritzel, Tim Green, Michael Figurnov, Olaf Ronneberger, Kathryn Tunyasuvunakool, Russ Bates, Augustin Žídek, Anna Potapenko, et al. Highly accurate protein structure prediction with alphafold. Nature, 596(7873) :583–589, 2021b.

Harald Carlens. State of competitive machine learning in 2022. ML Contests, 2023.

Adrien Pavão. Methodology for Design and Analysis of Machine Learning Competitions. PhD thesis, Université Paris-Saclay, December 2023.


_Original content by [Adrien Pavão](https://adrienpavao.com/)._