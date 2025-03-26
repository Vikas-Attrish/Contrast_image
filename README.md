# Contrast Stretching using OpenCV

This project implements **contrast stretching** on color images using OpenCV and NumPy. Contrast stretching enhances the image by expanding the pixel intensity range, improving visibility and clarity.

## 📷 What is Contrast Stretching?
Contrast stretching is a simple image enhancement technique that increases the dynamic range of pixel intensities. This improves the visibility of details in images with poor contrast.

## 📋 Project Structure
```
├── contrast(1).ipynb    # Main Jupyter Notebook (Contrast Stretching Code)
├── README.md            # Project Documentation
└── requirements.txt     # Dependencies
```

## 🧰 Requirements
Ensure Python is installed and install the required libraries:

```bash
pip install -r requirements.txt
```

### Dependencies (in `requirements.txt`)
```
opencv-python
numpy
matplotlib
```

## 🚀 How to Run
1. Clone the repository:

```bash
git clone https://github.com/Vikas-Attrish/Contrast_image.git
cd Contrast_image
```

2. Open the Jupyter Notebook:

```bash
jupyter notebook "contrast(1).ipynb"
```

If Jupyter is not installed, you can install it using:

```bash
pip install notebook
```

## 📊 How It Works
1. **Load the Image**: The program reads an input image (e.g., `contrast1.jpg`).
2. **Split Channels**: The image is divided into Blue, Green, and Red channels.
3. **Stretch Contrast**: Each channel undergoes pixel intensity transformation using the formula:

   \[ I_{out} = \frac{(I - I_{min})}{I_{max} - I_{min}} \times (255 - 0) + 0 \]

4. **Merge Channels**: The enhanced channels are combined to reconstruct the image.
5. **Display Output**: The original and contrast-stretched images are shown side-by-side.

## 📷 Example Output
The notebook displays the original and enhanced images:

```
Original Image       →       Contrast Stretched Image
```

## 📌 Future Improvements
- Support for grayscale images
- Batch processing for multiple images
- Allow user-defined output ranges

## 🤝 Contributing
Feel free to open issues or submit pull requests for improvements!

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).

