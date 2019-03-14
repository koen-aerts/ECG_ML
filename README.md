# ECG Machine Learning
This project contains Datalab notebooks that help you download the publicly available [MIT-BIH Arrhythmia Database](https://physionet.org/physiobank/database/mitdb/), and do some Machine Learning on it to predict if the heart-beats in your ECG data classify either as "Normal" or "Abnormal".

Many training models on ECG data seem to work around building out a Convolutional Neural Network (CNN) in Keras. A [CNN](https://en.wikipedia.org/wiki/Convolutional_neural_network) is typically used for classifying image data, for instance is this picture a house or a cat. [Keras](https://keras.io/) is the API that makes building such a neural network relatively easy. The model in this project instead uses [Tensorflow Estimators](https://www.tensorflow.org/guide/estimators).

More details are included in each of the notebook files.

# Requirements
* [Google Datalab](https://cloud.google.com/datalab/) - Click [here](https://koenaerts.ca/running-google-datalab-locally/) to learn how to run Datalab on your local workstation or VM.
* [Python](https://www.python.org/) - This may already come installed on your Linux distribution. Recommended version is 3.
* [NumPy](https://docs.scipy.org/doc/numpy/dev/)
* [Matplotlib](https://matplotlib.org/)
* [wfdb](https://pypi.org/project/wfdb/)
* [mitdb](https://github.com/Nospoko/qrs-tutorial) - You'll need the code from the "datasets" and the "utils" directory. In Python 3 you may see compilation errors for this library. In most cases you just need to put round brackets in the "print" statements - example "print '123'" would become "print('123')". In one case you need to replace an import statement from "import urllib2" to "import urllib.request as urllib2". The error messages from your notebook will guide you to the proper files. Files affected are "datasets/mitdb.py" and "utils/download.py".
* [BioSPPy](https://github.com/PIA-Group/BioSPPy)
* [Tensorflow](https://www.tensorflow.org/)

Note that most of the above Python libraries are already included in the Datalab Docker image when you install Datalab on your localhost machine.

# Disclaimer
Do not use anything from this project to make medical decisions. It is for educational and learning purposes only.

# More Info
[Mobia Technology Innovations](http://mobia.io/)
