# Image Compression Using  Clustering

## Overview
This project demonstrates image compression using the K-Means clustering algorithm. By reducing the number of colors in an image, we can efficiently compress images while retaining visual quality. The approach involves clustering pixel colors in the RGB space and replacing each pixel with its nearest centroid.

## How It Works
1. **Load the Image**: The original image is loaded and visualized.
2. **Preprocess the Data**: The image is reshaped into a 2D array where each row represents a pixel with its RGB values.
3. **K-Means Clustering**:
   - Initialize centroids randomly from the dataset.
   - Assign each pixel to the closest centroid.
   - Compute new centroids based on the mean of assigned pixels.
   - Repeat the process for a fixed number of iterations.
4. **Reconstruct the Image**: Each pixel is replaced with its corresponding centroid color, and the image is reshaped back to its original dimensions.
5. **Save and Display**: The compressed image is displayed and saved.

## Features
- Supports compression for multiple images.
- Customizable number of colors (K) for compression.
- Displays and saves compressed images.
- Efficient clustering using vectorized operations.

## Requirements
- Python 3.x
- NumPy
- Matplotlib
- OS (for handling file paths)

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/image-compression-kmeans.git
   ```
2. Navigate to the project directory:
   ```sh
   cd image-compression-kmeans
   ```
3. Install dependencies:
   ```sh
   pip install numpy matplotlib
   ```
4. Run the script:
   ```sh
   python image_compression.py
   ```
5. View compressed images in the output folder.

## Example
- Original Image: 24-bit color depth.
- Compressed Image: Reduced to 16 or 8 colors using K-Means.
- Achieves ~6x compression by storing only centroid indices instead of full RGB values.

## Results
After applying K-Means clustering, images are compressed while preserving recognizable visual quality. This technique is useful for reducing storage and transmission costs while maintaining an acceptable level of detail.

## License
This project is open-source and available under the [MIT License](LICENSE). Feel free to contribute and improve it!

