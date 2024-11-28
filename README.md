# Stable Diffusion Model for Face Generation

This repository contains a project implementing a Stable Diffusion model for generating high-quality, realistic facial images. The project explores the application of diffusion models to generate diverse and photorealistic faces, suitable for tasks like artistic creations, synthetic data generation, and research in generative AI.

## 🌟 Features

- Implementation of the Stable Diffusion algorithm for face generation.
- Pretrained model fine-tuned for face-specific tasks.
- Customizable parameters to control image diversity and quality.
- Support for generating images of specified resolutions.
- Efficient performance on GPU-enabled setups for real-time generation.

## 🔧 Installation

### Clone the Repository

```bash
git clone https://github.com/pasquale9197/Stable_diffusion_model_for_face_generation.git
cd Stable_diffusion_model_for_face_generation
```
## Install Required Dependencies

```bash
pip install -r requirements.txt
```
## Download the Pretrained Model Weights
Access the model weights from Hugging Face or the specified link in the repository. Place the downloaded weights in the models/ directory.

## Set Up Your Environment
* Ensure CUDA is enabled for GPU acceleration.
* Verify your Python version is 3.8 or higher.

## 🚀 Usage
Generate Face Images
Run the main script to generate images:
```bash
python generate_faces.py --num_images 5 --output_dir outputs/
```
Customize generation with optional parameters:
* --num_steps: Number of diffusion steps (default: 50).
* --guidance_scale: Degree of adherence to input prompts (default: 7.5).
* --seed: Set a random seed for reproducibility.

## Example
```bash
python generate_faces.py --num_images 10 --num_steps 100 --guidance_scale 8.5 --seed 42
```

## 📂 Project Structure
* models/: Contains pretrained model weights.
* scripts/: Utility scripts for preprocessing, training, and evaluation.
* outputs/: Generated images are saved here.
* notebooks/: Jupyter notebooks for exploratory data analysis and visualization.
* requirements.txt: List of Python dependencies.

## 📊 Results
Generated faces exhibit:

High photorealism with diverse attributes (age, gender, ethnicity).
Customizable styles based on diffusion model parameters.

Sample generated images:

![image047_I](https://github.com/user-attachments/assets/127092c3-3a31-400d-b47e-e760d862eec7)

## 🛠️ Customization
Modify the training script in train.py to fine-tune the model on custom datasets.
Use the config.yaml file to change hyperparameters such as learning rate, batch size, and number of epochs.
