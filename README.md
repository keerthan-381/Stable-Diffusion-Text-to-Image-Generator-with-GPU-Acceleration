# Stable Diffusion Image Generator

This project is a Jupyter notebook-based implementation of Stable Diffusion for generating high-quality images from text prompts. It uses the `diffusers` library by Hugging Face and integrates with the Stable Diffusion model to produce visually appealing results.

## Features

- Generate images from natural language prompts using Stable Diffusion.
- Run on GPU for faster image generation.
- Customize the output by modifying parameters like `guidance_scale`.

## Requirements

- Python 3.7 or above
- CUDA-enabled GPU and compatible PyTorch version
- Required Python libraries:
  - `torch`
  - `diffusers`
  - `matplotlib`
  - `transformers`
  - `accelerate`

Install all dependencies using:

```bash
pip install torch diffusers matplotlib transformers accelerate
```

## Files

- **`image_generator.ipynb`**: The main Jupyter notebook for generating images.

## Setup and Execution

1. **Clone the repository:**

   ```bash
   git clone git@github.com:keerthan-381/Stable-Diffusion-Text-to-Image-Generator-with-GPU-Acceleration.git
   cd image_generator
   ```

2. **Set up authorization token:**

   Replace `"YOUR_AUTH_TOKEN"` in the notebook with your Hugging Face API token. Obtain your token from [Hugging Face](https://huggingface.co/).

4. **Run the notebook:**

   Open `image_generator.ipynb` using Jupyter Notebook or Jupyter Lab and execute the cells sequentially.

## How It Works

1. **Model Loading:**
   - Downloads and loads the `CompVis/stable-diffusion-v1-4` model from Hugging Face.
   - Configured to use FP16 precision for optimal GPU performance.

2. **Text-to-Image Generation:**
   - Prompts the user to enter a text description.
   - Generates an image using the Stable Diffusion model with the specified guidance scale.

3. **Display Output:**
   - Displays the generated image using Matplotlib.

## Usage

1. Run the notebook and enter your text prompt when prompted.
2. The notebook will generate and display an image based on your input.
