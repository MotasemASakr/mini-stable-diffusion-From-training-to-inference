# mini-stable-diffusion-From-training-to-inference

## Mini Stable Diffusion for 16x16 Sprites
Welcome to the Mini Stable Diffusion project repository! This project focuses on training a mini model to generate 16x16 pixel sprites using Stable Diffusion. The model is trained using two different methods: with context (hero, non-hero, food, spell, side-facing) and without context.
Table of Contents

### Table of Contents
- About the Project
- Getting Started
- Training the Model
- Inference

### About the Project
This project aims to leverage the power of diffusion models to generate small-scale sprite graphics suitable for video games. By training on 16x16 pixel images, we can create diverse and detailed sprite assets efficiently. The project explores two training methodologies:
With Context: Incorporates additional labels such as character type or orientation to guide sprite generation.
Without Context: Relies solely on the sprite images themselves without any additional guiding information.

### Prerequisites
To run this project, you will need:
- Python 3.8 or higher
- PyTorch
- Transformers library

### Structure
- Inference: Use diffusion model to generate 16x16 sprites
- Training: Training small diffusion model with U-net
- Training_with_context: Training small diffusion model with U-net on sprites and context dataset to change the output based on the selected context (hero, non-hero, food, spell, side-facing)

### Sampling visualization:


https://github.com/user-attachments/assets/50e5c0c9-c98e-4414-b802-a2da6f61d661



### Generated Image samples:
The following sprites were generated using the following context:
    # hero, non-hero, food, spell, side-facing
    - human hero
    - hero and food
    - food and spell
    - hero and side-facing
    - hero and non-hero
    - hero and spell
<img width="314" alt="inference_samples" src="https://github.com/user-attachments/assets/641769e5-ee27-4863-95d5-4f313979a6bf">


### Acknowledgments
- Sprites by ElvGames, FrootsnVeggies and kyrise
- This code is modified from, https://github.com/cloneofsimo/minDiffusion
- Diffusion model is based on Denoising Diffusion Probabilistic Models and Denoising Diffusion Implicit Models
