# CyFuture-Project
Text to image generator using stable diffusion 

# Text-to-Image Generation using Stable Diffusion and Diffusers

This project provides a practical demonstration of text-to-image synthesis, leveraging the Stable Diffusion model through the Diffusers library.

## Requirements

- Python 3.7 or higher
- Jupyter Notebook

## Installation

1. Clone the github repository:
    ```sh
    git clone https://github.com/Shrajalkaurav/CyFuture-Project.git
    cd CyFuture-Project
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    venv\Scripts\activate
    ```
## Usage

1. Open the Jupyter Notebook:
    ```sh
    jupyter notebook
    ```

2. Open the `22MCA020-Text-to-image.ipynb` notebook and run the cells to generate images from text descriptions.



## Example

Here is an example of generating an image from a text description:

```python
from diffusers import StableDiffusionPipeline

# Load the pipeline
pipeline = StableDiffusionPipeline.from_pretrained("dreamlike-art/dreamlike-diffusion-1.0")

# Generate an image from text
prompt = "Musician with black guitar"
image = pipeline(prompt).images[0]

# Display the image
image.show()
```
