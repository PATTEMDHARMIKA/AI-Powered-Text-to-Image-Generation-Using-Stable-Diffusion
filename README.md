# AI-Powered-Text-to-Image-Generation-Using-Stable-Diffusion

This project provides a Google Colab notebook for generating images using **Stable Diffusion** without requiring an API key. Users can input text prompts, and the model will generate high-quality images directly in Colab.

## Features

- Generate images from text prompts.
- Fully runs in Google Colab using GPU acceleration.
- No API key required.
- Easy to customize prompt and settings.

## Requirements

The notebook installs and uses the following libraries:

- `diffusers`
- `transformers`
- `torch`
- `accelerate`
- `safetensors`
- `PIL` (Python Imaging Library)

## How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Make sure the runtime is set to **GPU**:
   - `Runtime → Change runtime type → GPU`
3. Run all cells sequentially.
4. Enter your text prompt when requested to generate images.
## Example

```python
prompt = "A futuristic city skyline at sunset, digital art"
generated_image = pipe(prompt).images[0]
generated_image.show()
