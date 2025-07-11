### Topics Covered

- **Introduction to causality and causal reasoning** – Hisham  
- **Machine & Deep Learning** – Clement  
- **AI & Intellectual Property** – *(TBD)*  
- **AI in Health** – Clement  
- **Frugal AI: Social & Environmental Impact** – Yogi
-  **AI Project Management & Data Challenge** – Yogi  
- **Generative AI** – Hisham  

### Introduction to causality and causal reasoning

This section covers foundations of causal graphs, probabilistic models, and causal discovery.  While correlation identifies associations between variables, causal inference seeks to answer what happens if we intervene? This shift from observation to intervention is critical in fields like medicine, economics, and artificial intelligence.

#### 🔍 Key Concepts Covered
##### 1. Causality vs. Correlation
- Describes the limitations of associational statistics.
- Demonstrates how correlation does not imply causation using simple examples.

##### 2. Counterfactual Reasoning
- Introduces the concept of counterfactuals, i.e., reasoning about "what would have happened if…"
- Provides formal notation for counterfactual queries and their use in causal reasoning.

##### 3. Structural Causal Models (SCMs)
- Formal framework proposed by Judea Pearl.
- Defines variables and relationships via directed acyclic graphs (DAGs).
- Encodes assumptions explicitly to model interventions and counterfactuals.

##### 4. Do-Calculus and Interventions
- Introduces the do-operator $do(X = x)$ to model interventions.
- Explains how to compute post-intervention distributions.


##### 5. Identifiability and Estimation
- Discusses when a causal quantity is identifiable from observational data.
- Introduces conditions like back-door and front-door criteria.

------ 

### Machine & Deep Learning Course Overview

During this course, which consisted of 8 sessions of 3 hours each, we covered a wide range of technical topics related to AI and machine learning. Below is a summary of the key concepts and techniques we explored:

#### 📚​ Introduction to AI and Neural Networks

- We began with an introduction to the history of AI, highlighting significant milestones such as the coining of the term "AI" in 1956 and the creation of the first chatbot, Elisa, in 1966.
- Our discussions on neural networks included their components such as databases for training, validation, and testing, neuron structures, cost/loss functions, metrics, and learning algorithms like gradient descent.

#### 🧠​ Types of Neural Networks

- **Convolutional Neural Networks (CNNs)**: We examined how CNNs process raw data using filters and pooling to automatically extract features, and the role of layers like batch normalization and dropout.
- **Recursive Neural Networks (RNNs)**: These were discussed in the context of handling sequential and temporal data, along with their challenges like slow convergence and instability.
- **Long Short-Term Memory Networks (LSTMs)**: As an advanced form of RNNs, we focused on their architecture involving gates such as forget, input, and output gates, which help in capturing long-term dependencies.

#### 💡​ Key Concepts in Machine Learning

- We addressed common challenges in machine learning such as overfitting and underfitting, and the bias-variance trade-off. Techniques like regularization were discussed to improve model generalization.
- The conversion of text into numerical forms using tokenization, vectorization, and one-hot encoding was covered, emphasizing their importance in processing textual data.
- Embeddings were explored as a method to project words into a dimensional space, preserving semantic meanings and relationships.

#### 🛠️​ Machine Learning Techniques

- The importance of splitting data into training, validation, and test sets was emphasized for robust model evaluation.
- We covered various learning paradigms, including supervised, unsupervised, semi-supervised, self-supervised, and transfer learning.
- Evaluation metrics for models were discussed, such as accuracy, precision, recall, F1-score for classification, and MSE, RMSE, MAE for regression tasks.
- Various models were studied, including K-means Clustering for unsupervised learning, K-Nearest Neighbors (KNN) for classification, Decision Trees for both classification and regression, and Logistic Regression.

#### 👨‍💻​​ Practical Sessions 👩‍💻

