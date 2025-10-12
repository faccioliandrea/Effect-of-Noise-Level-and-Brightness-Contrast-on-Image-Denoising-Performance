The project investigates how **noise level**, **brightness**, and **contrast** interact to influence the performance of two representative denoisers:

- **BM3D (Block-Matching and 3D Filtering)** — a classical, model-based approach exploiting self-similarity and transform-domain filtering.  
- **DRUNet (Deep Residual U-Net)** — a modern neural network denoiser integrating convolutional and residual connections in a U-Net architecture.

Using the **Kodak24** dataset, images are systematically manipulated across multiple brightness and contrast settings, and corrupted with **additive white Gaussian noise (AWGN)** and **Poisson noise** at different intensities.  
Each variant is denoised with both BM3D and DRUNet, producing a large-scale benchmark of denoising outcomes.

Performance will be assessed using:

- **PSNR** – for pixel-wise fidelity.  
- **LPIPS** – for perceptual similarity based on deep visual features.

The study applies **linear mixed-effects models (LMMs)** to quantify the effects and interactions of denoiser type, noise characteristics, and image adjustments on restoration quality.

Current Phase: Implementation
