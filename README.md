<p align="center">
  <img src="https://github.com/user-attachments/assets/fc25df40-75a5-433f-a0d9-712153b6490f">
</p>

# GAN for Image Generation (MNIST Dataset)

This repository contains a project focused on generating images using a Generative Adversarial Network (GAN). The project is implemented in Python using TensorFlow/Keras and is trained on the MNIST dataset, a collection of handwritten digits. The model consists of a generator and a discriminator, which work together to produce realistic images of digits.

## Implemented Features

1. ### Data Preprocessing
   - Loading the MNIST dataset and preparing it for input into the GAN. This includes reshaping and normalizing the images.

2. ### Generator Model
   - The generator is a neural network that creates new images from random noise. It attempts to generate images that are indistinguishable from real ones, learning through feedback from the discriminator.

3. ### Discriminator Model
   - The discriminator is a neural network that classifies images as real (from the dataset) or fake (from the generator). It helps the generator improve by providing feedback on the generated images.

4. ### Model Training
   - Both models are trained in an adversarial setup, where the generator tries to produce more realistic images while the discriminator learns to differentiate between real and fake images.

5. ### Image Generation
   - After training, the generator can produce MNIST-looking handwritten digits. The generated images are displayed in a grid format using Matplotlib.

## Tools Used
- **Python**: Main programming language.
- **Python Libraries**: TensorFlow, Keras, NumPy, Matplotlib.
- **Development Environment**: Any Python IDE such as Jupyter Lab or Visual Studio Code.

## Main Project Structure

- **`generativeModelMNIST.ipynb`**: Main script for training the GAN, including both the generator and discriminator models.

## How to Use

1. **Clone the repository**:
    - `git clone <repo URL>`

2. **Install the required dependencies**:
    - `pip install tensorflow numpy matplotlib`

3. **Prepare the MNIST dataset**:
    - The dataset is automatically loaded via TensorFlow, so no manual download is needed.

4. **Run the main script**:
    - Run Jupyter Lab or other IDE
    - Open and run `generativeModelMNIST.ipynb`
        - The script will train the GAN and generate images, which are displayed during and after training.

5. **Customize the Training Process**:
    - Modify hyperparameters such as the **NOISE_DIM**, **learning_rate**, or **BATCH_SIZE** to experiment with different model settings.

## Contributions

Contributions are welcome! Feel free to submit pull requests with improvements, bug fixes, or new features. For discussions and suggestions, please open an issue.
