<p>From the beginning of the machine learning era, one aspect that has been constant throughout is data. Our model depends highly on the data we use to train our model. Noise in the data can significantly affect various data analysis tasks such as classification, clustering, and association analysis. What if someone tries to manipulate our data points? One question that might occur to you is that “Well, how can anyone manipulate our instances and why? And even if anybody does so, can’t we see it?”. One famous example to illustrate this is by I. Goodfellow et al. in the paper “Explaining and Harnessing Adversarial Examples”.</p>

![Example]{/assets/images/Adversarial_Panda_example.png}

<p>As it can be seen from the example above, to us normal humans, the image on both sides looks like a Panda. But when we add a carefully crafted noise to the actual image, the classifier misinterprets it. So much so that it is classifying the image on the right as a ‘Gibbon’ with over 99% confidence. So yes, in most cases we cannot see if an image is manipulated.</p>

<p>Therefore, it can be safe to formally state now that Adversarial examples are a threat to AI safety. Let us consider an example of a Self-driving car. These cars are usually capable of identifying common road signs. But what if an ill-intended adversary replaces a regular stop sign with another stop sign that has some calculated noise added to it which makes these self-driven cars identify it as a smiley face instead? This may end up causing loss of life even. Hence, studying these attacks and having algorithms that are tolerant to these noises are the need of the hour.</p>

<p>Three main aspects are used to evaluate the performance of these adversarially robust algorithms.</p>

1. Noise tolerance — Many kinds of noise exist when it comes to adversarial examples. Massart noise, Agnostic noise, Malicious noise, Nasty noise, to name a few. The algorithm to be developed should be robust to strongly corrupted data.
2. Computational efficiency — The goal remains to create algorithms such that they have utmost polynomial time complexity. Otherwise, it is impractical to implement such algorithms.
3. Sample and Label complexity — The last goal that remains is that the algorithm is label efficient and sample efficient. The first step to developing any Machine Learning model is to gather data. After collecting a bunch of data, we need to label each instance appropriately, and usually, this is done by crowdsourcing. This is a tedious process and there are times when the instance is not correctly labeled as well (As people we tend to make mistakes). Therefore we hope to find the ground truth by requiring a minimum number of samples and labels.

<p>Therefore we would want to build an algorithm that is noise-tolerant, computationally efficient, and minimizes the sample complexity and label complexity.
</p>

<p>So, machine learning models need to be trained so that the resulting model will be resistant to the noise and produce accurate results. Noise in a machine learning dataset can broadly be classified into two types: (i) attribute noise and (ii) class or label noise. Attribute noise is the noise present in the predictive attributes and label noise is the one present in the target attribute. Presence of noise in a dataset can cause increase in the number of training examples and increase in the model complexity. It is known through studies that label noise is potentially more harmful than feature noise.</p>

<p>Algorithms specific to a particular noise model are proposed in the literature. Following are some of the noise models considered in the agnostic PAC learning of halfspaces:
</p>

<p>In this article we have learned about noise and why is it important for us to build robust classifiers. We have also discussed shortly on the different kinds of noise models in the agnostic PAC learning of halfspaces.</p>

<p>To know more about adversarial noise I suggest you to watch the guest lectures by I. Goodfellow on the topic on YouTube. There is another video where J. Z. Kolter and A. Madry present Adversarial Robustness — Theory and Practice in NeurIPS 2018 which I personally found helpful. Happy Learning :)</p> 
