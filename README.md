# fakenewsdetector
With all the misinformation floating around, I wanted to build something that could help identify fake news. This project uses text classification to analyze news articles and predict whether they're legit or not.
Tech stack:
Python
Pandas & NumPy (data handling)
Scikit-learn (ML models)
Matplotlib & Seaborn (visualizations)
Jupyter Notebook

Dataset:
Using the ISOT Fake News Dataset with ~45k articles (23k fake, 21k real) covering political and world news from 2016-2017.

## Unique Feature: Source-Agnostic Detection

Unlike typical fake news detectors that rely on source recognition, 
this model analyzes *writing patterns* and *content quality* rather 
than simply memorizing trusted sources. This makes it more robust 
for detecting misinformation from unknown sources.

**Model Performance:**
- Algorithm: Logistic Regression
- Accuracy: 99.01%
- Dataset: ISOT Fake News (45k articles)

**Key Findings:**
- Model successfully identifies sensational vs professional writing styles
- Discovered dataset bias: model over-relies on source attribution (e.g., "Reuters")
- High accuracy on test set, but potential generalization issues

**Next Steps:**
- Implement source-agnostic training
- Test on diverse news sources
- Build web interface for testing
