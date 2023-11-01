## Emotion classification findings

Here are the findings derived from the implementation of the Support Vector Classifier (SVC) and LSTM models trained on Spacy word embeddings for a relatively small dataset with less than 10000 comments or utterances:

### Support Vector Classifier (SVC) Model

-  The SVC model achieves an accuracy of 69%, indicating that it correctly classifies emotions in approximately 69% of the instances.

- The highest F1-score (0.71) is achieved for the "joy" emotion, indicating that this emotion is relatively well-predicted by the model.

- The model has relatively balanced precision and recall for all three emotions, meaning that it doesn't favor one aspect (false positives or false negatives) significantly.

- The macro-average F1-score across all emotions is 0.70, suggesting a reasonable overall performance.

- The weighted average F1-score, which accounts for class imbalances, is also 0.69, indicating a decent model performance.


### LSTM Model

- The LSTM model has an accuracy of 65%, which is slightly lower than the SVC model's accuracy.

- The "joy" emotion achieves the highest F1-score (0.77) in this model, indicating it is well-predicted by the LSTM.

- The "anger" emotion has a lower recall (0.45), meaning that the model misses a significant number of actual instances of anger.

- The model has a lower precision for "fear" meaning that it incorrectly classifies some instances as "fear".

The macro-average F1-score is 0.65, indicating slightly lower overall performance compared to the SVC model.These findings suggest that while both models have similar macro-average F1-scores, they have different strengths and weaknesses in predicting specific emotions. The SVC model appears to have a more balanced performance across all emotions, while the LSTM model excels in predicting "joy" but struggles with "anger" and "fear". The choice of model may depend on which emotions are more critical in the specific context of the business objective.

---

> With more data, LSTM model has a better chance of addressing more patterns related to different emotions. This increased data can help the model learn more representations of the emotions it is trying to classify and can perform better than SVC model.

---

A pre-trained language model like BERT transformer can potentially perform very well in the scenario of emotion classification, with a relatively small dataset, but BERT models are computationally intensive, and training or fine-tuning them on a google colab can be challenging.





