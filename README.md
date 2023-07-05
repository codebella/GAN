# GAN
Data Synthesis for Modern Application

Every decade we see a shift in technology usage. From Radio, walkman, ipod to latest and greatest wearables. The irony is, some of us may have more apps in their phone to track different things than the fresh pair of cloths in our wadrobes. Naturally the world is becoming more vigilant in how these apps are using the collected data.
We already have seen phase where data privacy making businesses revisit their data gathering and storage terms. Not far from now, we will see that consent based data collection may even be chargeable.

In modern software development practices, we see that though their is consent about a given data availablility in production systems, however there are equal amount of information barriers which have to be maintained in brining this production data to the lower dev/test environments. For the benefit of keeping the essense of the paper, I have coined the term data-synthesis in parlance to photosynthesis, why so because the way plant produce their food using the process photosysnthesis, the modern tools will also be enabled to produce the data using data-synthesis. 

There are two forms of synthetic data generation techniques which can be utilized here
1) Parameterized: this will enable application to do data-synthesis for all their logical paths exactly once
2) Volume based: applications will carry out data-synthesis to produce delta variation for already generated data

Data Preprocessing: Start by preprocessing your real data to ensure it is in a suitable format for training the GAN. Normalize or scale the data, handle missing values, and encode categorical variables if necessary.

GAN Architecture: Design the architecture of the generator and discriminator networks. For multidimensional data, you'll typically use deep neural networks with multiple layers. The input to the generator is a random noise vector, and the output is a synthetic data sample with the same dimensions as the real data.

Training: Train the GAN by alternating between updating the discriminator and the generator. Initially, the generator produces random samples, and the discriminator learns to distinguish between the real and synthetic samples. The generator then tries to generate samples that fool the discriminator. This iterative process continues until the generator produces synthetic samples that closely resemble the real data.

Evaluation: After training the GAN, evaluate the quality of the generated synthetic data. Compare statistical properties such as mean, standard deviation, correlation, and distribution shapes between the real and synthetic data to ensure similarity. Visualizations and statistical tests can help in assessing the performance of the synthetic data generation.

Fine-tuning: If necessary, you can further refine the generated synthetic data. For example, you can adjust the training parameters, network architecture, or incorporate additional techniques like regularization to improve the quality and diversity of the synthetic samples.

It's important to note that GANs can be challenging to train and may require a significant amount of computational resources and fine-tuning. However, they can generate realistic and high-dimensional synthetic data that captures the complex patterns and dependencies present in the real data.
