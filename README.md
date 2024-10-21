# Machine Learning Assignment: Analyzing Injection Scenarios

## Overview
This assignment explores the application of machine learning techniques to analyze different injection scenarios using RPM and Speed data. We employed both unsupervised learning models, including K-Means clustering and Hidden Markov Models (HMM), to identify underlying patterns and assess the model performance against known attack labels.

## Models Used
- **K-Means Clustering**: A clustering algorithm used to group data points based on their features (RPM and Speed). 
- **Hidden Markov Models (HMM)**: A statistical model that assumes an underlying process generating observed data through hidden states.

## Key Findings
1. **Model Performance**:
   - **No Injection** scenario showed the best performance with an accuracy of **0.67** for both RPM and Speed.
   - **RPM Injection** struggled, achieving **0.00** accuracy for RPM and only **0.24** for Speed, indicating difficulties in pattern recognition.
   - **FFF Injection** exhibited low accuracies as well, with **0.16** for RPM and **0.00** for Speed.

2. **Observations**:
   - The models performed better in the absence of injections, suggesting that certain injection types may obscure patterns within the data.
   - There is a need for improvement in model performance, particularly in the more complex scenarios.

## Lessons Learned
- **Shortcomings of Unsupervised Learning**:
  - Unsupervised models like K-Means and HMM may not adequately capture the structure of the data, especially when clear labels are absent.
  
- **Improving Model Performance**:
  - Feature engineering to enhance data representation.
  - Incorporating labeled data through semi-supervised learning methods.
  - Exploring advanced algorithms or ensemble methods for better predictions.

## Conclusion
This assignment underscored the importance of selecting appropriate modeling techniques for specific problems and highlighted the challenges associated with unsupervised learning in the presence of complex data distributions. Future work may involve refining the dataset and experimenting with supervised learning approaches to enhance predictive performance.

## Installation
To install required packages, use the following command:
```bash
pip install -r requirements.txt
