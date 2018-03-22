# Question-Tagging

## Classifying Questions into 5 categories (What, Who, When, Affirmation(Yes/No) and Unknown.

## Approach

1. Text Exploration
2. Text Cleaning
3. Obtaing POS Tags, Identifying Named Entities, Lemmas, Syntactic Dependency Relations and Orthographic Features.
4. Using the obtained properties as features.
5. Using a Linear SVM model on the engineered features.
6. Predict Categories of Unseens Data.

## Results

#### Used an 80:20 test/train split to obtain 96.296% accuracy on test set.
#### Tagged 3000 unseen questions from [here](http://cogcomp.org/Data/QA/QC/train_3000.label)
#### The Tagged.csv files contains the tagged results.
#### The tagging_model.pkl file contains the trained LinearSVM model.
#### We tried a combination of features, results are below

| Variations in Features Used  | Test Set Accuracy |
| ------------- | ------------- |
| Named Entities, Lemmas, POS Tags, Syntactic Dependency, Orthography  | 95.96  |
| Named Entities, Lemmas, POS Tags  | 96.296  |

## References
Classifying What-type Questions by Head Noun Tagging (http://www.aclweb.org/anthology/C08-1061)
