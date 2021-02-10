# Generalized-Hough-Transform
Python implementation of the GHT(Generalized Hough Transform) to validate feature-based matches.
The jupyter notebook present a simple case-of-study with one model image and one test image.
This basic approach can be used to implement more complex detection systems, with multiple models and test images.

Implementation choices:
- The BARICENTER of the model image is used as reference point.
- SIFT (Scale-invariant feature transform) is used as features detector and descriptor.
- KDTREE algorithm is used to perform the search of the 2-NN (Nearest Neighbour).
- D.Lowe threshold is set to 0.7 to keep only good matches.
- the PEAK_LOCAL_MAXIMA function is used to find peaks in the AA(accumulator array).
- RANSAC is used to find a roboust homography for the estimation of the bounding-box in the test image.