In addition to theoretical learning, the course included practical sessions using Python notebooks. These hands-on sessions allowed us to implement and experiment with the concepts discussed in class. We worked on various datasets, applying machine learning techniques and neural network models to solve real-world problems. These practical exercises were crucial in reinforcing our understanding and skills in AI and machine learning. <br>
In these session we saw about 
- [VAE](Machine%20%26%20Deep%20Learning/VAE) (Variational Auto-Encoders) for simple image generation,
- [LSTM](Machine%20%26%20Deep%20Learning/LSTM) for emotion recognition in texts,
- [Machine Learning Algorithms](Machine%20%26%20Deep%20Learning/Machine_Learning) for mushrooms classification.

#### ✅ ​Conclusion

This course provided a comprehensive overview of foundational and advanced concepts in AI and machine learning. Through both theoretical and practical sessions, we gained valuable experience and insights into the field, preparing us for further exploration and application in artificial intelligence.

-------

### Frugal AI: Social & Environmental Impact

Frugal AI refers to resource-efficient, socially equitable, and environmentally sustainable approaches to AI development and deployment.

#### 🚩 Key Challenges Addressed
- High carbon footprint from large-scale AI models (e.g., LLMs)
- Social exclusion in under-resourced regions
- Misalignment between AI development and global sustainability goals

#### 📚 Related Theories and Readings
- **Donella Meadows – *Leverage Points***  
  - Frugal AI targets deep leverage points (e.g., shifting system goals and mindsets) to move beyond performance-focused AI.
- **Steve Easterbrook – *From Computational Thinking to Systems Thinking***  
  - Encourages viewing AI as part of complex socio-technical systems requiring holistic, interdisciplinary approaches.
- **Red AI vs. Green AI**  
  - *Red AI*: Prioritizes performance, scale, and accuracy—often ignoring energy and resource costs.  
  - *Green AI*: Focuses on efficiency, transparency, and sustainability—core to the Frugal AI approach.

#### 🧭 Core Principles
- ⚡ **Environmental Efficiency**
  - Model compression, pruning, and use of edge computing
  - Energy-efficient training and deployment processes

- 🌍 **Social Inclusion**
  - Design AI for low-resource environments and infrastructure
  - Utilize transfer learning, federated learning, and inclusive datasets

- 🧠 **Systems Thinking**
  - Evaluate AI through full life cycle assessment (LCA)
  - Consider unintended consequences and feedback loops

- 🎯 **Ethical & Sustainable Governance**
  - Align AI development with the UN Sustainable Development Goals (SDGs)
  - Encourage transparency, accountability, and interdisciplinary collaboration

#### 🎯 Overall Goal
> To move toward AI systems that **do more with less**, embedding sustainability, equity, and ethical responsibility as foundational—not optional—values in innovation.


### 🧩 AI Project Management & Use Case Design (Data Challenge)

As part of the challenge, we were tasked with **managing and delivering an end-to-end AI project** in under one day. The goal was to apply both theoretical and practical AI project management principles to a realistic industrial use case.

---

#### 🔄 AI Project Management Phases (Applied in Our Challenge)

1. **Business Understanding**  
   Defined the industrial need: automatic quotation of product manufacturing costs.

2. **Data Understanding**  
   Explored the provided dataset, identified gaps, and assessed quality and relevance.

3. **Data Preparation**  
   Cleaned, processed, and structured the data for modeling.

4. **Modeling**  
   Applied machine learning algorithms (Linear Regression, Random Forest) to predict prices.

5. **Evaluation**  
   Attempted to assess model performance based on accuracy and business relevance.

6. **Deployment Planning**  
   Proposed a basic integration plan into an industrial workflow.

7. **Monitoring & Maintenance (Theoretical)**  
   Considered how the model would need to evolve over time.

---

#### 🛠️ Use Case: Automatic Product Quotation System

