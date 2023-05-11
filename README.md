# Audio-classification-
## Objective :
the goal of this project is to utilize cnn and lstm to fit the audio data so we could see the evluation of each model 

## Requirements:
-sklearn 

-Tensorflow

-librosa

## Approach 

#### With Convolutional Neural Networks Model :
After loading the data we will try to visualize it to the freqency of the signal per time and we will see the signal spectogram 

Signal Plot: also known as a waveform plot,it displays the amplitude of a signal over time  and It represents the variation of the signal's amplitude along the horizontal time axis.

A spectrogram plot : is a visualization that shows how the frequency content of a signal changes over time and It provides a 2D representation of the signal's frequency components as they vary with time.

![Alt text](https://github.com/menna566/Audio-classification-/blob/main/specto-signal.png)


the First signal plot : the x-axis typically represents time, and the y-axis represents the amplitude or intensity of the signal "energy"
it represents the changes in amplitude correspond to changes in the sound's intensity or volume as it shows us a sense of how loud or quiet a clip is at any point in time, but it gives us very little information about which frequencies are present.

The second spectrogram plot: it displays the signal in the Frequency domain since the x-axis shows the range of frequency values of the signal at a moment in time and the intensity of it represents the power and magnitude of the signal at each time-frequency so The brighter the intensity the higher the energy of the signal 

then we applied Convolutional Neural Networks on the provided data as we see below :

![Alt text](https://github.com/menna566/Audio-classification-/blob/main/accuracy.png)

#### with LSTM Model 
we used librosa as We will be reading sound file with the help of librosa library which will convert sound file into time series y, represented as a one-dimensional Numpy floating point array and we adjusted the dimensions to apply LSTM Model as we see below :

![Alt text](https://github.com/menna566/Audio-classification-/blob/main/accuracyyy.png)

## Results :

CNN Model fit the data efficiently as we see below :

![Alt text](https://github.com/menna566/Audio-classification-/blob/main/model.png)


But unfortunately LSTM Modl tried to overfit the data as we see below :

![Alt text](https://github.com/menna566/Audio-classification-/blob/main/lstm.png)

in the future work we will solve the overfitting problem but we have for now CNN Model as the Good one





