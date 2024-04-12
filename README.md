# Quantum Digit GAN 

# Motivation

SOTA Quantum Generative Adversarial Networks have trouble generating high-quality images and usually tend to use lower-resolution images. A lot of the recent QGANs use a smaller version (usually 8*8 or 16*16) version of the MNIST dataset. 
We need the ability for GANs to be able to produce higher-quality images as well. 

Additionally, we want the ability to generate images even when we have a limited number of available qubits to work with. In this project we try to adapt the PatchGAN [1] model to a larger dataset. 

# Methodology
We follow the same Quantum ansatz as proposed in the original PatchGAN paper, but we adapt it for a larger dataset using the number of qubits in a range from 5 to 9. 

We start with a random noise vector and iteratively train the Generator and Discriminator to produce better-quality images.

# Results

**Generating the Digit 0 using 5 qubits**
![Digit0_5qb](https://github.com/AishwaryaHastak/QGAN/assets/31357026/1e28c4fc-e3b7-438c-b81e-8971d3c8778f)


**Generating the Digit 3 using 5 qubits**
![Digit3_5qb](https://github.com/AishwaryaHastak/QGAN/assets/31357026/d009c89d-1f21-4671-8847-abba40cbca3a)


**Generating the Digit 9 using 6 qubits**
![Digit9_6qb](https://github.com/AishwaryaHastak/QGAN/assets/31357026/03c54562-0b46-4a6e-89ef-a53b9445890b)



# References

[1]Huang, He-Liang, et al. "Experimental quantum generative adversarial networks for image generation." Physical Review Applied 16.2 (2021): 024051.
