### The code is this repository was used for my thesis 'Tracing the Social Construction of Abortion Attitudes in Online Discourse'

The code was written in Python 3.11.5 and in AWS PySpark.

The code requirements for the Python version of the code are located in the requirements.txt file.

---

## Repository Structure

### `Preprocessing/`
Scripts related to the initial extraction and cleaning of Reddit posts and comments:

- `post_extraction.ipynb` – Extracts Reddit posts from AWS.
- `comment_extraction.ipynb` – Extracts Reddit comments from AWS.
- `commentClean.ipynb` – Original cleaning and preprocessing of the extracted comments.

---

### `Classifiers/`
Notebooks related to classification and labeling of comments:

- `keyword_classifier.ipynb` – Applies keyword classification.
- `labeling_data.ipynb` – Demonstrates iterative labeling using the keyword classifier.
- `on_topic.ipynb` – Applies keyword classifier to determine on-topic vs. off-topic comments.
- `svm_original.ipynb` – Original application of the SVC model.
- `svc_model.ipynb` – Final version of the SVC model.
- `svc_launch_hcs.ipynb` – Launches the SVC model on 100k comments, and then using high-confidence sampling.
- `distilbert_data.ipynb` – Trains and applies the DistilBERT model for classification.

---

### `Topic_Modeling/`
Notebooks related to topic modeling of pro-life and pro-choice comments:

- `prolife_lda.ipynb` – LDA topic modeling on pro-life comments.
- `prolife_BT.ipynb` – BERTopic modeling on pro-life comments.
- `prochoice_BT.ipynb` – BERTopic modeling on pro-choice comments.
- `bt_explore.ipynb` – Further exploration of BERTopic models.
