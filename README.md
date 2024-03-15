This CNN was built as a final project for a course at UBC, CPEN355: Machine Learning with Engineering Applications.<br>
</br>
Using in-class knowledge from CPEN355 and CPSC330 (Applied Machine Learning), self-teaching and independent review of academic papers, I constructed a convolutional neural network with PyTorch. 
By relying on intuition and common guidelines for design-decisions and hyperparameter tuning with 5-fold cross validation, I achieved a 98% accuracy for three-way classification (Covid-19, Normal, Viral Pneumonia) on an [X-Ray image dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset/data) from Kaggle.

Please see my report for a detailed description on how this model was built.

### Summary of Methodology
<b>1. Data Preprocessing & Exploration</b>
  - Preparing and transforming data for input to a CNN
  - Exploring data to observe and trends or patterns in data
    
<b>2. Designing Model</b>
  - Selecting general model architecture
  - Roughly choosing types, amounts and dimensions of layers based on widely known guidelines

<b>3. Cross Validation & Tuning</b>
  - Fine-tuning hyperparameters and evaluating performance with K-Fold Cross Validation
  - Introducing additional hyperparameters and components

<b>4. Final Model Training & Testing</b>
  - Train final model on entire training set with selected hyperparameters
  - Evaluate performance on unseen test set
    
### Further Considerations
- Optimization of architecture:
  - reduce the number of parameters present in the network by changing the kernel size and/or the amount of convolutional layers.
  - use principal component analysis to significantly reduce the dimension of the model's input.
- Consider other existing models or architectures
  - In agreement with the feedback from my professor, I could compare my model's performance and architecture with other ML models to spot areas for improvement
  - Combine my model with other models by applying ensemble methods. An example of this is this [model](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9080057/), which combines a DenseNet with a model following a VGG16 arhictecture.

