# Maxwell
A Perceptual Hashing program for Media(Image, Audio, Video)

## Improvements on ImageHash
From one of my own repositories - I bring an upgraded version of the ImageHash - Maxwell. Maxwell uses pHash to create fingerprints of the media that is presented to it. 

### Why did ImageHash needed improvement ?
I loved the implementation of the ImageHash - it went through various iterations of development before being released. The problem however was one my assumptions. I wanted to create the avalanche effect of cryptographic hash functions for images. Well it completely makes sense - even a small change should produce a different fingerprint. What is it that was missing ? There is nothing wrong with the implementation of ImageHash(still really close to my ❤️), but I think it is time to move on for a new, better approach(It is not you, it is me.I swear this is not a breakup 🙂.)

Going through a quick revision of the implementation made me realize the problems with it - and also I came across Perceptual Hashing which I was, atleast in a naiive way trying to implement. Maxwell does not reinvents the whell - and make use of libraries for its approach.
