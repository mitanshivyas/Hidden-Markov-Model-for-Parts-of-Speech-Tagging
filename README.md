# Hidden-Markov-Model-for-Parts-of-Speech-Tagging 

## HMM

This repository contains a from-scratch Hidden Markov Model implementation utilizing the Forward-Backward algorithm and Expectation-Maximization for probabilities optimization. 
The HMM is one of the most commonly used algorithms in Natural Language Processing, and is a foundation to many deep learning techniques. In addition to parts-of-speech tagging, HMM is used in speech recognition, speech synthesis, etc.

## Procedure

The Markov Model contains a number of states and the probability of transition between those states.

In this case, the states are the parts-of-speech. A Markov Model utilizes a transition matrix, A. A Hidden Markov Model adds an observation or emission matrix B which describes the probability of a visible observation when we are in a particular state. In this case, the emissions are the words in the corpus. The state, which is hidden, is the POS tag of that word.

HMM models calculate first the probability of a given sequence and its individual observations for possible hidden state sequences, then re-calculate the matrices above given those probabilities. By iterating back and forth (what's called an expectation-maximization process), the model arrives at a local optimum for the tranmission and emission probabilities. It's a pretty good outcome for what might otherwise be a very hefty computationally difficult problem.
