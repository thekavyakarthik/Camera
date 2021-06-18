# Camera

This provides a simple interface, via OpenCV, for configuring and utilizing a camera device, using Python


## Installation Instructions
We will need to install OpenCV with the Python bindings so that we can access laptop cameras via our Python code. Follow the instructions for Windows and Mac.

### Installing opencv (Recommended)
```shell
conda install -c conda-forge opencv
```
Clone Camera, navigate to the resulting directory, and run

```shell
pip install -e .
```

## Usage
Please see the camera tutorial notebookin this repo for details of how to configure your camera.

```python
%matplotlib notebook
from camera import take_picture
import matplotlib.pyplot as plt
img_array = take_picture()  # returns shape-(H, W, C) array

fig,ax = plt.subplots()
ax.imshow(img_array)
```
