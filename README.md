# Noise_Cancelation_Piano
Signal &amp; System Communication Noise cancellation project using python
Milestone 1:
The python script is used to generate a song using 6 pairs of different frequencies from the 3rd and 4th octaves.
First, the required libraries were imported.
Then, the used frequencies were stored in arrays, as well as, the time between notes and the endpoint of each note.
After that, we looped over the arrays, each time generating two signals (one from the 3rd octave and one from the 4th octave), and then adding them to the final result signal.
Counters were used to access the elements of the arrays and were updated each time inside the loop according the corresponding values in the arrays.
Finally, the resulting song is plotted and played.
Milestone 2:
In this part of the project, we are applying the process of noise cancellation using frequency domain conversion.
First, the necessary library is imported.
Then, we set the number of samples and the frequency axis range.
After that, we generate a noise signal by selecting two random frequencies (which are different each time) and adding the generated noise to the original song.
Both of the signals (original and noise contaminated) are converted to the frequency domain.
For the actual process of noise cancellation, we loop over the frequency range and check the amplitude of the noise contaminated signal (in frequency domain).
If it is greater than the maximum amplitude of the original signal, then the corresponding frequency at this index is from the noise signal. 
So, we store the two frequencies in an array and round their values. 
Then, we get the filtered signal by subtracting a signal using the two found frequencies from the noise contaminated signal.
Finally, we get the corresponding filtered signal in the frequency domain and plot all the signals in time and frequency domains. 
The filtered signal is played to make sure it sounds like the original.
