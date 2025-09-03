# Activity Recognition Project

This repository contains an implementation of human activity recognition using the UCI Human Activity Recognition Using Smartphones dataset.

---

##  Dataset

We used the **UCI Human Activity Recognition Using Smartphones Dataset**:
- This dataset was generated from recordings of 30 subjects performing daily activities (WA LKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) while carrying a waist-mounted smartphone equipped with accelerometer and gyroscope sensors. :contentReference[oaicite:1]{index=1}
- The data includes preprocessed sensor signals, segmented into 2.56-second sliding windows with a 50% overlap, and features extracted in both time and frequency domains.

Dataset download link:
- [UCI HAR Dataset – UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

---

## Data Preprocessing and Merging

In this project, I merged the original training and test splits of the UCI Human Activity Recognition dataset into a single combined dataset for better model training and evaluation.
- We have 2 datasets for training namely S1_Dataset and S2_Dataset used for training
- A test folder which can be used for creating the testing data
- These 3 folders S1_Dataset, S2_Dataset and test dataset has several text files which is merged for the training purpose.


---

##  Modeling Approach

I tried experimenting with several classification algorithms to recognize human activities based on sensor input:

- **Logistic Regression**
- **k-Nearest Neighbors (k-NN)**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**


Each model was trained on the merged dataset and evaluated using appropriate metrics such as accuracy

---

##  Usage

To replicate or extend this project:

```bash
git clone <https://github.com/samruddhichitnis02/Activity_recognition.git>
cd repo-name

# Install dependencies
pip install -r requirements.txt

# Run preprocessing and model routines
- Run the Merge_Files_for_dataset_creation.ipynb file for creating the data if needed
- Use the already created data present in the folder Source_Data and run the individual files from Classification_Algorithms for running the individual algorithms.
