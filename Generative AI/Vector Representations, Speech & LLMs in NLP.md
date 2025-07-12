
## 1. Foundational Concepts: The Ontology of Meaning

The concept starts with the perennial question of meaning representation, tracing its lineage to Aristotelian syllogisms (e.g., *"Socrates is mortal"* derived from *"All men are mortal"*). Here, meaning is formally defined as the equivalence class of paraphrases—a set-theoretic construct where a sentence $s$ and its paraphrase $p$ satisfy $s \sim p$ if they share identical truth conditions across all possible worlds. This philosophical grounding transitions into computational formalisms, where meaning is operationalized through three complementary paradigms:

**Logical Forms** employ first-order predicate calculus to represent semantic relations. For instance, the syllogism is encoded as:

$$\forall x : \text{man}(x) \Rightarrow \text{mortal}(x), \quad \text{man}(\text{Socrates}) \Rightarrow \text{mortal}(\text{Socrates})$$

While precise, this approach falters under linguistic ambiguity and scalability constraints.

**Vector Spaces** map linguistic units to points in $\mathbb{R}^d$, where semantic proximity is quantified via metric geometry. The angular distance

$$\mathcal{D}_A(\vec{v}_A, \vec{v}_B) = \arccos\left( \frac{\vec{v}_A \cdot \vec{v}_B}{\|\vec{v}_A\| \|\vec{v}_B\|} \right)$$

becomes a fundamental measure, with empirical data showing:

$$\mathcal{D}_A(\text{‘anteater’}, \text{‘ant’}) \approx 15^\circ, \quad \mathcal{D}_A(\text{‘anteater’}, \text{‘train’}) \approx 68^\circ$$

This geometric interpretation naturally extends to higher dimensions, where clusters in $\mathbb{R}^2$ (e.g., animal/plant/artifact groups) visually corroborate semantic neighborhoods.

**Neural Networks** learn continuous representations $\phi : V \to \mathbb{R}^d$ from data, implicitly capturing distributional properties. This paradigm shift—from symbolic to geometric—enables scalable semantic modeling but introduces opacity in interpretability.

## 2. Componential Semantics: Decompositional Vector Spaces

Componential semantics formalizes lexical meaning through atomic primitives (semes), drawing from Wierzbicka's semantic primes and Greimas' structuralist theory. Each word $w$ is represented as a feature vector $\vec{v}_w \in \mathbb{R}^m$, where dimensions correspond to primitives like ±male or ±mature. The binary feature system exemplifies this:

$$\vec{v}_{\text{man}} = [1, 1], \quad \vec{v}_{\text{boy}} = [1, 0], \quad \vec{v}_{\text{child}} = [\alpha, 0], \quad (\alpha \in \{0,1\})$

**Chauché's Thematic Vectors** extend this to continuous space, using 873 concepts from the Larousse thesaurus as dimensions. Here, $\vec{v}_w$ encodes concept activations (e.g., *peace* activates PEACE at magnitude 0.9 and LIBERTY at 0.8), with non-negativity constraints preserving interpretability.

Vector operations define compositional semantics:

-   **Normalized Sum**: $$\vec{v}_{A \oplus B} = \frac{\vec{v}_A + \vec{v}_B}{\|\vec{v}_A + \vec{v}_B\|}$$

-   **Term-wise Product**: $$\vec{v}_{A \otimes B} = \vec{v}_A \odot \vec{v}_B$$

-   **Weak Contextualization**: $$\gamma(\vec{v}_A, \vec{v}_B) = \vec{v}_A + \vec{v}_B + (\vec{v}_A \odot \vec{v}_B)$$

Polysemy is resolved via superposition: for *frégate* (warship/bird), 

$$\vec{v}_{frégate} = \lambda_1 \vec{v}_{weapon} + \lambda_2 \vec{v}_{maritime} + \lambda_3 \vec{v}_{bird}$$

Database construction leverages kernel methods—manually indexing 1,000–2,000 seed terms, then automating expansion through synonymy graphs and corpus statistics—resulting in 276,000 acceptions for French with 61% polysemy.

## 3. Distributional Semantics: Contextual Geometry

Distributional semantics, rooted in Firth's axiom ("You shall know a word by the company it keeps"), posits that meaning emerges from contextual co-occurrence. Formally, the meaning of $w$ is the distribution $P(c \mid w)$ over contexts $c$, approximated empirically from corpora.

Salton's vector space model instantiates this via one-hot encodings: each word $w$ has a basis vector $\vec{e}_w \in \{0,1\}^{|V|}$, and documents are sums:

$$\vec{v}_d = \sum_{w \in d} \vec{e}_w$$

This suffers from the curse of dimensionality ($|V| \sim 10^6$) and sparsity, motivating dimensionality reduction. Latent Semantic Analysis (LSA) applies truncated SVD to the term-document matrix $X$:

$$X \approx U_k \Sigma_k V_k^\top, \quad k \ll |V|$$

projecting words into a latent space $\mathbb{R}^k$ where geometric relations encode semantic shifts.

**Word2Vec's** neural approach revolutionizes this via two architectures:

-   **Skip-gram** maximizes: $\sum_{(w_t, w_c)} \log \sigma(\vec{v}_{w_c} \cdot \vec{v}_{w_t})$

-   **CBOW** inversely predicts $w_t$ from $\{w_{t \pm c}\}$.

The resultant embeddings exhibit linear regularities (e.g., $\vec{v}_{\text{king}} - \vec{v}_{\text{man}} + \vec{v}_{\text{woman}} \approx \vec{v}_{\text{queen}}$) and neighborhood structures (e.g., $\cos(\vec{v}_{\text{Sweden}}, \vec{v}_{\text{Norway}}) \approx 0.76$). Limitations include static representations (ignoring context shifts) and brittleness for rare words.

**Celestial analogies** illustrate the geometric paradigm: angular separations between *Lune* (Moon), *Jupiter*, and *Sagittaire* in a 2D semantic map directly correspond to distributional dissimilarities, grounding abstract vector operations in physical intuition. This framework bridges symbolic linguistics with statistical learning, setting the stage for neural language models.

## Theoretical Synthesis

These sections trace an evolution from handcrafted symbolic representations (componential semantics) to data-driven geometric models (distributional semantics). The former prioritizes interpretability through discrete primitives and algebraic operations; the latter emphasizes scalability via continuous embeddings and statistical learning. Their convergence—evident in neural architectures—underpins modern NLP, where vectors serve as the universal substrate for semantic computation.