- Designed an AI-powered tool to support **cost estimation** in a manufacturing context.
- Mapped industrial needs to data and technical requirements.
- Balanced trade-offs between **accuracy**, **interpretability**, and **feasibility**.
- Shared insights and solution architecture in a final **team presentation**.

---

#### 💡 Key Takeaways from the Data Challenge

- We had only **5 hours** to regroup and complete the challenge, which tested our ability to prioritize, collaborate, and make quick decisions.
- We completed most of the presentation—including project planning and system design—but couldn’t deliver a **functioning machine learning model** in time.
- Despite trying both **Linear Regression** and **Random Forest**, our models failed to produce reliable predictions.
- Possible reasons include:
  - Data cleaning issues
  - Bugs or missteps in our **Python implementation**
  - Misalignment between model selection and the data characteristics
- This made it clear that early alignment around **data quality and preprocessing** is critical.
- Our biggest takeaway: **if the model fails, revisit the data pipeline first**—debugging at the model stage without clean data is often wasted effort.
- Moving forward, we need to rebuild the pipeline with a stronger foundation in **data cleaning**, **model debugging**, and **performance evaluation**.

📂 These are our
[team presentation slides](AI%20Project%20Management%20%26%20Data%20Challanges/AI-Driven%20Cost%20Estimation%20for%20Injection%20Mold%20Quotation.pdf) and 
[workbook/code](AI%20Project%20Management%20%26%20Data%20Challanges/Data_Project_Team_3%20Final.ipynb) from the data challange.


### Generative AI

This section covers fundamental theories of semantic representation in Natural Language Processing (NLP)

#### 🔍 Key Concepts Covered
##### 1. Ontology of Meaning
Semantic meaning is formally defined as the invariant truth conditions shared across paraphrased expressions, exemplified by deriving "Socrates is mortal" from "All men are mortal." This conceptual framework is implemented computationally through three complementary paradigms: symbolic logic using first-order predicate calculus (e.g., $\forall x: { } human(x) \Rightarrow mortal(x) $); vector geometry that maps words to $\mathbb{R}^D$ where angular distance quantifies semantic similarity $(e.g.,~\arccos\left( \frac{\vec{v}_1 \cdot \vec{v}_2}{\lVert \vec{v}_1 \rVert \lVert \vec{v}_2 \rVert} \right))$  reveals "anteater" ($\vec{v}_1$) and "ant" ($\vec{v}_2$) are 15° apart); and neural networks that learn continuous representations $\phi: \mathcal{V} \rightarrow \mathbb{R}^D$ directly from linguistic data, prioritizing scalability over interpretability.

##### 2. Componential Semantics
Lexical meaning is decomposed into atomic primitives—binary features ($man = [+male, +adult]$) for basic terms or continuous activations across 873 Larousse concepts for richer vocabulary (e.g., "peace" activates $PEACE=0.9$, $LIBERTY=0.8$). Semantic composition is governed by algebraic operations: normalized summation $\left( v_a\mathbin{\oplus_b} = \frac{v_a + v_b}{\lVert v_a + v_b \rVert} \right) $) merges primitives, term-wise product ($v_a\mathbin{\otimes_b} = v_a \odot v_b $) extracts intersections, and weak contextualization ($\gamma(v_a, v_b) = v_a + v_b + \left( v_a \odot v_b \right) $) enriches meaning. Polysemy is resolved via vector superposition, as in $bat = 0.6\cdot v_{animal} + 0.4 \cdot v_{sports{ }tool}$.

##### 3. Distributional Semantics"You understand a word by the words around it":

- Basic Approach:

  - Each word gets a unique ID (like "apple=ID73")

  - Documents become lists of these IDs


- Advanced Approach (Word2Vec):

  - Predicts neighboring words (e.g., "juice" likely near "orange")

  - Discovers relationships: king - man + woman ≈ queen

  - Groups similar words (Sweden/Norway/Denmark cluster together)

