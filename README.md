# Stable-Diffusion-text-to-image

Generated images from text using a pre-trained stable diffusion model (Stable Diffusion v2) on Huggingface.


## Stable diffusion
Stable Diffusion is composed of three major components:  
- Diffusion Model (U-Net)
- VAE
- Text Encoder (Transformer)  
Stable Diffusion can efficiently generate high-resolution images by training a diffusion model on the VAE latent space.
Text Encoder is trained on CLIP.
Text conditioning is performed by Cross-Attention in U-Net.
  
The architecture is such that the diffusion model is placed in the center, flanked at both ends by the VAE Encoder and Decoder. The input text is converted to a vector through the Text Encoder and incorporated from the side of the diffusion model.
