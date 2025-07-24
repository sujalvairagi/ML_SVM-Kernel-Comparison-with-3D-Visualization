# ML_SVM-Kernel-Comparison-with-3D-Visualization

This project aims to compare how different Support Vector Machine (SVM) kernels — Linear, RBF, and Polynomial — perform on synthetically generated non-linearly separable data. It includes both 2D decision boundary plots and 3D decision function visualizations, along with accuracy analysis and hyperparameter tuning.




Project Flow 

1. **Imported required libraries**
   Used libraries like NumPy, matplotlib, seaborn, sklearn (datasets, SVC, metrics), and mpl\_toolkits for 3D plots.

2. **Generated synthetic non-linear data**
   Created datasets using `make_moons` and `make_circles` with noise for realistic separation challenges.

3. **Scaled the features using StandardScaler**
   Normalized the feature space to improve SVM performance and margin calculation.

4. **Visualized the data in 2D**
   Plotted scatter plots to observe non-linear patterns that linear classifiers will struggle with.

5. **Trained SVM models individually (no pipeline)**
   Created and trained:

   * Linear kernel SVM
   * RBF kernel SVM
   * Polynomial kernel SVM (degree = 3)

6. **Plotted 2D decision boundaries for all kernels**
   Compared how each kernel separates classes on the 2D plane. Linear failed, RBF and Polynomial succeeded.

7. **Plotted 3D decision function surfaces**
   Visualized how each model transforms the space in 3D using the SVM’s decision function.

8. **Evaluated accuracy and confusion matrices**

   * Linear Kernel Accuracy: 87%
   * RBF Kernel Accuracy: 94%
   * Polynomial Kernel Accuracy: 88%

9. **Tuned hyperparameters using GridSearchCV**

   * Tuned `C` and `gamma` for RBF
   * Tuned `C`, `gamma`, and `degree` for Polynomial
   * Checked for improved performance

10. **Drew final conclusions**

    * RBF performed best overall
    * Polynomial gave good results after tuning
    * Linear was not suitable for non-linear datasets like moons


