## Code repository for the courses SCC0251 / SCC5830 *Image Processing*
### Moacir A. Ponti, 2020-1

#### Software Installation (using command line)
install virtualenvwrapper to manage virtual environments

```
pip install --user virtualenvwrapper
```

start the virtualenvwrapper
```
$ source /usr/local/bin/virtualenvwrapper.sh
```

make sure to include this at the shell session startup - usually .bashrc 
```
echo 'source /usr/local/bin/virtualenvwrapper.sh' >> ~/.bashrc
```

in order to create a new environment called venv use:
```
mkvirtualenv venv
```

inside the virtual environment, install all needed python packages
```
(venv) $ pip install numpy
(venv) $ pip install imageio
(venv) $ pip install matplotlib
(venv) $ pip install scipy
(venv) $ pip install jupyter
```

if you want to enter the virtual environment later, just type
```
workon venv
```


#### Running Jupyter Notebook
it opens on your browser in order to create new notebooks or run existing ones
```
(venv) $ jupyter notebook
```

#### Content:
Folder [Images](./images) contains images used in codes

1. [Fundamentals](./01_fundamentals.ipynb): basic libraries, loading images, pixel processing, showing and writing images in disk

2. Enhancement
- [(1) pointwise gray-level](./02_enhancement-pixel.ipynb): image enhancement using pixel-wise gray-level values
- [(2) histogram-based](./02b_enhancement-histogram.ipynb): using histograms to process images

3. Spatial Filtering (Convolution)
- [Convolution](./03_filtering.ipynb): convolution operator, designing filters for spatial processing

4. Fourier Transform and Frequency Analysis
- [(1) Frequency Analysis](./04a_frequency_analysis.ipynb): introduction to the analysis of frequencies
- [(2) Discrete Fourier Transform](./04b_fourier_transform.ipynb): the Discrete Fourier Transform in 1D and 2D
- [(3) Fast Fourier Transform](./04c_fourier_transform_fft.ipynb): the divide and conquer algorithm to implement Discrete Fourier Transform in O(n log n) time

5. Image Restoration 
- [(1) Denoising](./05a_restoration_noise.ipynb): simulating and studying noise, and filtering it out using denoising methods
- [(2) Deconvolution](./05b_restoration_deconvolution.ipynb): the point spread function and inverse problems

6. Colour images
- [(1) Colour Image Processing](./06a_colour_processing.ipynb): colour spaces and processing images
- [(2) Colour Image Description](./06b_colour_description.ipynb): using colour information to extract features from images 

7. Image Segmentation
- [Threshold and Region-based Segmentation](./07_segmentation.ipynb): strategies for threshold-based (histogram) and region-based (pixel) segmentation
