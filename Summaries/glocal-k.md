# GLocal-K: Global and Local Kernels for Recommender Systems

## Abstract

The paper "GLocal-K: Global and Local Kernels for Recommender Systems" proposes a matrix completion framework, named GLocal-K, that uses global and local kernels to represent a high-dimensional sparse user-item matrix entry into a low-dimensional space with a small number of important features, outperforming state-of-the-art baselines on three collaborative filtering benchmarks.

## Summary

GLocal-K is a hybrid recommender system that combines both global and local kernel methods to improve the accuracy of recommendation.

The authors argue that existing approaches to recommendation systems rely too heavily on either global or local information, which can lead to inaccurate results. Global recommendations are based on the overall popularity or rating of items, while local recommendations are based on a user's specific preferences or behavior.

To address this issue, the GLocal-K approach uses both global and local kernels to model the similarities between users and items. The global kernel captures overall similarities between items, while the local kernel captures similarities between items that are relevant to a user's specific interests.

The global kernel method uses all available user-item interactions to compute the similarity between items. The similarity between items is then used to make recommendations to users. However, this approach has a few limitations. For instance, items that are not similar to any other item in the dataset cannot be recommended using this method.

The local kernel method, on the other hand, uses only a subset of the available user-item interactions to compute the similarity between items. This method allows for the identification of similarities between items that may not be obvious when considering the entire dataset.

The GLocal-K approach combines these two methods to overcome the limitations of each. The global kernel method is used to make recommendations for items that have strong similarity to other items in the dataset. The local kernel method is used to identify similarities between items that may not be obvious when considering the entire dataset. By combining these methods, GLocal-K is able to provide accurate recommendations for a wider range of items.

The GLocal-K approach was tested on several real-world datasets and compared to other state-of-the-art recommendation algorithms. The results showed that GLocal-K outperformed other approaches in terms of recommendation accuracy, especially in scenarios where users have sparse or incomplete data.

Overall, GLocal-K is a promising approach for improving the accuracy of recommender systems, particularly in cases where traditional methods may fall short.

## Key insights and lessons learned

* Recommender systems face challenges in matrix completion to predict a user's interest based on a sparse user-item matrix.
* GLocal-K is a matrix completion framework that uses global and local kernels to transform data into a low-dimensional space with a small number of important features.
* GLocal-K is divided into two stages: pre-training an autoencoder with a local kernelized weight matrix and fine-tuning with a convolution-based global kernel using the rating matrix.
* GLocal-K outperformed state-of-the-art baselines on three collaborative filtering benchmarks.

## Citation

### MLA

Han, Soyeon Caren, et al. “GLocal-K: Global and Local Kernels for Recommender Systems.” Proceedings of the 30th ACM International Conference on Information & Knowledge Management, 2021, pp. 3063–67. arXiv.org, https://doi.org/10.1145/3459637.3482112.

## Keywords and Explantions

* **Recommender systems**: Recommender systems are a type of information filtering system that aim to predict the "rating" or "preference" that a user would give to an item. They are primarily used in commercial applications, such as online shopping, movies, music, news, books, research articles, search queries, social tags, and products in general.

* **Matrix completion**: Matrix completion is a problem in which a user-item matrix is incomplete and the goal is to fill in the missing entries. This problem is common in recommender systems, where the goal is to predict a user's interest in an item based on a sparse user-item matrix.

* **Autoencoder**: An autoencoder is a type of neural network that is used to learn efficient data codings in an unsupervised manner. The goal of an autoencoder is to learn a representation (encoding) for a set of data, typically for dimensionality reduction, by training the network to ignore signal "noise".

* **Global kernel**: A global kernel is a kernel method that uses all available user-item interactions to compute the similarity between items. The similarity between items is then used to make recommendations to users.

* **Local kernel**: A local kernel is a kernel method that uses only a subset of the available user-item interactions to compute the similarity between items. This method allows for the identification of similarities between items that may not be obvious when considering the entire dataset.

* **Convolution**: A convolution is a mathematical operation on two functions that produces a third function that expresses how the shape of one is modified by the other. In the context of neural networks, a convolution is a mathematical operation that takes two inputs, typically a matrix and a kernel, and produces an output matrix.

* **Collaborative filtering**: Collaborative filtering is a method of making automatic predictions (filtering) about the interests of a user by collecting preferences or taste information from many users (collaborating). The underlying assumption of the collaborative filtering approach is that if a person A has the same opinion as a person B on an issue, A is more likely to have B's opinion on a different issue x than to have the opinion on x of a person chosen randomly.

* **Sparse matrix**: A sparse matrix is a matrix in which most of the elements are zero. Sparse matrices are used to represent high-dimensional data in a compact form, which can be useful for machine learning algorithms that require a lot of memory.

* **Dimensionality reduction**: Dimensionality reduction is the process of reducing the number of random variables under consideration, often through obtaining a set of principal variables. Dimensionality reduction is a common preprocessing step for machine learning algorithms that are sensitive to the curse of dimensionality.

* **Curse of dimensionality**: The curse of dimensionality is a phenomenon that occurs when the number of features exceeds the number of samples in a training dataset. This can lead to overfitting, where the model learns the noise in the data rather than the underlying relationships.

* **Neural network**: A neural network is a computational model that is inspired by the structure and functions of biological neural networks. Neural networks are used to model complex patterns and relationships in data.

* **Convolutional neural network**: A convolutional neural network (CNN) is a class of deep neural networks that is used for image recognition and classification. CNNs are similar to traditional neural networks, but they are designed to take advantage of the data structure of images.

* **Convolutional autoencoder**: A convolutional autoencoder is a type of autoencoder that uses convolutional neural networks to learn efficient data codings in an unsupervised manner. The goal of a convolutional autoencoder is to learn a representation (encoding) for a set of data, typically for dimensionality reduction, by training the network to ignore signal "noise".
