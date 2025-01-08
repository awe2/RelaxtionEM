# Laplacian Relaxation vs Physically Informed Neural Network

### Purpose:

This Repository houses a single jupyter notebook that will demonstrate the relaxation method for finding a numerical solution to Laplace's equation on a 2D grid with user defined boundary conditions. The notebook was developed for Phys 7401 Spring 2025 to learn more about this method

In addition to demonstrating the Relaxation method, I also show how to use a neural network to find a numerical solution using a Physically Informed Neural Network (PINN), which is a developing technique used to solve more complicated fields.

I have also included a ChatGPT translation of the Mathematica file that Yuri released. At time of writing, I have not verified it line-by-line to be an exact replica of Yuri's, or that it even runs. Nonetheless, it might be useful for those unfamiliar with Mathematica.

### Installation

To use this repository, you will need a virtual environment with the neccessary python packages installed. I have included a conda environment.yml file that will aid that installation:

```bash
#remember to replace $ENV with your env name
conda create --name $ENV --file environment.yml
conda activate $ENV
```

I haven't actually evaluated that this installation works to get all neccessary dependencies. The dependencies are numpy matplotlib jupyter and PyTorch otherwise.

### Conclusion

While obviously a problem as simple as this doesn't really require a PINN solution, and the error + computational efficiency of the PINN compared to the Relaxtion method is very poor, PINNs are being investigated for more complicated problems or more generally to learn functions with arbitrary constraints. I encourage the reader to play around with the hyperparameters of the Network, as you'll find slight deviations can cause the PINN to no longer converge.

### Author:

Andrew Engel, engel.250@osu.edu