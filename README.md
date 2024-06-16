# SVM classification of cats and dogs images
 This is a machine learning project that utilizes Support Vector Machine (SVM) algorithms to classify images into categories of cats and dogs, featuring preprocessing steps, hyperparameter tuning with GridSearchCV, and performance evaluation with detailed metrics.
 # DATASET
 The dataset contain images(4955) of cats and dogs. The script reads the images, resizes them to a uniform size (50x50 pixels), normalizes the pixel values, flattens them into a 1D array, and assigns appropriate labels based on the filename.
 Dataset: https://www.kaggle.com/c/dogs-vs-cats/data
 # OVERVIEW
 1. Import Libraries: The code begins by importing necessary Python libraries for data handling (os, numpy), machine learning (sklearn), image processing (cv2), and visualization (matplotlib, seaborn).

2. Set Up Data Path: The path to the training data is set using os.getcwd() to ensure it points to the current working directory.

3. Initialize Lists: Two lists, train_images for storing image paths and features with labels for storing image data and their corresponding labels, are initialized.

4. Load Image Paths: Using os.walk, the code traverses through all subdirectories in the training data path to find and append image file paths to train_images.

5. Image Preprocessing:
   - Each image path is checked to determine if it's a cat or dog based on the filename, assigning a label accordingly.
   - Images are read using cv2.imread, resized to a uniform (50, 50) size, normalized by dividing pixel values by 255, and then flattened into a 1D array.
   - The flattened image data and labels are appended to their respective lists.

6. Convert Lists to Arrays: The lists of features and labels are converted into NumPy arrays for efficient computation and compatibility with scikit-learn.

7. Split Data: The dataset is split into training and testing sets with an 80-20 ratio using train_test_split.

8. Create Pipeline: A pipeline is created with two steps: scaling features using StandardScaler and applying the SVM classifier.

9. Hyperparameter Search:
   - A parameter grid is defined for the SVM classifier, specifying different kernels and regularization strengths to be tested.
   - GridSearchCV is used to perform cross-validation and find the best combination of parameters.

10. Model Training: The best model from grid search is trained on the training data.

11. Model Evaluation:
    - The trained model's accuracy is evaluated on the test set.
    - A classification report provides detailed performance metrics like precision, recall, f1-score for each class (Cat/Dog).
    - A confusion matrix visualized using seaborn shows the true vs predicted labels.

12. Visualization: Finally, a heatmap of the confusion matrix is displayed using matplotlib to visualize the model's performance.
![confusion matrix](https://github.com/Akhila-04-03/PRODIGY_ML_03/assets/159133840/6c9e9b99-5265-4049-b1fd-27ec860813b0)

## Contact Information

For any inquiries or discussions requests, please reach out to me at:

- Email:## Contact Information

For any inquiries or collaboration requests, please reach out to me at:

- Email:## Contact Information

For any inquiries or collaboration requests, please reach out to me at:

- Email: [akhilaraveendranpm@gmail.com](akhilaraveendranpm@gmail.com)
- LinkedIn: [akhilaraveendranpm](https://www.linkedin.com/in/akhila-raveendran-pm))
