# deep-learning-challenge
## Alphabet Soup Charity Neural Network Model Optimization

### Background

The Alphabet Soup foundation aims to select applicants for funding with the highest likelihood of success in their ventures. With the help of machine learning and neural networks, a binary classifier has been developed to predict whether applicants will be successful if funded by Alphabet Soup.

### Initial Model 

The initial model utilized the following configurations:
- Input features: All columns except `EIN` and `NAME`.
- First hidden layer: 80 units with ReLU activation function.
- Second hidden layer: 30 units with ReLU activation function.
- Output layer: 1 unit with sigmoid activation function.

The initial model achieved an accuracy of 72.40%.

### Optimization Attempts

To improve the model performance, several optimization attempts were made:
1. **Decreased Cutoff Values**: The cutoff values for `APPLICATION_TYPE` and `CLASSIFICATION` were lowered from 500 and 1000 to 10, respectively, to increase the number of input features.
2. **Variation in Activation Functions**: Different activation functions were explored for the hidden layers, including `relu`, `tanh`, and `softmax`.
3. **Variation in Hidden Layers and Units**: The number of hidden layers and units were varied to explore different model architectures.
4. **Reduced Epochs**: Due to long training times, the number of epochs was reduced to 60 from 100 to expedite model optimization.

### Results

After optimization, the best performing model (referred to as `model2`) achieved an accuracy of 72.66%. 
During the class, additional optimization attempts were made to find the optimal model. 
An `optimization2` was attempted using the same number of epochs (100), but the execution time exceeded 6 hours. To expedite the process, the number of epochs was reduced, resulting in a slightly lower accuracy compared to the previous best performing model.

### Summary

The optimization process involved adjusting input data, exploring different model architectures and activation functions, and reducing training epochs to expedite model evaluation. While the best performing model showed a slight improvement in accuracy, further optimization efforts could be explored to achieve higher accuracy without compromising training time. The saved models (`AlphabetSoupCharity_Optimization.h5` and `AlphabetSoupCharity_Optimization2.h5`) provide valuable insights into the effectiveness of different optimization strategies and serve as a foundation for future model improvements.
