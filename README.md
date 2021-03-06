# Music-Genre-Classification
Author: 
* [Apoorva Srivastava](https://github.com/apooorvasri)
* [Umang Sorathiya](https://github.com/umang718)
* [Vivek Joshi](https://github.com/vivekjoshi556)

This project has two main files
*  main.py - Contains the main executable code.
*  features.py - This contains helper functions like to extract audio features.

The name of the dataset is GTZAN dataset and it can be downloaded from the given link (https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification)

The data will be downloaded in zip form and contains multiple files. We'll be using only the audio files present in the extracted folder. 
So we just need the genres_original folder from the zip. Rename the folder "genres_original" to "genres" and put that folder in a separate folder with the two files mentioned above.

To see the working of code just run the ipynb file named main.ipynb.

**Features Used**:<br/>
Audio features are primarily from 2 domains:<br/>
• Time-domain Features: <br/>
&emsp;1. Amplitude Envelope<br/>
&emsp;2. Root Mean Square Energy<br/>
• Frequency-domain Features:<br/>
&emsp;1. Mel Frequency Cepstral Coefficient (MFCC)<br/>

***MFCC was used in this project because unlike other features. MFCC has the capability to differentiate between various frequencies just like humans would perceive those sounds.***<br/>

**Techniques and Models Used**<br/>
• K-Means Clustering<br/>
• K-Nearest Neighbours<br/>
• Multiclass SVM<br/>
<br/>
**Metrics Comparison and Results**<br/>
KMC performed very poorly for the given feature values of the selected dataset because it tries to create clusters using the nearby values.<br/>
KNN performed well over the same given dataset because it takes only k values nearest to itself, which is a much better measure to differentiate between different genres.<br/>
SVM : In case of polynomial model, the accuracy slightly decreases compared to the KNN model. Whereas the linear models shows slight improvement in accuracy.<br/>
![image](https://user-images.githubusercontent.com/38426238/173165415-36ca8ae8-6f18-43fd-a452-3d71c5c0e7b6.png)







