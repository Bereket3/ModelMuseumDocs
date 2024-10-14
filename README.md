### 1. **GNCN-t1/Rao (Rao & Ballard, 1999)**
   - **Type**: Unsupervised, hierarchical predictive coding.
   - **Use Case**: This model is used to understand how the brain handles perception. It focuses on minimizing the prediction errors between the brain’s internal model and the external sensory input.
   - **Pros**:
     - Can model complex sensory processes.
     - Efficient for understanding perception-based tasks.
   - **Cons**:
     - Limited scalability to more generalized tasks outside perception.
     - High computational complexity.
    
### 2. **GNCN-t1-Sigma/Friston (Friston, 2008)**
   - **Type**: Unsupervised, predictive coding with free-energy minimization.
   - **Use Case**: Applied in neuroscience, it models perception and action by minimizing "free energy" (i.e., uncertainty) through Bayesian inference.
   - **Pros**:
     - Effective for understanding the brain’s organization of predictions and errors.
     - Incorporates a probabilistic approach, making it robust in uncertain environments.
   - **Cons**:
     - Complex to implement for real-world, large-scale applications.
     - Theoretical, with limited practical applications in AI.

### 3. **GNCN-PDH (Ororbia & Kifer, 2022)**
   - **Type**: Unsupervised, predictive coding-based model.
   - **Use Case**: This model is designed for learning efficient representations and performing inference, especially useful for unsupervised learning tasks like clustering.
   - **Pros**:
     - High efficiency in representation learning.
     - Robust for unsupervised learning with minimal labeled data.
   - **Cons**:
     - Requires careful parameter tuning.
     - Limited versatility outside of unsupervised learning.

### 4. **GNCN-t1-FFM (Whittington & Bogacz, 2017)**
   - **Type**: Supervised, feedforward predictive coding.
   - **Use Case**: Focuses on neural circuits that optimize prediction accuracy, useful for tasks like image recognition.
   - **Pros**:
     - Strong in tasks requiring accurate predictions (e.g., classification).
     - High efficiency with fewer parameters.
   - **Cons**:
     - Works well only when data distribution matches its assumptions.
     - Poor performance with noisy data.

### 5. **GNCN-t1-SC (Olshausen & Field, 1996)**
   - **Type**: Unsupervised, sparse coding.
   - **Use Case**: Applied to sensory data, like natural images, to learn sparse representations.
   - **Pros**:
     - Efficient in capturing key features with a small set of active neurons.
     - Strong in tasks like image compression.
   - **Cons**:
     - Sensitive to noise.
     - Hard to generalize beyond sensory data.

### 6. **Harmonium (Smolensky, 1986; Hinton, 1999)**
   - **Type**: Unsupervised, probabilistic graphical model.
   - **Use Case**: Often used in energy-based models for deep learning, such as Restricted Boltzmann Machines (RBMs).
   - **Pros**:
     - Can model complex high-dimensional distributions.
     - Effective for generative tasks.
   - **Cons**:
     - Training can be computationally expensive.
     - Slow convergence in large datasets.

### 7. **SNN-BA (Samadi et al., 2017)**
   - **Type**: Supervised, spiking neural network.
   - **Use Case**: Used for tasks like pattern recognition, mimicking how neurons in the brain communicate through spikes.
   - **Pros**:
     - Energy efficient and biologically plausible.
     - Works well with real-time data.
   - **Cons**:
     - Difficult to train due to its reliance on timing precision.
     - High complexity for hardware implementation.

### Summary Table:

| **Model**             | **Type**       | **Use Case**                  | **Pros**                                   | **Cons**                                |
|-----------------------|----------------|-------------------------------|--------------------------------------------|-----------------------------------------|
| GNCN-t1/Rao           | Unsupervised   | Perception modeling           | Models complex sensory processes           | High computational complexity           |
| GNCN-t1-Sigma/Friston | Unsupervised   | Brain’s prediction system      | Probabilistic, robust in uncertainty       | Theoretical, complex implementation     |
| GNCN-PDH              | Unsupervised   | Representation learning        | Efficient in unsupervised learning         | Requires careful tuning                 |
| GNCN-t1-FFM           | Supervised     | Classification tasks           | High accuracy, efficient                   | Poor with noisy data                    |
| GNCN-t1-SC            | Unsupervised   | Sparse representation          | Great for image compression                | Sensitive to noise                      |
| Harmonium             | Unsupervised   | Deep learning, generative models | Good for modeling high-dimensional data    | Computationally expensive               |
| SNN-BA                | Supervised     | Real-time pattern recognition  | Energy efficient, real-time capability     | Difficult to train, high complexity     |

### Resource
    - Ngc-learn’s documentation [https://ngc-learn.readthedocs.io/en/stable/]    
