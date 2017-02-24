An implementation of two famous edge detectors
===================

Canny edge detector
-------------

Description
-

The Canny edge detector uses a multi-stage algorithm to detect a wide range of edges in images. It was developed by John F. Canny in 1986. Canny also produced a computational theory of edge detection explaining why the technique works.

Steps Involved
-

- Applying Gaussian filter to smooth out the image
- Finding intensity gradients from given image
- Applying non-maximum suppression to remove spurious response to edge detection
- Applying double threshold to determine potential edges
- Track edge by hysteresis: Finalize the detection of edges by suppressing all the other edges that are weak and not connected to strong edges (not done)

Motivation
-------------
John Canny's paper on 'A Computational Approach to Edge Detection' [ https://pdfs.semanticscholar.org/55e6/6333402df1a75664260501522800cf3d26b9.pdf ]

Result
-------------
![canny result](https://github.com/adl1995/edge-detectors/blob/master/result-canny.png)

![marr hildreth result](https://github.com/adl1995/edge-detectors/blob/master/marr-hildreth-edge.py)

How to run
-------------

To run this program you need the following libraries installed:

 - Matplotlib
 - Skimage
 - Numpy
 - mpl_toolkits

Clone this repository using 
> git clone https://github.com/adl1995/edge-detectors.git

After this, just open up a terminal and type
> python canny-edge.py
> python marr-hildreth-edge.py


