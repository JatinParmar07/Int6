# Int6

# Iris Classification with KNN

This is a simple machine learning project, where I classified Iris flower species using the famous Iris dataset and the **K-Nearest Neighbors (KNN)** algorithm from `scikit-learn`. I also visualize the decision boundaries to better understand how KNN separates different species in feature space.

## What I did

1. **Loaded the Iris dataset**  
   I used `pandas` to load the dataset from a CSV file.

2. **Shuffled the data**  
   I made sure to shuffle the dataset using `sample(frac=1, random_state=100)` before splitting features and labels to prevent any ordering bias.

3. **Normalized the features**  
   I standardized the features using `StandardScaler` so that each feature has zero mean and unit variance.

4. **Split the data**  
   I split the dataset into training and test sets (75% train, 25% test) using `train_test_split`.

5. **Trained a KNN classifier**  
   I used `KNeighborsClassifier`. I experimented with different values of `k` to observe how accuracy changes.

6. **Evaluated the model**  
   I evaluated the model using **accuracy** and a **confusion matrix**. I printed the results to see how well it performed.

7. **Visualized decision boundaries**  
   I reduced the features to 2D using **PCA** for visualization purposes. Then I plotted decision boundaries using `plt.contourf` and overlaid the training points. I also added a colorbar/legend to map colors to species names.

## Key Learnings

- Standardizing features improves KNN performance because KNN is distance-based.
- Choosing different `K` values will change the accuracies.

