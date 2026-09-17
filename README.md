# Unsupervised Learning and Reinforcement Learning

## Overview

This practical introduces two important areas of Machine Learning:

* **Unsupervised Learning** using K-Means Clustering
* **Reinforcement Learning** using a simple route-selection example

The practical focuses on understanding how Machine Learning concepts can be applied to real-world business problems.

## Learning Objectives

By completing this practical, we learn how to:

* Understand customer segmentation using **K-Means Clustering**
* Group similar customers based on their behaviour
* Interpret customer clusters from a business perspective
* Understand the basic concept of **Reinforcement Learning**
* Identify an **Agent, Action, Environment, and Reward**
* Understand **Exploration vs. Exploitation**

---

## Part A: Customer Segmentation Using K-Means

### Business Problem

An online retailer wants to identify different types of customers using two features:

* Monthly Spending
* App Visits

K-Means Clustering is used to divide the customers into **3 groups (K = 3)**.

### Dataset

The dataset contains 8 customers:

| Customer | Monthly Spending | App Visits |
| -------- | ---------------: | ---------: |
| A        |             9000 |         20 |
| B        |             8500 |         18 |
| C        |             1200 |          3 |
| D        |             1500 |          4 |
| E        |             5000 |         10 |
| F        |             5500 |         12 |
| G        |             8800 |         19 |
| H        |             1800 |          5 |

### Method

The following steps are performed:

1. Create the customer dataset using Pandas.
2. Select Monthly Spending and App Visits as clustering features.
3. Apply K-Means with `K = 3`.
4. Assign each customer to a cluster.
5. Visualize the resulting customer groups.
6. Interpret the clusters from a business perspective.

### Business Interpretation

The clusters can be interpreted based on customer behaviour rather than the cluster number itself.

Possible segments include:

* **Premium Customers** – High spending and high app engagement
* **Medium-Value Customers** – Moderate spending and app activity
* **Low-Engagement Customers** – Lower spending and fewer app visits

Possible business actions include:

* Loyalty rewards for highly engaged customers
* Personalized recommendations for medium-value customers
* Re-engagement campaigns for customers with low activity

### Customer Segmentation Graph

The practical produces a scatter plot showing customers based on their monthly spending and app visits, with different clusters represented separately.

> Add the screenshot of the customer-segmentation graph here after running the notebook.

---

## Part B: Introduction to Reinforcement Learning

### Business Scenario

A delivery company has two possible routes:

* Route A
* Route B

The company wants to identify which route generally provides better delivery performance.

Example rewards are:

```text
Route A: [5, 4, 6, 5, 4]
Route B: [8, 9, 7, 10, 8]
```

The average reward is calculated for each route.

Route B has a higher average reward in this example, demonstrating how reward feedback can influence future decisions.

### Reinforcement Learning Components

| Component   | Example                                |
| ----------- | -------------------------------------- |
| Agent       | Delivery decision system               |
| Environment | Roads and traffic                      |
| Action      | Choosing Route A or Route B            |
| Reward      | Feedback based on delivery performance |

The basic learning process can be represented as:

**Action → Reward → Learning → Future Decision**

### Exploration vs. Exploitation

**Exploration** means trying a new or less-used option to gather more information.

Example:

> Trying Route A even when Route B has previously performed better.

**Exploitation** means choosing the option that is already known to perform well.

Example:

> Choosing Route B because its historical average reward is higher.

---

## Machine Learning Concepts Covered

| Machine Learning Type  | Main Idea                      | Business Example          |
| ---------------------- | ------------------------------ | ------------------------- |
| Supervised Learning    | Learn from known answers       | Customer churn prediction |
| Unsupervised Learning  | Discover hidden patterns       | Customer segmentation     |
| Reinforcement Learning | Learn from actions and rewards | Route optimization        |

---

## Technologies Used

* **Python**
* **Pandas**
* **Scikit-learn**
* **Matplotlib**
* **Google Colab**

---

## Files

```text
part-a/
└── unsupervised-learning/
    ├── Unsupervised_and_Reinforcement_Learning_Practical_Name.ipynb
    ├── README.md
    └── customer-segmentation.png
```

---

## Key Takeaways

### Unsupervised Learning

Unsupervised Learning finds patterns or groups in data without predefined labels.

### Clustering

Clustering groups data points that have similar characteristics.

### K-Means

K-Means divides data into a specified number of clusters. In this practical, **K = 3**.

### Customer Segmentation

Customer segmentation helps businesses understand different customer behaviours and create more targeted marketing strategies.

### Reinforcement Learning

Reinforcement Learning involves an agent taking actions and learning from rewards or feedback received from the environment.

### Exploration and Exploitation

* **Exploration:** Try different options to learn more.
* **Exploitation:** Use the option currently known to perform well.

---

## How to Run

1. Open the `.ipynb` notebook in **Google Colab**.
2. Run the cells from top to bottom.
3. Observe the customer dataset and cluster assignments.
4. View the customer-segmentation graph.
5. Review the calculated route rewards.
6. Complete the reflection questions.
7. Add a screenshot of the customer-segmentation graph to the repository.

---

## Submission

The notebook should be renamed as:

```text
Unsupervised_and_Reinforcement_Learning_Practical_Name.ipynb
```

and uploaded under:

```text
part-a/unsupervised-learning/
```

The repository should also contain a screenshot of the customer-segmentation graph.
