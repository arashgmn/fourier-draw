# Andrew's Hat
This repository is a fork of [fourier-draw](https://github.com/staghado/fourier-draw) with a few algorithmic improvements to enhance speed and the final result, namely:

- The Fourier coefficients are not approximated using the FFT algorithm instead of manual integration. This makes finding coefficients blazing fast.
- The points are ordered by traversing over a spanning tree (breadth-first search) constructed from the coordinates extracted from the image. This minimizes the sudden jumps from one point to another. For a large number of points, it takes a few minutes to construct the tree.

# Requirements
Check the `requirements.txt` file. The main packages are:

- cv2
- scipy
- numpy 
- matplotlib
- networkx
- ffpmg (on your machine)


![fast_andrew](https://raw.githubusercontent.com/arashgmn/fourier-draw/refs/heads/master/fast_andrew.gif)
