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


