# ImageToPCA
Takes a satellite imagery, converts it to a series of principal components and displays it with Historgram EQ

This basic jupyter notebook code converts a satellite image to 3 principal components and displays the results using red = PCA1, green = PCA2, blue = PCA3

Here's the text from the Linkedin Post that explains PCA:

Satellite imagery captures reflected light across multiple spectral bands, with each band representing a data dimension. Sentinel-2 imagery records data in 13 spectral bands, each tailored to specific analytical purposes. While humans can visualize data in two or three dimensions (e.g., scatter plots or 3D plots), datasets with higher dimensions—such as Sentinel-2's 13 bands or hyperspectral imagery's 150+ bands—become challenging to interpret visually. Moreover, these datasets often contain redundant information and noise.
Principal Components Analysis (PCA) is a mathematical technique that addresses these challenges by reducing the dimensionality of the data. It transforms the original spectral bands into a new set of uncorrelated components, known as principal components, which are ranked based on the variance they capture:

Dimensionality Reduction: PCA condenses the dataset into a smaller number of principal components that retain most of the original variance, making analysis more manageable.

Noise Suppression: By prioritizing the most informative components, PCA reduces the influence of noise and less significant variations in the data.

Compact Representation: The transformed data is more compact, enabling easier visualization and improving computational efficiency for subsequent analyses.

To demonstrate the power of PCA, I processed a Sentinel-2 image to create a PCA-transformed image. By assigning PCA1 to red, PCA2 to green, and PCA3 to blue, and applying histogram equalization for display, the resulting image reveals enhanced details that are invaluable for applications such as land cover classification, feature extraction, and change detection.
Below is a comparison of the original true-color image and the histogram-equalized PCA image. Notice how the PCA image highlights subtle features, providing greater clarity and insight for remote sensing tasks
