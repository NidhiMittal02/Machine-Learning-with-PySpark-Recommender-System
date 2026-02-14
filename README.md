# 🛍️ E-Commerce Product Recommendation System using PySpark & Embeddings

## 📌 Project Overview

This project builds a scalable **Product Recommendation System** using:

- OpenAI text embeddings  
- PySpark for distributed processing  
- K-Means clustering  
- PCA visualization  

The system recommends similar products based on product title and description.

---

## 🎯 Objective

To recommend products to users based on:

- Recently viewed products  
- Semantic similarity using embeddings  
- Cluster-based grouping  

---

## 📥 Input

- CSV Dataset (`products_dataset.csv`)
  - `product_id`
  - `title`
  - `description`
- List of recently viewed product IDs  

---

## 📤 Output

- Clustered products  
- 2D visualization of clusters  
- Recommended products from same cluster  
- Printed product titles as recommendations  

---

## 🧠 Methodology

### Step 1: Data Loading
- Load dataset using PySpark.

### Step 2: Text Preprocessing
- Combine title and description into `combined_text`.

### Step 3: Embedding Generation
- Generate 512-dimensional embeddings using OpenAI API.
- Convert text into vector representation.

### Step 4: Feature Engineering
- Convert embedding columns into Spark feature vector.

### Step 5: Clustering
- Apply K-Means clustering (`k=5`).
- Similar products grouped together.

### Step 6: Dimensionality Reduction
- Apply PCA (512 → 2 dimensions).
- Visualize clusters.

### Step 7: Recommendation Logic
- Identify clusters of recently viewed products.
- Recommend other products from same clusters.
- Randomly select 5 products per cluster.

---

## 🛠 Technologies Used

- Python  
- PySpark  
- OpenAI Embeddings API  
- Pandas  
- NumPy  
- Plotly  
- Machine Learning (K-Means, PCA)  

---

## 📊 Machine Learning Concepts Used

- Text Embeddings  
- Feature Vectorization  
- K-Means Clustering  
- PCA  
- Semantic Similarity  

---

## 🚀 Key Features

- ✔ Distributed data processing with Spark  
- ✔ AI-powered semantic embeddings  
- ✔ Cluster-based recommendation  
- ✔ Interactive visualization  
- ✔ Scalable architecture  

---

## 📌 Conclusion

This project demonstrates how modern AI embeddings combined with distributed machine learning can build an efficient and scalable product recommendation system.

The system:

- Understands product meaning (not just keywords)  
- Groups similar products  
- Provides personalized recommendations  
- Can scale to millions of products  

It showcases the integration of **LLM embeddings + Big Data + Machine Learning** for real-world applications.
