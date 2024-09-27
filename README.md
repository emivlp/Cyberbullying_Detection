# **Cyberbullying Detection and Topic Modeling Using Machine Learning and NLP**

## **Project Overview**
This project focuses on the detection of **cyberbullying** using advanced **Natural Language Processing (NLP)** and **Machine Learning** techniques. By leveraging modern pre-trained language models, text preprocessing, and topic modeling, this analysis provides a comprehensive study of how harmful content can be identified, categorized, and understood within social media data.

## **Objectives**
- **Cyberbullying Detection**: Build and evaluate classification models using machine learning techniques to detect cyberbullying in tweets.
- **Topic Modeling**: Apply **Latent Dirichlet Allocation (LDA)** to uncover hidden topics in the tweets and gain insights into the main themes and issues discussed.
- **Model Comparison**: Compare various machine learning models, including **DistilRoBERTa**, **Logistic Regression**, and **Random Forest**, to identify the most effective model for this task.
- **Feature Importance**: Analyze and visualize the most important features contributing to the classification of cyberbullying.

## **Dataset**
The dataset used in this project consists of tweets labeled as either **cyberbullying** or **non-cyberbullying**. Each tweet is categorized based on specific types of harmful content such as **religion**, **ethnicity**, **age**, or **gender-based bullying**.

## **Models Used**
1. **DistilRoBERTa**: A lightweight transformer-based model used for binary classification (cyberbullying vs. non-cyberbullying).
2. **Cardiff NLP (Twitter-RoBERTa for Hate Detection)**: A pre-trained model specifically designed to detect hate speech on social media.
3. **Logistic Regression** and **Random Forest**: Traditional machine learning models used for comparison with modern transformer models.

## **Techniques**
- **Preprocessing**:
  - **Text Cleaning**: Replacing emojis, handling contractions, lowercasing, and tokenization.
  - **Class Balancing with SMOTE**: The **Synthetic Minority Over-sampling Technique (SMOTE)** is used to balance the classes in the dataset to avoid model bias toward the majority class.
- **Topic Modeling with LDA**: **Latent Dirichlet Allocation (LDA)** is used to extract hidden topics within the tweets, providing deeper insights into the nature of cyberbullying.
- **Evaluation Metrics**:
  - **Accuracy**, **Precision**, **Recall**, and **F1-Score** were calculated to evaluate the effectiveness of the classification models.
  - **ROC-AUC**: Used to understand the model’s ability to distinguish between the classes.

## **Model Comparison**
- **DistilRoBERTa** demonstrated a strong balance between precision and recall, achieving an F1-score of **89.29%**.
- **Cardiff NLP (Twitter-RoBERTa)** excelled in precision but had lower recall for non-cyberbullying tweets, resulting in a high F1-score for detecting harmful content but missing some non-bullying cases.
- **Logistic Regression** and **Random Forest** also performed well, with **Random Forest** achieving an F1-score of **92%** for the cyberbullying class.

## **Key Findings**
1. **DistilRoBERTa** provides a strong balance between precision and recall, making it an excellent choice for detecting both cyberbullying and non-cyberbullying tweets.
2. **LDA Topic Modeling** revealed the most common themes and issues in the dataset, such as **hate speech**, **gender-based bullying**, and **ethnicity-related content**. These topics could be further used to improve classification models.
3. **SMOTE** helped balance the class distribution and improved the overall performance of the models by addressing the **class imbalance** in the dataset.

## **Visualizations**
- **Topic Visualization with pyLDAvis**: The top 10 topics were visualized using **pyLDAvis**, showing the 30 most relevant words and the spread of topics across the dataset.
- **Feature Importance for Random Forest**: Key features contributing to the detection of cyberbullying were identified and visualized, aiding in understanding how the model classifies tweets.

## **Future Work**
- **Fine-tuning Pre-trained Models**: Continue exploring and fine-tuning models like **DistilRoBERTa** or other social media-focused transformers to further improve recall and precision.
- **Exploring Alternative Approaches**: Investigate other techniques such as **BERT**, **XLNet**, or **GPT-based models** to compare performance.
- **Advanced Data Augmentation**: Apply more sophisticated data augmentation techniques to generate synthetic tweets and enhance the training dataset.

## **How to Use**
1. Clone this repository and install the necessary dependencies.
2. Load the dataset using the provided data loading function.
3. Run the **preprocessing** and **topic modeling** scripts to clean and analyze the text data.
4. Train and evaluate the **classification models** to detect cyberbullying.
5. Visualize the topics and feature importance using **pyLDAvis** and **matplotlib**.

## **Conclusion**
This project demonstrates how modern NLP techniques, such as transformer-based models and topic modeling, can be effectively applied to the task of detecting **cyberbullying** in social media data. By analyzing both the content and the hidden themes in the tweets, we can develop models that not only detect harmful behavior but also provide insights into the nature of the content, enhancing both prediction and interpretability.

---

### **Author**: [emivlp]  
### **Date**: [September 2024]  
### **Contact**: [https://github.com/emivlp]  
