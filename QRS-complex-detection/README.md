#### QRS complex. 
Finding QRS complexes in the ECG signal is important for a number of algorithmic goals. It directly gives you information about the heart rate and heart rhythm and provides important context when doing more complex processing.

![QRS](/Images/SinusRhythmLabels.png)


### Pan-Tompkins Algorithm

Is an algorithm used to find QRS complexes.

For most event detection tasks like this, we start with preprocessing steps that will boost the signal and suppress the noise. For Pan-Tompkins, we start with the bandpass filter that selects for frequencies in the QRS complex and suppresses frequencies outside of that band. This is followed by a one-sample difference, which is analogous to a derivative operation. 
This will preserve the steep slopes of the QRS complex and attenuate shallower ones elsewhere in the waveform. Next, we do an element-wise square which non-linearly amplifies the larger portions of our signal and makes everything positive. Finally, we do a moving sum over a fixed window length. This takes advantage of the fact the QRS complex has a fixed width of 150ms. If we tune the moving sum window to 150ms, we can fully take advantage of all the energy in the QRS complex, while attenuating other spikes that are shorter or longer than 150ms.

The detection steps are fairly simple. We simply find the peaks in our pre-processed waveform and then threshold them to select for the QRS complexes.