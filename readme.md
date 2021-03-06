### Image Similarity using Siamese Neural Network

This project uses a **Siamese architecture** to detect the similarity between two image pairs. A Siamese Neural Network is a class of neural network architectures that contain two or more identical subnetworks. ' identical' here means, they have the same configuration with the same parameters and weights. Parameter updating is mirrored across both sub-networks.

![Siamese Architecture](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcThYeo64i2nIkmPO0aX-OJ7yP7ezkjH5MxNUg&usqp=CAU)

The data is taken from the Fashion-MNIST dataset. Image pairs are made, similar ones being labelled as 1 and dissimilar pairs labelled as 0. The model is used is simple convultional one with dense layers to output 28 size embedding for each image. The embeddings are then passed to a lambda layer that calculates the euclidean distance between the two embeddings and finally the distance is sent to a dense layer with single nueron have sigmoid activation. The model shares weight across the two image pairs and hence acts as sister networks or a siamese network. 
