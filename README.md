# SiameseNet_using_LSIDD
Our  model utilizes the image of SIDD dataset. It's the first image-based data set for network attack detection. dataset contained communication-based network traffic log images from 15 different observation sites in various countries in Asia. which is used to identify two different types of anomalies in harmless network traffic. Each 48x48 image contains multi-protocol communication within 128 seconds 
We train our Siamese network model based on the paired group, malicious, and Benign. From the image paired image, we feed one image to network A and another image to network B. The role of these two networks is only to extract the feature vectors. So, we use three convolution layers with relu activations for extracting the features. Once we have learned the feature, we feed the resultant feature vectors from both networks to the energy function which measures the similarity, we use Euclidean distance as our energy function. We train our network by feeding the image pair to learn the semantic similarity between them.
