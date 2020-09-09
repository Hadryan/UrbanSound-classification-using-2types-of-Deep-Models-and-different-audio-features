#### *This repo contains my undergraduate thesis work*

### Thesis Topic:
Urban Sound Classification Using Convolutional Neural Network and Long Short Term Memory Based on Multiple Features

### Dataset: 
[Urban Sound Classification](https://urbansounddataset.weebly.com/urbansound8k.html). For detailed explaination about the dataset and the methods used to clean and compile it please read this [paper](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/salamon_urbansound_acmmm14.pdf).

### Audio features(Spectral features) extracted:
[MFCC](https://librosa.org/doc/latest/generated/librosa.feature.mfcc.html#librosa.feature.mfcc), 
[Mel Spectrogram](https://librosa.org/doc/latest/generated/librosa.feature.melspectrogram.html#librosa.feature.melspectrogram), 
[Chroma STFT](https://librosa.org/doc/latest/generated/librosa.feature.chroma_stft.html#librosa.feature.chroma_stft), [Chroma CQT](https://librosa.org/doc/latest/generated/librosa.feature.chroma_cqt.html#librosa.feature.chroma_cqt), 
[Chroma Cens](https://librosa.org/doc/latest/generated/librosa.feature.chroma_cens.html#librosa.feature.chroma_cens),[Spectral Contrast](https://librosa.org/doc/latest/generated/librosa.feature.spectral_contrast.html#librosa.feature.spectral_contrast),
[Tonnetz](https://librosa.org/doc/latest/generated/librosa.feature.tonnetz.html#librosa.feature.tonnetz).

### Models Used:
* A CNN model with layers of **CONV2D ---> MAXPOOL ---> CONV2D ---> MAXPOOL ---> DENSE ---> DENSE ---> SOFTMAX**.The first layer of Conv2d uses 64 filters with the dimension of (5\*1\*1) which is placed on the input shape of (20\*5\*1). After that a maxpool layer is applied followed by another CONV2D layer and so on. Finally a softmax layer is used at the end to classify between the 10 classes. We have used the adam optimizer which is the most optimized algorithm to calculate the cost.
* A LSTM model 


