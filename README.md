# pcc-octree-jpeg

This is the octree-jpeg codec developed for the MPEG PCC CfP 
It uses an octree to compress the geometry information 
It maps the attribute data to an image using space filling curve, 
first converting 3D to 1D and then to a 2D image. 
The images are encoded using JPEG or PNG 
The png files can be further compressed using bpg image codec using x265.
This is the method for lossy attribute color coding.
The lossless geometry compresssion is comparable state of art in MPEG 
The attribute coding performance is slightly worse, but has the benefit of reusing existing
image coders. For help on usage run octree-jpeg --help. 
Only the windows 64 bit executable is provided for running the codec.   

The algorithm is based on the paper, with improved entropy encoding and png mode: 
Rufael Mekuria, Kees Blom, Pablo Cesar
Design, Implementation, and Evaluation of a Point Cloud Codec for Tele-Immersive Video 
IEEE Transactions on Circuits and Systems for Video technology
 Volume: 27, Issue: 4, p 828 - 842   April 2017 
