# DarknetGNNClassifier

Using Graph Neural Networks to classify scanner behavior by mapping the Darknet as a graph

Project done as the final project for my "Networking and Machine Learning class"
> A graduate class bridging Networking and Machine Learning

## Motivation
- Packets sent to the Darknet is interesting. It can be caused by: 
  - Scanners (both malicious and non-malicious) finding open ports
  - Configuration error
- Networks are laid out like a graph, so why not use Graph NNs?

## Project Overview
- Construct the packets as a graph using MetaPath2Vec (Node2Vec for Heterogenous graphs)
- Use clustering methods to determine scanner behaviors: Found 4 types of scanners.
  - Use HDBScan and hyperparameter tune it for sillhouette score using Bayesian Optimization
- **Final Slides** and **Report** in the main directory

## Notes
- Project used the UCSD Caida Darknet Telescope dataset
  - https://www.caida.org/projects/network_telescope/
- Project was done on Google Colab

