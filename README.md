### Thesis
My graduation thesis (Bachelor) in russian language. Short summary of the work is available in this file.  
In thesis, multiple techniques are used to construct embeddings for social network groups (i.e. Facebook groups)  
In this work anonymous data from vk.com was used to test various approaches (existing one and proposed solution)
### Algorithm
In this work, skip-gram model was taken as the baseline. Model was trained on likes, subscribe and unsubscribe data, with various modifications of the NLP algorithm, i.e. an optimization function. Likes were represented as a weak signals, while subscribe/unsubscribe were strong signals. Combining various inputs was a challenge, and new optimization function was created.
### Experiments and results
Small sample of 1200 groups and 45000 user session was used. Various formulas were tested, such as softmax (baseline), and custom formulas. (*See table 1*).   
One of the discovered formulas (softmax approximation) had the same accuracy as the softmax, but was more usable in real-life scenarios (i.e. it doesn't depend on number of unique groups, and the time to calculate it is lower)  
Various techniques were used to test the quality of result embeddings, making use of tags related to social groups.  
Model was tested against standard approaches in the field (ALS/LDA) and was proven to have better accuracy on next user action (*table 6*), geolocation (*table 7*). 

