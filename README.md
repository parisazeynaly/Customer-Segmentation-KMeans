# Customer Segmentation: A Novel Approach with NLP Integration

**Summary:** This project goes beyond traditional customer segmentation by integrating a modern Natural Language Processing (NLP) technique to discover more meaningful customer groups. It combines standard numerical features with insights from customer reviews, providing a richer and more actionable analysis.

---

## The Traditional Baseline

The project begins with a classic approach to customer segmentation using the **K-Means Clustering** algorithm on two numerical features: `Annual Income` and `Spending Score`. This baseline analysis successfully identifies five distinct segments, providing a solid foundation for comparison.

## The Novelty: Enriching Segments with NLP

This repository's key innovation lies in its use of **Topic Modeling (LDA)**. We created a new textual feature from simulated customer reviews to capture underlying sentiments and needs that are not reflected in numerical data. By doing this, we turned unstructured text into a valuable feature for our clustering model.

This process involves:

* **Feature Engineering:** Using the **LDA algorithm** to transform text reviews into numerical features (topic probabilities).
* **Data Integration:** Combining these new features with the original `Annual Income` and `Spending Score`.

---

## Results & Key Findings

By integrating NLP, the K-Means algorithm discovered new, more nuanced customer segments. The final clusters are not only defined by their financial habits but also by their underlying concerns and interests as expressed in their reviews.

![Traditional vs. Novel Clustering](images/comparison_plot.png)

* **Example:** A group previously identified as "Low Income, Low Spender" might now be split into two groups: "Low Income, Price-Conscious" and "Low Income, Quality-Focused."

---

## How to Explore

1.  **Traditional Analysis:** Start with the `notebooks/01_Traditional_KMeans_Analysis.ipynb` to see the baseline model.
2.  **Novelty:** Proceed to `notebooks/02_Novel_NLP_Integration.ipynb` to follow the full workflow, including the NLP steps and the final combined clustering.

---

## Technologies Used

* **Python**
    * `pandas` & `numpy`
    * `scikit-learn` for K-Means and LDA
    * `matplotlib` & `seaborn` for visualization

---

## Author

* **Name:** [parisa zeynaly]
