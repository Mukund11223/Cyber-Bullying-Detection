# CYBER BULLYING DETECTION
## WEB APP
<img width="1436" alt="Screenshot 2024-11-26 at 9 29 21 PM" src="https://github.com/user-attachments/assets/3e408067-ee0e-45ad-bb3b-225ed7852257">

# PROJECT FLOW

## Data Preprocessing

	•	Label Modification: Convert all -1 labels to 1 for consistency.
	•	Data Cleaning:
	•	Remove user mentions (@username).
	•	Retain alphabetic characters only.
	•	Filter out words with fewer than three characters.
	•	Augmentation: Duplicate the dataset for better generalization.
	•	Lemmatization: Standardize words to their base forms.

## Data Visualization

	•	Pie Chart: Visualize the distribution of toxic vs. non-toxic samples.
	•	Bar Plots: Compare model performance metrics (Accuracy, F1-Score).
 <img width="463" alt="Screenshot 2024-11-26 at 9 25 40 PM" src="https://github.com/user-attachments/assets/37c51507-acf6-42f3-9855-ada5ef5c90a5">


## Feature Extraction

	•	TF-IDF Vectorizer:
	•	Convert text data into numerical vectors.
	•	Remove stop words using stopwords.txt.

## Model Training

Used multiple classifiers:
	•	LinearSVC
	•	LogisticRegression
	•	MultinomialNB
	•	DecisionTreeClassifier
	•	AdaBoostClassifier
	•	BaggingClassifier
	•	SGDClassifier

Performance metrics calculated:
	•	Accuracy
	•	F1-Score
	•	Precision
	•	Recall
	•	Training and Prediction Time

<img width="1122" alt="Screenshot 2024-11-26 at 9 27 03 PM" src="https://github.com/user-attachments/assets/6c48dbb1-11c3-4927-8061-ddf11fc69692">


## Results

Best Classifiers:
	•	Accuracy: DecisionTreeClassifier (0.9723)
	•	F1 Score: DecisionTreeClassifier (0.9788)
	•	Training Time: MultinomialNB (0.012s)
	•	Prediction Time: SGDClassifier (0.002s)

 <img width="1169" alt="Screenshot 2024-11-26 at 9 27 35 PM" src="https://github.com/user-attachments/assets/7d7f5433-a875-4cd7-a665-4f6d54d92329">


## Dataset

- **Source**: `dataset.csv` 
- **Columns**: 
  - `headline`: Text of comments.
  - `label`: Classification labels (`1` for toxic, `0` for non-toxic).
- Total Records: `18,148` (before data augmentation).

----

