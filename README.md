# Image Compression Using K-Means Clustering

## project overview

This project focuses on image compression through the **K-Means clustering algorithm**. The method works by reducing the total number of colors in an image, which allows for efficient compression while preserving overall visual quality. It achieves this by grouping similar pixel colors in RGB space and replacing them with their nearest cluster centers.

## Process

1. **Load the Image**: Import and visualize the original image.
2. **Data Preparation**: Convert the image into a 2D matrix where each row corresponds to a pixel represented by its RGB values.
3. **Apply K-Means Clustering**:

   * Randomly select initial centroids from the dataset.
   * Assign each pixel to the closest centroid.
   * Update centroids by averaging the pixels in each cluster.
   * Repeat until the set number of iterations is reached.
4. **Rebuild the Image**: Replace each pixel with the color of its assigned centroid and reshape the data back to the original image size.
5. **Output**: Display and save the final compressed image.

## Key Features

* Handles compression of multiple images.
* Allows customization of the number of colors (K).
* Provides both visualization and storage of compressed results.
* Implements clustering efficiently using vectorized computations.

---

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

