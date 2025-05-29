

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

