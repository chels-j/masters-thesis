#  Graduation Thesis: M.Sc. Data Science, Tilburg University

![PosterLayout_JPEG](https://github.com/user-attachments/assets/57335fec-9a21-4957-b7b2-9b18b2323f58)

Here you can read my graduation thesis for the M.Sc. Data Science & Society program at Tilburg University, which I completed between February 2025 - January 2026. 

For my thesis, I built a <b> semi-supervised machine learning pipeline to classify manufacturing error messages by root cause category </b> for a pharmaceutical manufacturing company, Amgen Breda.<br>
Error messages are free-text messages written by operators to describe the reason for stoppage of a normal production process. They are important for root cause analysis and regulatory compliance.<br>
Because they are free-text descriptions, there is considerable variation in how they are written by operators, including differences in length, punctuation, grammar, syntax and quality of the information provided.<br>
Additionally, thousands of error messages are produced everyday. This makes manual categorization time-consuming and error prone.<br>
Therefore, machine learning classification was proposed as a method to more efficiently and accurately categorize error messages by their cause category.<br>
This classification can then feed in to improving downstream tools, such as ETL processes, analytics dashboards, as well as RAG and generative AI systems.<br>

<b>My thesis involved the following steps:</b>
- Collect feedback from stakeholders in the quality and manufacturing departments regarding previous efforts to classify error messages into categories and lessons learned.
- Process over 10,0000 error messages in preparation for algorithms.
- Have colleagues label a small subset of messages using a pre-defined set of categories.
- Use a clustering algorithm to broadcast/propagate labels to similar unlabeled messages based on semantic similarity.
- Train machine learning classifiers using the now expanded labeled dataset in order to be able to classify new error messages.

<b> Results: </b>
- Maximum accuracy (macro F1 score) of 60% was achieved using BERTopic-based HDBSCAN clustering and Random Forest classifier.
- The model performed better on smaller categories than larger ones.
- The Receiver Operating Curved indicated that the model does exceptionally well at ranking the probability of different classes for each message, althought overall accuracy remained low.
  
<b> Conclusions: </b>
- The model struggles to discern messages in the larger categories due to a high amount of textual variation in these categories.
- Further anlaysis revealed that different colleagues often label the same error message with different categories.
- This indicates that standardizing how error messages are written and how initial labels are applied by colleagues is needed in order to improve model accuracy.


