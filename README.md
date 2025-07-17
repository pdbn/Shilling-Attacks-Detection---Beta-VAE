# Shilling-Attacks-Detection--Beta-VAE

This projects serves as the final assignment to the course EBC 4257 Machine Learning of Maastricht University (i6290653)

Topic: Recommender systems have become increasingly important in modern digital platforms, playing a crucial role in enhancing user satisfaction and engagement.
However, the increasing reliance on recommender systems has also made them vulnerable to adversarial manipulation. One prominent threat is the shilling attack, where malicious users introduce fake profiles with manipulated ratings to unfairly promote or demote certain items. 

Detecting such attacks is inherently a problem of anomaly detection, as the behavior of malicious users typically diverges from that of genuine users. Yet, this task becomes particularly challenging in real-world scenarios where user-item interactions are sparse. For example, in the widely used MovieLens 20M dataset, more than 90\% of the user-item matrix consists of missing values, reflecting the high sparsity common in practical systems. 

In this research, we investigate the application of unsupervised anomaly detection methods for identifying shilling attacks in recommender systems, with a specific focus on deep generative models. We simulate realistic attack scenarios by injecting various types of shilling profiles into the MovieLens 20M dataset and evaluate the ability of these methods to detect them. 

Our primary study is an exploration of the beta-Variational Autoencoder as a framework for detecting anomalous users. The model is trained only on clean user data from the training set to learn the latent representation of normal user behavior. In the testing phase, we introduce a mix of normal and adversarial profiles to assess whether the learned latent distributions can help isolate anomalous users.
