                FATHIMA HASHMATH 
               -D25

---

### **Title**: 
**Telecommunication Facility Data Analysis**

The project analyzes telecommunication facility data in San Francisco, aiming to uncover patterns and insights.

---

### **Results & Model Evaluation**:

1. **Exploratory Data Analysis (EDA)**:
   - Basic statistics and visualizations provided insights into the distribution of telecommunication facilities by type and location.
   - A bar chart visualized the count of different facility types, helping identify the most common types.
   - Scatter plots were used to assess the geographical distribution based on latitude and longitude.

2. **Data Preprocessing**:
   - Missing values in the location column were dropped to ensure the integrity of spatial data. 
   - No significant data transformation was required as the dataset mainly contained categorical and geographical features.

3. **Clustering Models**:
   - **K-Means Clustering** was used to group facilities based on their geographic coordinates. After experimenting with different cluster numbers, the best separation was achieved using 3 clusters.
   - Results showed clear geographic clusters, which helped visualize facility density across San Francisco.
   
4. **Classification Models**:
   The project explored several classification models:
   
   - **Logistic Regression**:
     - Test accuracy: Moderate but provided a simple linear boundary between categories.
   
   - **Random Forest**:
     - **Test Accuracy**: One of the highest-performing models with substantial predictive power across various facility types.
     - **Precision** and **Recall** were also robust, indicating its ability to handle imbalanced classes well.
     - **F1 Score** was balanced, showing a good tradeoff between precision and recall.

   - **Support Vector Machine (SVM)**:
     - Performed well in terms of accuracy but struggled with recall for some facility types.
     - **Precision**: High precision but lower recall meant the model was conservative in predictions.

   - **Multi-layer Perceptron (MLP)**:
     - Neural networks yielded moderate performance, with a focus on non-linear relationships between variables.
     - Test accuracy was decent, but the training time was significantly higher than other models.

   - **K-Nearest Neighbors (KNN)**:
     - **Test Accuracy**: Comparable to SVM but took longer to train due to the large dataset and high dimensionality.

---

### **Evaluation Metrics**:

The models were evaluated using standard metrics:
- **Accuracy**: Measured the overall correctness of the model’s predictions.
- **Precision**: Indicated how well the model predicted positive cases.
- **Recall**: Assessed the model’s ability to capture all relevant positive cases.
- **F1 Score**: A harmonic mean of precision and recall, showing balance in model performance.
- **Confusion Matrix**: Illustrated true vs. predicted outcomes, helping identify misclassifications.

---

### **Best Model**:
Based on the performance evaluation:
- **Random Forest** emerged as the best-performing model, excelling in terms of accuracy, precision, recall, and overall model stability.
- **K-Means Clustering** successfully grouped facilities geographically, helping visualize the spatial concentration of telecommunication infrastructure.

---

### **Conclusion**:

- **Key Findings**:
   - The telecommunication facilities in San Francisco show distinct geographical clusters, indicating dense facility areas.
   - Random Forest showed the best predictive power among classification algorithms, making it ideal for future predictions on facility types.
   
- **Limitations**:
   - Imbalanced data in facility types posed a challenge, especially for models like Logistic Regression.
   - Some models, like SVM, struggled with recall, suggesting further hyperparameter tuning is required.

---

### **Future Work**:
- **Improvement Areas**:
   - **Data Collection**: More data points, especially from different geographical locations, could improve model generalization.
   - **Deep Learning**: Testing advanced neural networks might yield better accuracy for predicting telecommunication facility types.
   - **Address Imbalance**: Applying techniques like SMOTE (Synthetic Minority Oversampling) to balance the dataset could enhance model performance.

---
