---
date: 2021-06-16
title: "Review: Handwriting Recognition Using AI"
linkTitle: "Handwriting"
tags: ["report", "reu" , "comunication"]
description: "This study reviews two approaches and/or machine learning tools used by researchers/developers to convert handwritten information into digital forms using Artificial Intelligence."
author: Mikahla Reeves
github_url: https://github.com/cybertraining-dsc/su21-reu-366/edit/main/project/index.md
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---

[![Check Report](https://github.com/cybertraining-dsc/su21-reu-366/workflows/Check%20Report/badge.svg)](https://github.com/cybertraining-dsc/su21-reu-366/actions)
[![Status](https://github.com/cybertraining-dsc/su21-reu-366/workflows/Status/badge.svg)](https://github.com/cybertraining-dsc/su21-reu-366/actions)
Status: final, Type: Report

Mikahla Reeves, [su21-reu-366](https://github.com/cybertraining-dsc/su21-reu-366), [Edit](https://github.com/cybertraining-dsc/su21-reu-366/blob/main/project/index.md)

{{% pageinfo %}}

## Abstract

The first thing that comes to numerous minds when they hear *Handwriting Recognition* is simply computers identifying handwriting,
and that is correct. Handwriting Recognition is the ability of a computer to interpret handwritten input received from different sources. 
In the artificial intelligence world, handwriting recognition has become a very established area. Over the years, there have been many 
developments and applications made in this field. In this new age, Handwriting Recognition technologies can be used for the conversion of
handwritten and/or printed text to speech for the blind, language translation, and for any field that requires handwritten reports to be 
converted to digital forms instantly.

This study investigates two of the approaches taken by researchers/developers to convert handwritten information to digital 
forms using (AI) Artificial Intelligence. These two deep learning approaches are the (CNN) Convolutional Neural Network and 
(LSTM) Long Short Term Memory. The CNN takes advantage of the spatial correlation in data, while LSTM makes predictions based on sequences of data. 

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** handwriting recognition, optical character recognition, deep learning.

## 1. Introduction

Perhaps one of the most monumental things in this modern-day is how our devices can behave like brains. Our various devices can call mom, play our favorite song,
and answer our questions by just a simple utterance of Siri or Alexa. These things are all possible because of what we call artificial intelligence. Artificial
intelligence is a part of computer science that involves learning, problem-solving, and replication of human intelligence. When we hear of artificial intelligence,
we often hear of machine learning as well. The reason for this is because machine learning also involves the use of human intelligence. Machine learning is the
process of a program or system getting more capable over time [^2]. One example of machine learning at work is Netflix. Netflix is a streaming service that allows
users to watch a variety of tv shows and movies, and it also falls under the category of a recommendation engine. Recommendation engines/applications like Netflix
do not need to be explicitly programmed. However, their algorithms mine the data, identify patterns, and then the applications can make recommendations.

Now, what is handwriting recognition? Handwriting Recognition is a branch of (OCR) Optical Character Recognition. It is a technology that receives handwritten
information from paper, images, and other items and interprets them into digital text in real-time [^1]. Handwriting recognition is a well-established area in the
field of image processing. Over the last few years, developers have created handwriting recognition technology to convert written postal codes, addresses, math questions,
essays, and many more types of written information into digital forms, thus making life easier for businesses and individuals. However, the development of handwriting
recognition technology has been quite challenging.

One of the main challenges of handwriting recognition is accuracy, or in other words, the variability in data. There is a wide variety of handwriting styles, both good and bad, 
thus making it harder for developers to provide enough samples of what a specific character/integer looks like [^3]. In handwriting recognition, the computer has to translate 
the handwriting into a format that it understands, and this is where Optical Character Recognition becomes useful. In OCR, the computer focuses on a character, compares it to 
characters in its database, then identifies what the letters are and fundamentally what the words are. Also, this is why deep learning algorithms like Convolutional Neural 
Networks and Long Short Term Memory exist. This study will highlight the impact each algorithm has on the development of handwriting recognition.

## 2. Convolutional Neural Network Model 

![Figure 1](https://github.com/cybertraining-dsc/su21-reu-366/raw/main/project/images/CNN.jpg)

**Figure 1:**  Architecture of CNN for feature extraction [^4]

In this model, the *input image* passes through two convolutional layers, two sub-sample layers, and a linear SVM (Support Vector Machine) that allows for the output
which is a *class prediction*. This class prediction leads to the editable text file. 

Class prediction is a supervised learning method where the algorithm learns from samples with known class membership (training set) and establishes a 
prediction rule to classify new samples (test set). This method can be used, for instance, to predict cancer types using genomic expression profiling [^8].

## 3. Long Short Term Memory Model

![Figure 2](https://github.com/cybertraining-dsc/su21-reu-366/raw/main/project/images/LSTM.jpg)

**Figure 2:** Overview of the CNN-RNN hybrid network architecture [^6]

This model has a spacial transformer network, residual convolutional blocks, bidirectional LSTMs and the CTC loss (Connectionist Temporal Classification loss)
which are all the processes the *input worded image* has to pass through before the output which is a *label sequence*.

Sequence labeling is a typical NLP task which assigns a class or label to each token in a given input sequence [^9].

## 4. Handwriting Recognition using CNN

![Figure 3](https://github.com/cybertraining-dsc/su21-reu-366/raw/main/project/images/HRS.png)

**Figure 3:** Flowchart of handwriting character recognition on form document using CNN [^4]

In the study, former developers created a system to recognize the handwriting characters on form document automatically and convert it into editable text.
The system consists of four stages: get ROI (Region of Interest), pre-processing, segmentation and classification. In the getting ROI stage, according to 
the specified coordinates, the ROI is cropped. Next, each ROI goes through pre-processing. The pre-processing consists of bounding box removal using
the eccentricity criteria, median filter, and bare open. The output image of the pre-processing stage will be segmented using the Connected Component
Labeling (CCL) method. It aims to get an individual character[^4].

## 5. Conclusion

In this study, we learned how to use synthetic data, domain-specific image normalization, and augmentation - to train an LSTM architecture[^6]. 
Additionally, we learned how a CNN is a powerful feature extraction method when applied to extract the feature of the handwritten characters and 
linear SVM using L1 loss function and L2 regularization used as end classifier[^4].

For future research, we can focus on improving the CNN model to be able to better process information from images to create digital text. 

## 6. Acknowledgments

This paper would not have been possible without the exceptional support of Gregor von Laszewski, Carlos Theran, Yohn Jairo.
Their constant guidance, enthusiasm, knowledge and encouragement have been a huge motivation to keep going and to complete this work.
Thank you to Jacques Fleicher, for always making himself available to answer questions. Finally, thank you to Byron Greene
and the Florida A&M University for providing this great opportunity for undergraduate students to do research.

## 7. References

[^1]: Handwriting Recognition in 2021: In-depth Guide. (n.d.). <https://research.aimultiple.com/handwriting-recognition>

[^2]: Brown, S., 2021. Machine learning, explained | MIT Sloan. [online] MIT Sloan. Available at: <https://mitsloan.mit.edu/ideas-made-to-matter/machine-learning-explained>.

[^3]: ThinkAutomation. 2021. Why is handwriting recognition so difficult for AI? - ThinkAutomation. [online] Available at: <https://www.thinkautomation.com/bots-and-ai/why-is-handwriting-recognition-so-difficult-for-ai/>.

[^4]: Darmatasia, and Mohamad Ivan Fanany. 2017. "Handwriting Recognition on Form Document Using Convolutional Neural Network and Support Vector Machines (CNN-SVM)." In 2017 5th International Conference on Information and Communication Technology (ICoIC7), 1–6.

[^5]: Ramakrishnan, A. G. "The Magic of Automated Recognition of Handwriting." Current Science 107, no. 2 (2014): 159-60. <http://www.jstor.org/stable/24103112>

[^6]: K. Dutta, P. Krishnan, M. Mathew and C. V. Jawahar, "Improving CNN-RNN Hybrid Networks for Handwriting Recognition," 2018 16th International Conference on Frontiers in Handwriting Recognition (ICFHR), 2018, pp. 80-85, doi: 10.1109/ICFHR-2018.2018.00023.

[^7]: S, Preetha, Afrid I M, Karthik Hebbar P, and Nishchay S K. 2020. "Machine Learning for Handwriting Recognition." International Journal of Computer (IJC) 38 (1), 93-101. <https://ijcjournal.org/index.php/InternationalJournalOfComputer/article/view/1637>

[^8]: "Class Prediction (Predict Parameter Value)." NEBC: NERC Environmental Bioinformatics Centre. Silicon Genetics, 2002. <http://nebc.nerc.ac.uk/courses/GeneSpring/GS_Mar2006/Class%20Prediction.pdf>

[^9]: Jacob. "Deep Text Representation for Sequence Labeling." Medium. Mosaix, August 15, 2019. <https://medium.com/mosaix/deep-text-representation-for-sequence-labeling-2f2e605ed9d>
