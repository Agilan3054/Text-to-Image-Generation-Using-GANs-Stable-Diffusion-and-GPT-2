# Text-to-Image GAN with GPT-2 & Stable Diffusion

This project integrates **Generative Adversarial Networks (GANs)** with **GPT-2** and **Stable Diffusion** for generating high-quality images from text descriptions. The project leverages **PyTorch** for training custom GANs and **Hugging Face Transformers** for text encoding with GPT-2. Additionally, **Stable Diffusion** is utilized to enhance image synthesis. The complete pipeline is designed to work on CUDA-enabled devices.

## Key Features
- **Text Encoding with GPT-2**: Uses GPT-2 from the Hugging Face library to encode text descriptions into meaningful embeddings that guide the image generation process.
- **GAN-based Image Generation**: A custom GAN architecture generates images from latent noise vectors combined with text embeddings.
- **Stable Diffusion for Enhanced Image Quality**: Stable Diffusion is integrated for refined and detailed image synthesis, leveraging pretrained models for improved visual outputs.
- **Advanced Data Augmentation**: Implements augmentation techniques such as random cropping, flipping, and color jitter to make the model more robust and reduce overfitting.
- **CUDA Support**: Full support for CUDA devices for faster model training and image generation.

## Project Structure
```bash
.
├── generator.py              # Generator model definition
├── discriminator.py          # Discriminator model definition
├── text_encoder.py           # GPT-2 text encoder
├── stable_diffusion.py       # Stable Diffusion integration
├── train.py                  # Training loop with GAN and Stable Diffusion
├── dataset.py                # Dataset and DataLoader setup
└── README.md                 # Project documentation
