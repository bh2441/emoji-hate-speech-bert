## Emoji-Aware Hate Speech Detection (DS-UA 301 Group Project)
This project was completed in Spring 2025 as part of the Advanced Techniques in Machine Learning and Deep Learning course at New York University. In collaboration with Daphne Ozkan and Alice Yang, I explored whether augmenting social media comment text with emoji descriptions could improve hate speech classification performance.

We began with a CNN model using GloVe embeddings, but after observing poor performance, we transitioned to a BERT-based approach. We compared a standard text-only BERT classifier to an emoji-aware version that converts emojis into text (e.g., 😂 → “face with tears of joy”).

Our dataset was a filtered version of final_hateXplain.csv, including only comments with emojis. Models were fine-tuned on bert-base-uncased and evaluated using accuracy, F1-score, precision, recall, and confusion matrices. The emoji-aware model showed a modest improvement in recall and overall accuracy, suggesting that incorporating emoji sentiment can enhance nuanced hate speech detection.
