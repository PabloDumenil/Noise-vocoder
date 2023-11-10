An open source Noise-Vocoder for pitch degradation.

Algorithm steps :

1. Input Parameters:

   - ‘x’: input signal

2. Envelope extraction:

   - envelope = abs(x)

3. Low-Pass Filtering:
 
   - Smooth the envelope by removing high-frequency components, leaving only the slower amplitude variations.
     
4. Filtering the input signal and the noise 

- Generates white noise with the same length as the input signal.
- Applies a filter bank to both the input signal `x` and the generated noise. 

5. Modulating the input signal bands with the noise bands

6. Multiplying with the extracted envelope

 - Multiplies the envelope with the corresponding frequency band of the filtered noise. 
   (Modulates the noise with the amplitude variations of the input signal)

6. Summing the modulated bands

 - The modulated bands are summed up across all frequency bands.
 

