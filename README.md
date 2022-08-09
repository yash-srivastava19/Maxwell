# Maxwell
A Perceptual Hashing program for Media(Image, Audio, Video)

## Improvements on ImageHash
From one of my own repositories - I bring an upgraded version of the ImageHash - Maxwell. Maxwell uses pHash to create fingerprints of the media that is presented to it. 

### What's new in Maxwell?
Maxwell is twisted take on One Shot Frequency Dominant Neighborhood Search(https://www.sciencedirect.com/science/article/pii/S0262885621001505). The scheme provided in the paper is a bit modified to generate fingerprint for an image. There are two fingerprint that are generated - one long one, and one a short one.


### Why did ImageHash needed improvement ?
I loved the implementation of the ImageHash - it went through various iterations of development before being released. The problem however was one my assumptions. I wanted to create the avalanche effect of cryptographic hash functions for images. Well it completely makes sense - even a small change should produce a different fingerprint. What is it that was missing ? There is nothing wrong with the implementation of ImageHash, but I think it is time to move on for a new, better approach

Going through a quick revision of the implementation made me realize the problems with it - and also I came across Perceptual Hashing which I was, atleast in a naiive way trying to implement. Maxwell does not reinvents the whell - and make use of libraries for its approach.

 ### What is Perceptual Hashing ?
 Perceptual Hashing plays an important role in many fields of computer vision such as : image authentication, image description or image copy detection. Perceptual hashing algorithms make use of DCT(Discrete Cosine Transform),DWT(Discrete Wavelet Transform) or DFT(Discrete Fourier Transform). Ideally, the hashing should be robust against certain types of attacks : noise addition, scaling, rotating, watermarking etc.
