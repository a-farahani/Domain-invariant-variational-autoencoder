This code is the pytorch implementation of [DIVA: DOMAIN INVARIANT VARIATIONAL AUTOENCODERS](https://arxiv.org/pdf/1905.10427.pdf) Maximilian Ilse et al. the goal of this paper is to tackle the problem of disentaglement and generalizing the representations over the unseen domains. The implementation of the code has not been shared by the authors and I implemented the code based on the architecture explained in the paper for the supervised part and will add unsupervised part soon.
The abstraction of this paper is as below:

"We considers the problem of domain generalization, namely, how to learn representations given data from a set of domains that generalize to data from a previously unseen domain. We propose the Domain Invariant Variational Autoencoder (DIVA), a generative model that tackles this problem by learning three independent latent subspaces, one for the domain, one for the class, and one for any residual variations. We highlight that due to the generative nature of our model we can also incorporate unlabeled data from known or previously unseen domains. To the best of our knowledge this has not been done before in a domain generalization setting. This property is highly desirable in fields like medical imaging where labeled data is scarce. We experimentally evaluate our model on the rotated MNIST benchmark and a malaria cell images dataset where we show that (i) the learned subspaces are indeed complementary to each other, (ii) we improve upon recent works on this task and (iii) incorporating unlabelled data can boost the performance even further."

The architecture is as below:


![alt text](https://github.com/a-farahani/Domain-invariant-variational-autoencoder/blob/master/imgs/DIVA_model.png "DIVA architecture")

