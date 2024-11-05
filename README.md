# amis-voice-classifier
Final project for BC's Documenting Indigenous Languages with Data Science course.

# Project description
This was an open-ended group project for Boston College's Documenting and Preserving Indigenous Languages with Data Science course. Our main objective was to investigate the distribution of grammatical voice across verbs in the Formosan language Amis (ISO 639-3: ami). For this project we applied the natural language processing techniques that we learned throughout the course to train a classifier that identifies words in Amis as verbs or non-verbs with 87% accuracy and to analyze the frequency of the verbs and their voices in our dataset.

Group members: Talia Potter, Qiuyi Lu, Maggie Berkley

# Datasets 
* [NTU Corpus of Formosan Languages](https://corpus.linguistics.ntu.edu.tw/#/)
* Amis translation of the Bible

# Tools
* **Programming language:** Python
* **Markup language:** XML
* **Platform:** Google Colab
* **Libraries:**
  * **xml and ElementTree** for creating and parsing XML files. 
  * **re** for using regular expressions to identify words with certain affixes or glosses.
  * **scikit-learn** for testing classifier models on our data. We ended up using the gradient boosting classifier.
  * **NumPy** for converting our data into feature vectors.
  * **Pandas and Matplotlib** for analyzing and visualizing the verb and voice frequencies.

# Part 1: Cleaning and Formatting Data
Bible.ipynb: This notebook contains the code for preparing the Bible data and putting it into FormosanBank XML format.

NTU.ipynb: This notebook contains the code for preparing the NTU Corpus data and putting it into FormosanBank XML format.

# Part 2: Classifying and Analyzing Verbs
Verb_Classifier.ipynb: This notebook contains most of our work for this project. It includes parsing the XML files, creating a list of verbs and lists of words in each of the voices using the NTU glosses, experimenting with different classifiers to sort words into verb and non-verb categories, and applying the classifier to the Bible data.

Verb_Analysis.ipynb: This notebook contains an analysis of the verbs and voices in the NTU and Bible data.
