Machine Learning Project Proposal
To: Dr. Lu
From: James Garrison,
Michael Scales
Subject: Project Proposal – CMU Sphinx Improving WER Performance
Date: 11/20/2018
The purpose of this proposal is to get your feedback on our project idea. We are looking to improve the performance
of the Carnegie Mellon Universities’ (CMU) Sphinx Speech Recognition Tool for our single spoken word
application.
Summary
Many modern speech recognition tools are available for use, but they are general purpose and don’t necessarily work
well under specific application constraints. For our application, we want high single word recognition with low
WER (Word Error Rate). Our application wants to execute command words, so the recognition tool must be
accurate for only a single spoken word.
Discussion
We want to test and analyze training model improvements to CMU Sphinx open-source speech recognition toolkit.
We want to look at the benefit of performing model adaptations on the existing training model versus the benefits of
training the model under two different variations. Our project will use four tools: Pocketsphinx 1 , Sphinxbase 2 ,
Pocketsphinx Python 3 , and Sphinxtrain 4 . We intend to use Python and shell scripting to record and tag the
transcription files with their corresponding audio files.
The CMU Sphinx documentation recommends performing acoustic model adaptations on their existing training
models in order to achieve performance improvements. We intend to first perform the adaptation and we will
measure WER. With the captured data we will compare subsequent training techniques to find the optimal training
method characterized as having the lowest WER for a single spoken word.
Next, we will provide alternate transcription files for training the Acoustic Model. Typical transcription files provide
the sequence of words and sounds in groups of phrases. We want to compare the effects of transcription files tagged
by individual words instead of by phrase.
First, we will be train the model by providing it a transcription file using full phrases for each tag. This is the method
that is frequently demonstrated when attempting to improve the performance of a speech recognition tool by training
the model. After training the model with the full phrase transcription file, we will measure WER and compare to our
other results.
For our last experiment, we will train the model by tagging single words in the transcription file. We will measure
WER and compare all of our results to see which method of training provides the lowest WER for a single spoken
word.
Recommendation
Pocketsphinx 1 - lightweight recognizer library written in C
Sphinxbase 2 — support library required by Pocketsphinx
Pocketsphinx Python 3 - Python API for pocketsphinx and Sphinxbase
Sphinxtrain 4 — acoustic model training tools
Our intuition is that training the model using a transcription file which has tagged single words should perform well
compared to acoustic model adaptations or full phrase transcription files. We would appreciate any of your
feedback.
