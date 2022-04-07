# T-T-Lab-Project

# About the Dataset: 
The GTZAN genre collection dataset was collected in 2000-2001. It consists of 1000 audio files each having 30 seconds duration. There are 10 classes ( 10 music genres) each containing 100 audio tracks. Each track is in .wav format. It contains audio files of the following 10 genres: 
1.Blues 2.Classical 3.Country 4.Disco 5.Hiphop 6.Jazz 7.Metal 8.Pop 9.Reggae 10.Rock

# Aim:
To develop a deep learning project to automatically classify different musical genres from audio files. Classifying these audio files using their low-level features of frequency and time domain.

# Flow - Diagram:
Dataset --> Feature Extraction --> (Data Augumention) --> Model Training --> Trained Classifer --> Prediction <-- Feature Extraction <-- Input Audio File.

# Technologies/Techniques/Languages Used:
Language: Python 
Technology: Deep Learning
Techniques: Feature Extraction, Neural Network Algorithms, Data Augumention.

# Input/Output:
Input : An audio file (.wav format)
Output : Input audio's predicted genre

#Project Brief --
Processes and Accuracy:
1. model trained using the original data and different augmented data individually (pitch and rate increased/decreased) gave ~70% accuracy each.
2. combined all the data  generated using different types of data augmentation which increased the data from ~1000 to ~5000  and recieved accuracy of ~80%
3. Updated CNN model to a Hybrid CRNN(CNN + RNN) model  and trained using oringinal data gave accuracy of ~ 89%
4. Used all the combined data i.e., 5000 audio files + the Hybrid CRNN model which gave accuracy of ~ 94%

#files --

CNN_Original.ipynb               - trained using original data
CNN_PitchBoosted_-2.0.ipynb      - lowerd the pitch by -2.0 nsteps and trained using that data
CNN_PitchBoosted_2.0.ipynb       - boosted the pitch by +2.0 nsteps and trained using that data
CNN_RateBoosted_0.9.ipynb        - lowerd the rate by 0.9 times and trained using that data
CNN_RateBoosted_1.1.ipynb        - boosted the rate by 1.1 times and trained using that data
CNN_FinalCombined.ipynb          - combined all the data from all types of augmentation and trained using that 5000 data
CRNN_Original.ipynb              - trained using original data to the Hybrid CRNN model
CRNN_HybridFinalCombined.ipynb   - combined all the data from all types of augmentation and trained using that 5000 data to the Hybrid CRNN model
