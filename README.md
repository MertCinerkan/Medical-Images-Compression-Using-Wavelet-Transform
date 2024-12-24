# Medical Images Compression Using Wavelet Transform

This project applies wavelet transform techniques to compress medical images such as X-rays, CT scans, and ultrasounds. It evaluates the effectiveness of different wavelet types and levels, optimizing the balance between compression efficiency and image quality.

## Features
- **Wavelet Transform**: Utilizes various wavelet types (e.g., db, sym, bior) for 2D image compression.
- **Global Thresholding**: Applies sparsity norms to compress images efficiently.
- **Detailed Analysis**: Compares energy retention and compression performance across wavelet configurations.

## Requirements
- MATLAB (with Wavelet Toolbox installed)
- Sample medical images (e.g., X-rays, CT scans, ultrasounds)

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/medical-images-compression.git
   ```
2. Open MATLAB and navigate to the project directory.
3. Ensure the required medical image files are available in the project folder.

## Usage
1. Load the medical image you want to compress.
2. Use the provided MATLAB script to apply wavelet transforms and thresholding.
3. View the decomposition tree and compression results for the selected wavelet type and level.

Example script:
```matlab
load('example_image.mat'); % Load the image
wavelet = 'db3'; % Select wavelet type
level = 4; % Select decomposition level
[compressedImage, ratio] = compressImage(image, wavelet, level);
imshow(compressedImage);
disp(['Compression Ratio: ', num2str(ratio)]);
```

## Results
The project includes a detailed comparison of:
- Energy retention across different wavelet types and levels
- Compression efficiency using various sparsity norms (e.g., sqrt, standard)

## Contributing
Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests to enhance the project.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements
- Medical image datasets sourced from [Kaggle](https://www.kaggle.com/) and [The Cancer Imaging Archive](https://www.cancerimagingarchive.net/).
- MATLAB Wavelet Toolbox for providing the essential tools for wavelet analysis and compression.

---

Developed by Mert Çinerkan.

