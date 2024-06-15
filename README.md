# Histogram-and-Contrast-Calculation
Experiment with histogram modification approaches, alongside  seeing their effects on images. This aims to provide practical insights into image processing methods for enhancing contrast, essential in fields such as digital photography, medical imaging, and computer vision applications.

# Description
The main aim of this assignment is to experiment with histogram modification approaches, alongside seeing their effects on images. In more details, given an input image, as a first step, the contrast of such an image is to be evaluated. Second, the three approaches (contrast stretching, histogram equalization, and gray-scale transformation) are to be performed in the input image (producing three outputs). Finally, for each of the three outputs, the contrast is re-evaluated. As per that, the following components are to be implemented: 
- Co-occurrence matrix and calculate contrast. 
- Calculate Histograms: 
  - Image histogram. 
  - Cumulative histogram. 
  - Color covering percentage. 
- Modify histogram: 
  - Contrast stretching  
  - Histogram equalization 
  - Gray-scale transformation

# Functions
## Co-occurrence matrix and calculate contrast
In this part, we need to implement two functions as follows: 
### 1. CalculateCo-occurrence 
- Input: 2D array representing the image (feel free to use a predefined function to transform an image into an array). 
- Output: 2D array representing the co-occurrence matrix. 
- Description: Implements the co-occurrence matrix technique (using the North-South orientation).

### 2. CalculateContrast 
- Input: A co-occurrence matrix. 
- Output: The contrast evaluation. 
- Description: Implement the contrast evaluation using the co-occurrence matrix as per the following equation:
  
![COnte](https://github.com/Khaledayman9/Histogram-and-Contrast-Analysis/assets/105018459/d93a4b5f-c0de-475b-8d52-2a81d8d3fecc)


## Calculate Histograms 
Histograms are a useful, statistical, tool utilizable in the domain of images. Hence, in this part, we implement two functions as follows:
### 1. CalculateHistogram
- Input: 2D array representing the image (feel free to use a predefined function to transform an image into an array). 
- Output: 1D array representing the histogram. 
- Description: Calculate the histogram.

### 2. CalculateCumulativeHistogram 
- Input: 1D array representing the histogram.
- Output: 1D array representing the cumulative histogram. 
- Description: Calculate the cumulative histogram.

### 3. GetColorAtPersentage 
- Input: 1D array representing the cumulative histogram, and a percentage value. 
- Output: two numbers representing color intensities. 
- Description: Given a certain percentage (5% for example), get the color intensities at which the percentage is fulfilled at both ends of the cumulative histogram (5% and 95% in this case).


## Modify histogram
In this part, we implement two functions as follows:
### 1. StretchContrast
- Input: 2D array representing the image (feel free to use a predefined function to transform an image into an array), and four numbers representing color intensities. 
- Output: An image presenting the effect of the contrast stretching on the input image. 
- Description: Implement contrast stretching.

### 2. EqualizeHistogram 
- Input: 2D array representing the image (feel free to use a predefined function to transform an image into an array), and two numbers representing color intensities. 
- Output: An image presenting the effect of the histogram equalization on the input image.
- Description: Implement histogram equalization with the modification of tuning the linearization as per the frequency of the given color intensities.
  
### 3. Gray-scaleTransformation  
- Input: 2D array representing the image (feel free to use a predefined function to transform an image into an array), and four numbers representing color intensities. 
- Output: An image presenting the effect of the gray-scale transformation on the input image. 
- Description: Implement gray-scale transformation.

After implementing the functions above, the testing is to be performed on two steps. The first step is to evaluate the pair of color intensities covering the three percentages, 5%, 10% and 15%. Second, each pair of color intensities are to be involved in the modification processes. 

# Technologies:
- Python

- Google Colab
