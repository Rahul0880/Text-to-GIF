# Text-to-GIF Animation Using Stable Diffusion 

This project demonstrates the generation of a dynamic GIF animation using the **Stable Diffusion** model. By interpolating between latent vectors, it creates smooth transitions between frames, resulting in visually appealing animations based on a given text prompt.

## Features

- Utilizes the `stabilityai/stable-diffusion-2` model for generating high-quality images.
- Implements smooth latent space interpolation for realistic transitions.
- Enhances animation smoothness with a moving average filter.
- Generates GIF animations with customizable frame counts and durations.

## How It Works

1. **Prompt Definition**: Specify a text prompt to guide the animation generation.
2. **Latent Space Interpolation**: Smoothly transitions between initial and final latent vectors.
3. **Frame Smoothing**: Applies a moving average for seamless visual transitions.
4. **GIF Creation**: Compiles the generated frames into an animated GIF.

## Example

Using the prompt:

```
"A dog playing in a park, running through grass in one direction"
```

The project produces a 40-frame animation that depicts a dog running through the grass.

## Dependencies

- `torch`
- `diffusers`
- `Pillow`
- `numpy`

Install them with:

```bash
pip install torch diffusers pillow numpy
```

## Running the Code

1. Ensure a CUDA-compatible GPU is available.
2. Run the script to generate a GIF based on your specified prompt.
3. The output file will be saved as `dogrunning.gif`.

## Customization

- **Change the prompt** to create animations on different themes.
- Modify `num_frames` to adjust the animation length.
- Adjust the `guidance_scale` or `num_inference_steps` for creative variations.

## Output

The generated GIF animation will be a smooth depiction of the prompt with dynamic motion.