##### Evolutionary Synthesis
The trajectory progresses from interpretable handcrafted features (1960s-2000s) to data-driven statistical embeddings (2010s), culminating in hybrid deep learning models that balance precision and scalability. This convergence establishes vectors as the universal substrate for semantic computation in modern NLP systems.

### ⚖️ AI & Intellectual Property

- **Human authorship is required** for most IP rights (copyrights, patents).
- **AI-generated content** (text, images, inventions) typically cannot be patented or copyrighted on its own.
- **Prompts** used to guide AI (e.g. in Midjourney or ChatGPT) are **not considered inventions** and don't qualify for patent protection.

#### 🎨 Notable Example
- In 2022, an AI-generated image ("**Théâtre D'opéra Spatial**") won an art competition using **Midjourney**.
- It sparked controversy over fairness, originality, and copyright—raising global debate on AI's role in creative fields.

#### 🔑 Takeaways
- Patents and copyrights currently **exclude non-human creators**.
- Legal frameworks are **not yet adapted** to fully address AI-generated works.
- Future laws may evolve to recognize **human-AI collaboration**, but the field remains a legal gray zone.

### 🧬 AI in Health

AI technologies are revolutionizing medicine through **precision-based treatments**, enabled by **big data**, **clinical insights**, and **multi-omics analysis**. This section combines theoretical concepts with hands-on Python notebooks developed as part of our AI in Health module.

---

#### 🧠 Key Concepts

- **Precision Medicine**  
  AI enables analysis of large-scale biomedical data to design **targeted, personalized treatments** based on demographic and molecular information.

- **Targeted Therapies**  
  Modern anti-cancer drugs are designed to interact with specific **molecular targets**, often proteins, identified through data-driven AI methods.

- **Disease Understanding**  
  - A disease involves cellular or tissue-level dysfunction that impairs organ performance and causes clinical symptoms.  
  - **Chronic diseases** last 3+ months and often require longitudinal data for proper analysis.

- **Global Health Impact**  
  AI helps **characterize patients at scale** and propose targeted interventions across populations.

- **The Multi-Omics Era**  
  Diseases arise from complex interactions across different biological layers—**genomics, proteomics, transcriptomics**, etc.—which AI helps interpret through integrated models.

---

#### 📚 AI for Health – Python Notebooks

1. **🧾 Tabular Data: Risk Classification**  
   [`AI4Health_01_Tabular_Classification.ipynb`](AI%20For%20Health/AI4Health_01_Tabular_Classification.ipynb)  
   - Applies AI to structured patient data for **disease risk prediction**.
   - Demonstrates classification pipelines with demographic and clinical features.

2. **📄 Clinical Text Classification**  
   [`AI4Health_02_Clinical_Text_Classification.ipynb`](AI%20For%20Health/AI4Health_02_Clinical_Text_Classification.ipynb)  
   - Processes real-world **clinical notes** using NLP techniques.
   - Builds models to **classify health conditions** from unstructured text data.

3. **🧬 Multi-Omics Precision Modeling**  
   [`AI4Health_03_Omics_Precision_Medicine.ipynb`](AI%20For%20Health/AI4Health_03_Omics_Precision_Medicine.ipynb)  
   - Integrates genomic and molecular-level data.
   - Demonstrates how AI can support **precision medicine** by linking genetic profiles to treatment outcomes.

4. **🧫 Histology Image Classification**  
   [`AI4Health_04_Histology_Image_Classification.ipynb`](AI%20For%20Health/AI4Health_04_Histology_Image_Classification.ipynb)  
   - Uses computer vision to analyze **microscopic tissue images**.
   - Helps automate disease diagnosis and improve early detection.

---

#### 🔑 Summary

These notebooks demonstrate how AI can be applied across multiple healthcare data types—structured tables, clinical text, omics, and images—to support precision medicine and improve patient care.

> 💡 Together, they reflect how AI is **not just a tool**, but a transformative force for global health and next-generation medical practices.
