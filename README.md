# Severo Ochoa Basic Neural Networks 2025
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/basic-neural-network-2025/HEAD)

SO Basics of Neural Networks 2025 school at the IAA-CSIC

For the widespread adoption of these techniques, researchers should be able to design and use their own DL models. Image classification is one of the main applications of DL  in astrophysics and offers a convenient way to learn about neural networks. The de facto standard to tackle this problem is Convolutional Neural Networks (CNN), a concrete deep learning architecture.  This course will serve as an introduction to Deep Learning with four  sessions with the following objectives: understanding the basics of neural networks, getting to know the fundamental libraries and fundamental architectures, learning how to train a CNN, gaining confidence in using CNNs for image classification tasks, and learning how to evaluate their preformance.

The tutor of this school is Dr Francisco Eduardo Sanchez Karhunen (Universidad de Sevilla).

**Summary of Contents**

- Session 1: Deep Learning fundamentals
- Session 2: Convolutional Neural Networks fundamentals
- Session 3: Practical considerations in real-world CNNs
- Session 4: Evaluation

# Agenda

## Thursday, October 16

### Session 1 (9:00 → 12:00) Deep Learning fundamentals

Roots of deep learning techniques. Reasons for layer stacking. Role of weights and activation functions. Layer as a map between representation spaces. Model parameters. Basic structure for classification tasks. Network training as an optimization problem. Weight initialization techniques. Typical loss functions and optimizers. Learning-rate scheduling.

Hands-on lab: Build from scratch a basic multilayer neural network using the Tensorflow-2 library. Sequential mode of layer stacking. Model training to tackle a classical basic image classification problem.

### Session 2 (14:00 → 18:30) Convolutional Neural Networks fundamentals

Drawbacks of classical multilayer networks in image classification tasks. Human brain image handling. Convolutional layers: padding and stride. Types of pooling layer. Kernels for feature map extraction. Kernel stacking. CNNs as an extension of classical stacked layer models. Top layers in CNNs.

Hands-on lab. Build from scratch a basic CNN for image classification using the Galaxy10 dataset.

## Friday, October 17
### Session 3 (9:00 → 13:00) Practical considerations in real-world CNNs

Overfitting in CNNs. Techniques for overfitting reduction: data augmentation and drop-out. Types of data augmentation. Drop-out rates. Transfer learning: concept and usage. Top Pre-Trained models for image classification. Handling large image datasets: ImageDataGenerators.
Hands-on lab: Use of ImageDataGenerators combined with realistic folder structures in image classification problems. Inclusion of data augmentation in our preprocessing pipelines. Add drop-out layers to the CNN design in session 2. Use of transfer learning in a real situation.

There will be coffee breaks available for all participants during the sessions.

### Session 4 (14:00 → 17:00) Evaluation


## Installation

We recommend using [Conda-Forge](https://conda-forge.org/) or [Conda](https://docs.conda.io/en/latest/miniconda.html) with **mamba** for fast environment management.

### Option 1: Install Miniforge (recommended if you don't have conda)

Miniforge is a conda distribution that includes mamba by default and uses conda-forge as the primary channel:

```bash
# Download installer (Linux/macOS)
wget "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"

# Install (follow the interactive prompts)
bash Miniforge3-$(uname)-$(uname -m).sh
rm Miniforge3-$(uname)-$(uname -m).sh

# Restart your terminal or initialize conda manually. These two commands will initialize conda manually.
# (If you didn't install to the default location, adjust the path accordingly)
$HOME/miniforge3/bin/conda init
source ~/.bashrc  # or source ~/.zshrc for zsh users

# Verify installation
mamba --version
```

### Option 2: Add mamba to existing conda installation

If you already have conda installed, you can add mamba:

```bash
conda install conda-forge::mamba
```

# Download the school materials
1. In a terminal, go to your working directory and clone this repository:

```
git clone https://github.com/iaa-so-training/basic-neural-network-2025.git
cd basic-neural-network-2025
```

2. Install the dependencies for the tutorials (replace `mamba` with `conda` if you don't have mamba installed):
```
mamba env create -f environment.yml
```

3. Execute the tutorials

You need to activate the conda environment and initialize a Jupyter Lab session:

```
conda activate iaa_nn
jupyter lab
```

Once everything is installed, you just need to run step 4 to run the tutorials.

You can also launch the tutorials without installation in the free myBinder service by clicking here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/basic-neural-network-2025/HEAD). Note that this is a free service with limited resources, useful to execute and modify the tutorials live, but computationally expensive steps may not be possible.


# Organizing Committee 

- Rainer Schödel (Chair), IAA-CSIC, Spain 
- Laura Darriba, IAA-CSIC, Spain  
- Javier Moldón, IAA-CSIC, Spain 


--- 
This event is supported by the "Center of Excellence Severo Ochoa" award to the Instituto de Astrofísica de Andalucía. We acknowledge financial support from the Severo Ochoa grant CEX2021-001131-S funded by MCIN/AEI/ 10.13039/501100011033 from the Instituto de Astrofísica de Andalucía.
