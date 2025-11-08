[[dsp]]

# Building the simplest possible automatic gain control (AGC) for auto-regulated feedback

Feedback is the basis of many audio applications; installations, effects, instruments and such.

To be able to work with feedback without letting a system become unstable (think of a microphone feeding back into the speaker causing a crowd to close their ears) one can develop a system with automatic gain control (AGC for short). This system would sense approaching instability (auditory danger) and reduce the volume to prevent the amplitude rising to infinity.

Another use of AGC in the case of feedback is thinkable, namely for systems in which feedback is valuable. Think for example of Karplus-Strong synthesis, where a delayed signal is fed back to the input to create a musical frequency. 
In some cases it is necessary to keep a specific level to make sure the feedback doesn’t die out. Here the AGC is helpful again in sensing if the level is too low and then amplifying the signal.

In this case we will be building a very aggressive AGC that can be used to tame signal feedback in the digital domain, using concepts from digital signal processing.


Gain
Gain determines how much the signal's amplitude is increased or decreased. It can be written using the difference equation:

 	y[i] = ⍺  * x[i]

Where y[i] is the output at the current sample and x[i] the input. ⍺ is the amplitude or gain value. This is the value we want to change automatically depending on the amplitude of the final signal.


Analysis
To be able to determine wether we have to reduce or amplify a signal and by how much we need a clear idea of how loud the initial signal is.
We will be measuring the amplitude at the input of our AGC module. The simplest way to measure amplitude over a small amount of time is to take the average.
Let us assume our input signal is in the value range [-1, 1]. 
The first step to be able to take the average in the correct way is to make all numbers positive. If we don’t do this the average value will probably be somewhere around zero. So before taking the average we should get the absolute value of the input. 
An important choice in the analysis stage is the size of the analysis. The smaller amount of samples used for the analysis, the faster our AGC will react. Too small an amount of samples gives an unrealistic view of the current amplitude.
Depending on the sample rate used, a fine aggressive AGC uses around 100 samples. This can be written like this:

	𝐴 = 1/n Σ | x[i] |

Where 𝐴 is the average value and n is the size of the calculation.

Note: dependent on the goal in mind a more suitable and sophisticated method is analysis using the RMS value.


Calculation
Now that we know our average input amplitude we have to extract a logical amount of attenuation/ amplification.
Before we can do this it is important to have a goal amplitude in mind. Let’s call this value ɣ. 
The simplest formula to determine the gain we need is:

	⍺ = ɣ / 𝐴

where:
	⍺ is the final gain value
	ɣ is the goal amplitude
	𝐴 is the analysed input amplitude

We can try with an example, let’s say:
	our analysed amplitude is 0.4;
	we want our amplitude to stay around 0.6.
The gain we need to apply is:
	⍺ = 0.6 / 0.4 
	= 1.5
	
This makes sense because if we would multiply our analysed amplitude by our computed gain value we would get our goal amplitude value:

	0.4 * 1.5 = 0.6


Application to input signal and smoothing
Of course if we would change the gain to our input every 100 or so samples just like that we would be hearing clicks or other effects. 
This is why we need to interpolate between the changing gain values. The way this is done also can be important for the observed speed of the effect, but again the simplest way is to take the average of two values:

	value = (old value + new value) / 2

Eventually after having computed this new gain value the last step is to multiply the gain value with the input signal:

 	y[i] = ⍺  * x[i]


Conclusion
This algorithm for AGC is suitable for applications where feedback needs to be reduced/ amplified in a very practical way. It would maybe be less suitable for gain control of dialogue or radio signals as are the other uses of AGC.

#dsp 
#pisanje 