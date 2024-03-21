


# Assistive Listening Device

## Project Overview

The Assistive Listening Device is designed to aid individuals with auditory disabilities by canceling external noise and boosting frequencies associated with 
hearing loss. This project utilizes MEMS microphone technology along with Raspberry Pi for audio processing and transmission to an in-ear speaker.

## Introduction


## Implementation

The implementation of the Assistive Listening Device involves the following steps:

- **Audio Collection**: Audio is captured using an IM69D130 MEMS microphone.
  
- **Audio Processing**: The captured audio is processed using Python on a Raspberry Pi 3.

- **Noise Cancellation**: The Assistive Listening Device employs the Wavelet Thresholding Method for noise cancellation, a powerful technique in signal processing. 
This method involves decomposing the audio signal into different frequency components using wavelet transforms, and then selectively removing noise based on certain 
thresholding criteria.

Wavelet thresholding offers several advantages, including its ability to effectively suppress noise while preserving important signal features. The following types of
 wavelets are utilized in this method:

Haar Wavelet: The mathematical function of the Haar wavelet, ψ(x), is defined as:

ψ(x) = 
1/sqrt(2)   for 0 ≤ x < 1/2
-1/sqrt(2)  for 1/2 ≤ x < 1
0           otherwise
The Haar wavelet detects abrupt changes or edges in signals, making it suitable for noise cancellation tasks.

Daubechies Wavelets: Daubechies wavelets are a family of orthogonal wavelet transforms. The mathematical function of the Daubechies wavelet, ψ(x), depends on the specific order of the wavelet (e.g., db1, db2, db3, etc.). For example, the db1 (Haar) wavelet is the same as the Haar wavelet function defined above. Higher-order Daubechies wavelets have more complex mathematical expressions.

Symlets: Symlets, or "symmetric Daubechies wavelets," have improved symmetry properties compared to Daubechies wavelets. The mathematical function of the Symlet wavelet, ψ(x), depends on the specific order of the wavelet (e.g., sym2, sym3, sym4, etc.).

Bi-orthogonal Wavelets: Bi-orthogonal wavelets use two separate sets of wavelet functions for decomposition and reconstruction. The mathematical functions of the bi-orthogonal wavelet pairs, ψ(x) and φ(x), are often denoted as ψ(x) and φ(x). These wavelets offer greater flexibility and control over the wavelet transform process.

By leveraging these wavelet functions and the wavelet thresholding method, the Assistive Listening Device effectively removes unwanted noise from the audio signal, improving the overall auditory experience for users with auditory disabilities.
	

- **Frequency Shaping using Filter Banks**: In addition to wavelet thresholding, the Assistive Listening Device employs frequency shaping using filter banks. Filter 
banks are used to divide the audio signal into different frequency bands, allowing for selective amplification or attenuation of specific frequency components.

Filter banks consist of multiple bandpass filters arranged in parallel, each covering a specific frequency range. By adjusting the gain of individual filters, the 
frequency response of the audio signal can be shaped to enhance or suppress certain frequencies.

This frequency shaping technique is particularly useful for boosting frequencies associated with hearing loss while attenuating background noise. By customizing the 
gain of each filter in the filter bank, the Assistive Listening Device can adapt to the specific auditory needs of the user, providing a personalized listening 
experience.

- **Wireless Transmission**: The processed audio is wirelessly transmitted to the in-ear speaker for playback.

## Technologies Used

- **Python**: Utilized for implementing signal processing algorithms and data manipulation.
  - **Libraries**: 
    - pywavelets and pywt for wavelet transform-based processing.
    - numpy for numerical computations.
    - scipy for scientific computing and signal processing.
- **Raspberry Pi 3**: Serves as the processing unit for audio data.
- **IM69D130 MEMS Microphone**: Used for capturing audio input.

# Performance and Results








## Conclusion

The Assistive Listening Device effectively integrates advanced technologies to address the needs of individuals with auditory disabilities. By leveraging MEMS 
microphone technology, Python signal processing libraries, and the computational power of the Raspberry Pi, the device enhances the auditory experience by canceling 
external noise and boosting frequencies. This demonstrates a promising solution for improving accessibility and enhancing the quality of life for users with auditory
 impairments.

## References


## Project Mentors
1. [Chandan Padmashali](https://github.com/CHANDAN-2003)
2. [Omkar Patil](https://github.com/Omi729)
3. [Shubham Swadi](https://github.com/shubham-swadi)

## Project Mentees
1. Aniruddh Kamath
2. [Madhav Kedia](https://github.com/madhavkedia018)




