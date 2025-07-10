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

### 🧩 AI Project Management & Use Case Design

#### 🔄 AI Project Management Phases

1. **Business Understanding**
   - Define the problem, success metrics, and expected impact
   - Align AI goals with business or industrial needs

2. **Data Understanding**
   - Identify available data sources
   - Assess data quality, relevance, and compliance (e.g., GDPR)

3. **Data Preparation**
   - Clean, transform, and structure data
   - Address bias, missing values, and standardization

4. **Modeling**
   - Select and train AI/ML models
   - Optimize for accuracy, efficiency, and interpretability

5. **Evaluation**
   - Test model on unseen data
   - Assess performance against KPIs and business expectations

6. **Deployment**
   - Integrate AI into existing systems and workflows
   - Ensure scalability, monitoring, and user acceptance

7. **Monitoring & Maintenance**
   - Continuously assess model performance
   - Update model or retrain as needed

---

#### 🛠️ Use Case: Automatic Product Quotation System

- **Goal**: Design an AI-powered decision support tool to estimate production costs
- **Process**:
  - Map industrial needs → identify data needs → define technical solutions
  - Address challenges of performance, explainability, and user integration

- **Performance Evaluation**:
  - Assess accuracy, usability, and business value
  - Include interpretability tools (e.g., feature importance, decision trees)
  - Ensure sustainable and ethical deployment

---

#### 💡 Key Takeaways
- AI project success requires both technical and organizational alignment
- Data quality and governance are foundational
- Collaboration between domain experts and data scientists is critical
- Sustainable AI systems must be explainable, efficient, and impactful

