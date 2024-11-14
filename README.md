

# JPEG Compressor

This project implements a JPEG compression algorithm in Python using a Jupyter Notebook. The notebook provides step-by-step instructions and code for compressing images by applying the Discrete Cosine Transform (DCT) and quantization techniques. The JPEG compression technique is widely used to reduce the file size of images without significant loss of quality, making it ideal for web and mobile applications.

## Features

- **Discrete Cosine Transform (DCT):** Converts image blocks from the spatial domain to the frequency domain.
- **Quantization:** Reduces the amount of data by approximating DCT coefficients.
- **Inverse DCT:** Reconstructs the compressed image from the quantized coefficients.
- **Image Quality Control:** Allows control over the compression level and quality of the output image.

## Requirements

- Python 3.x
- Jupyter Notebook
- Required Libraries:
  - `numpy` - for efficient array manipulation
  - `Pillow` - for image handling and manipulation
  - `matplotlib` - for visualization

Install the dependencies using:

```bash
pip install numpy pillow matplotlib
```

## Usage

1. Open the notebook file `jpeg_compressor.ipynb` in Jupyter Notebook or JupyterLab.
2. Run each cell sequentially to understand and execute the JPEG compression process.
3. The notebook includes comments and explanations for each step.

### Compression Level

You can adjust the compression level in the quantization step. A higher quantization factor results in higher compression and lower image quality, while a lower factor results in better quality and larger file size.

## How It Works

1. **Read Image**: Load an image and convert it to grayscale for simplicity.
2. **DCT Transformation**: Apply the Discrete Cosine Transform to 8x8 blocks of the image.
3. **Quantization**: Use a quantization matrix to reduce the precision of the DCT coefficients.
4. **Inverse DCT**: Reconstruct the image using the inverse DCT of the quantized blocks.
5. **Result Comparison**: Display the original and compressed images side-by-side to compare quality.


