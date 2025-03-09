# Analysis-DL-Medical-Transcription-dataset

This is a revisitation of the original design obtained from Kaggle, trying to optimize as much as possible the analysis (https://www.kaggle.com/code/ritheshsreenivasan/clinical-text-classification/notebook). 

**Description of the Original Project:**

The original project aims to automatically classify medical texts into their respective specialties. The employed methods involve the use of the Tf-Idf technique for text representation, a spaCy model for biomedical entities recognition and Logistic Regression for classification. The process involved initial experimentation on the entire dataset, followed by subsequent reduction of category numbers and the application of SMOTE for class balancing.

**Limitations of the Original Project:**

It selectively used a subset of transcriptions without clear computational justification. The exclusive reliance on the Tf-Idf model for frequency-based analysis overlooked semantic context. Moreover, the application of PCA for complexity reduction was flawed.

**Objective:**

This project aimed to overcome the limitations of the original study through a careful and targeted analysis of the dataset. This included addressing imbalances in the dataset, reducing complexity as needed, and introducing a new Word2Vec model to capture semantic nuances. These refinements aimed to boost overall predictive accuracy and model robustness.

**Method:**

To achieve the objectives of the enhanced project, a meticulous examination of the original pre-processing and code was conducted, assessing its rationale and implementing changes where deemed necessary. Various parameters were systematically tested to optimize predictive performance for logistic regression. The dataset was subsequently tested on a new Word2Vec model, experimenting with various parameters, and evaluating it on processed and reduced data. Initially, the testing involved no vocabulary restrictions, and later, the SpaCy model was applied, specifically adapted for a biomedical context.

**Results:**

Results highlight the significance of category reduction for improved classification performance. Even the original model shows enhanced performance with implemented modifications. Both methods demonstrated high classification accuracy (tfIdf=0.78, W2V=0.79), further boosted by incorporating SMOTE to address class imbalance, especially benefiting minority classes. Notably, PCA had minimal impact on performance improvement. Both models faced consistent classification challenges, attributed to dataset issues rather than inherent model limitations.


Authors:
- alessandro.sandron
- alesia.m@
- nicola.c@
- alessia.r@
- valeria.b@
