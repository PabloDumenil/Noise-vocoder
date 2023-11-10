# NoiseCocoder

Open source noise-vocoder to degrade the pitch of speech or polyphonic music.

A program to degrade the pitch of a musical fragment. In this experiment, the TV tunes. In order to make proof of concept of this noise-vocoder, we tested it on the Zebra Finch recording we degraded with Matthew Winns' noise vocoder.

The extraction of the envelope of an input signal x was computed by first taking the absolute value of the signal to remove negative values and then applying a Butterworth low-pass filter with a specified cutoff frequency and filter order. This filtering process effectively smoothes the signal, capturing its slow-varying amplitude variations while attenuating high-frequency components. 
