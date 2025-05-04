# Aircraft-Jet-Engine-Damage-Modelling

Aircraft Jet Engine Damage Modelling Using Data Mining and Statistical Techniques
Aircraft jet engine damage modelling is a critical task for predictive maintenance and operational safety in the aviation industry. This project leverages data mining, statistical, and numerical techniques, implemented using Python and Jupyter Notebooks, to analyze and predict engine health. The modelling focuses on two datasets, FD001 and FD004, which are subsets of NASA's C-MAPSS dataset. These datasets provide time-series data from simulated jet engine operations under varying conditions.

# Regression Analysis for Predicting RUL
The first objective of this project is to perform regression analysis to predict the Remaining Useful Life (RUL) of jet engines. RUL prediction is essential for estimating how many operational cycles are left before an engine fails. For this, data preprocessing and feature engineering techniques were applied to clean and transform the raw data into a suitable format. A variety of regression models, including linear regression, ensemble methods, and stacked models, were implemented to predict RUL with high accuracy. The FD001 dataset, which has a single fault mode, was particularly suited for regression due to its simplicity. However, domain knowledge and mechanical expertise were crucial in understanding the sensor data and identifying key features that influence engine degradation, such as temperature, pressure, and cycle count.

# Classification for Failure Detection and Damage Classification
The second objective involves classification tasks, aimed at detecting engine failures and classifying damage levels or fault modes. Two types of classification were implemented:

# 1. Binary Classification 
This was used for failure detection, where the model predicts whether an engine is at risk of failure (high hazard) or not (low hazard). Thresholds for RUL were defined to differentiate between these states, such as classifying engines with RUL below 50 cycles as high risk.

# 2. Multi-Class Classification: This was used for damage classification, which is significantly more challenging. For FD004, which includes two fault modes, the goal was to classify engine damage into multiple categories based on the type and severity of faults. This required careful feature engineering and the use of advanced multi-class classification models such as gradient boosting algorithms and neural networks.
Implementing multi-class classification proved to be more complex due to the increased variability in the data and the need to account for multiple fault modes simultaneously. Unlike FD001, FD004 requires models to distinguish between different fault types, necessitating more sophisticated approaches and deeper domain knowledge.

# The Role of Domain Knowledge
A key aspect of this project was the integration of mechanical expertise and domain knowledge into the modelling process. Understanding jet engine mechanics and failure mechanisms was critical for:
1. Interpreting sensor data and identifying the most relevant features.
2. Setting appropriate thresholds for RUL to define classes for both binary and multi-class classification.
3. Designing feature engineering strategies that reflect the operational behavior of jet engines.

# Summary
This project demonstrates the application of advanced data mining and statistical techniques to model jet engine damage. By leveraging Python and Jupyter Notebooks, regression models were implemented for RUL prediction, while classification models were used for failure detection and damage classification. The project highlights the challenges of multi-class classification, particularly for datasets like FD004 with multiple fault modes, and underscores the importance of domain knowledge in achieving accurate and reliable results.
