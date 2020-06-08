# Speech Emotion Recognition using CNN with RAVDESS dataset

You can run this notebook on local machine using Jupyter Notebook, or on Google Colab if you want to save some disk space. For Google Colab, you will mount this notebook to your Google Drive, download/save the dataset in the Drive.

### About RAVDESS dataset

This is the Ryerson Audio-Visual Database of Emotional Speech and Song dataset, and is free to download. This dataset has 7356 files rated by 247 individuals 10 times on emotional validity, intensity, and genuineness. The entire dataset is 24.8GB from 24 actors, but we’ve lowered the sample rate on all the files. In our model, we are taking the emotion (third identifier) in consideration only.

### File naming convention

Each of the 7356 RAVDESS files has a unique filename. The filename consists of a 7-part numerical identifier (e.g., 02-01-06-01-02-01-12.mp4). These identifiers define the stimulus characteristics:

### Filename identifiers

- Modality (01 = full-AV, 02 = video-only, 03 = audio-only).
- Vocal channel (01 = speech, 02 = song).
- Emotion (01 = neutral, 02 = calm, 03 = happy, 04 = sad, 05 = angry, 06 = fearful, 07 = disgust, 08 = surprised).
- Emotional intensity (01 = normal, 02 = strong). NOTE: There is no strong intensity for the 'neutral' emotion.
- Statement (01 = "Kids are talking by the door", 02 = "Dogs are sitting by the door").
- Repetition (01 = 1st repetition, 02 = 2nd repetition).
- Actor (01 to 24. Odd numbered actors are male, even numbered actors are female).

---

### Model is trained for 100 epochs

![model is trained for 100 epochs](https://github.com/huaiyukhaw/speech-emotion-recognition/blob/master/screenshot/screenshot1.png)

### Learning curve of the model
![model accuracy](https://github.com/huaiyukhaw/speech-emotion-recognition/blob/master/screenshot/screenshot2.png)

![loss accuracy](https://github.com/huaiyukhaw/speech-emotion-recognition/blob/master/screenshot/screenshot3.png)

### Confusion matrix
![confusion matrix](https://github.com/huaiyukhaw/speech-emotion-recognition/blob/master/screenshot/screenshot4.png)

### Model summary
![model summary](https://github.com/huaiyukhaw/speech-emotion-recognition/blob/master/screenshot/screenshot5.png)



This is a group effort with my friends — Yit Tyn, Zhi Qin, and Jing Xuan.
