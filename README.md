# SPAM DETECTOR 
Machine learning spam detection using Scikit-learn, NLP preprocessing, and logistic regression. Processes raw email datasets, converts them into word vector features, and achieves over 98% accuracy on test data.
📧 Spam Email Detector
A high-accuracy machine learning system that detects spam emails using the Apache SpamAssassin Public Corpus.
Processes raw email data, extracts meaningful features, and classifies emails as Ham (Non-Spam) or Spam with over 98% accuracy.

📂 Dataset
Ham (Non-Spam) → Legitimate emails

Spam → Unwanted promotional/malicious emails

Source: Apache SpamAssassin Public Dataset

Size: 2,500 ham emails + 500 spam emails

🔹 Workflow
1️⃣ Data Acquisition

Downloaded and organized ham & spam datasets locally.

2️⃣ Email Parsing

Used Python’s email module to extract content & metadata.

Checked MIME types (plain text, HTML, multipart).

3️⃣ Exploratory Analysis

Spam emails contain more HTML, links, and promotional keywords.

4️⃣ Data Splitting

80% training, 20% testing.

5️⃣ Text Preprocessing

Converted HTML → plain text

Lowercased, removed punctuation

Replaced URLs & numbers with placeholders

Applied stemming using NLTK

6️⃣ Feature Extraction

Created vocabulary from most frequent words.

Represented emails as sparse word frequency vectors.

7️⃣ Pipeline Creation

Combined preprocessing + vectorization in a Scikit-Learn Pipeline for efficiency.

8️⃣ Model Training

Algorithm: Logistic Regression

Cross-validated for stability.

9️⃣ Evaluation

Accuracy: ~98.5%

Precision: 96.88%

Recall: 97.89%

📊 Key Insights
Spam → More HTML, links, and marketing keywords.

Preprocessing pipeline significantly boosts accuracy.

Balanced precision & recall → fewer false positives & negatives.

📦 Tech Stack
Python

Scikit-Learn – ML pipelines & model building

NLTK – Text preprocessing & stemming

urlextract – URL detection

NumPy & SciPy – Sparse matrix handling

email – Email parsing

🚀 Outcome & Future Improvements
✅ High-accuracy spam detection ready for integration into email systems.
🔹 Future Enhancements:

Use TF-IDF or word embeddings for richer features.

Experiment with SVMs or neural networks.

Deploy as a real-time API service.

