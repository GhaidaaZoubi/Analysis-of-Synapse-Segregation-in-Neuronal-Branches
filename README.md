# Analysis of Synapse Segregation in Neuronal Branches

**Authors:** Ghaida Zoubi & Donia Shebrawi  
**Program:** MSc Statistics – Data Science, University of Haifa  

---

##  Overview
This project investigates whether synapse placement along neuronal branches is random or follows structured organizational patterns.  
Using data from over **9 million valid branch splits across ~130,000 neurons**, we applied **classical statistics**, **null simulations**, and **machine learning** to uncover patterns of **synapse segregation**.

---

##  Research Question
> Are synapses randomly distributed at neuronal branch points, or do they show organized, neuron-specific segregation patterns?

---

##  Methods
We combined several statistical and machine learning approaches:

- **Fisher’s Exact Test** – To test individual branch splits for segregation.  
- **Binomial Test** – To assess if the proportion of significant splits exceeded random expectation (5%).  
- **False Discovery Rate (FDR)** – To correct for multiple comparisons.  
- **Null Simulations** – Random reassignment of synapse counts to confirm results weren’t due to bias.  
- **Chi-Squared Test** – To test dependence of significant splits within neurons.  
- **Depth and Superclass Analysis** – To examine structural and functional patterns.  
- **Random Forest Classifier** – To predict significant splits using neuronal features.  
- **Generalized Linear Model (GLM)** – To quantify relationships while controlling for neuron-level clustering.

---

##  Key Findings
- **~11.3%** of splits showed significant segregation — much higher than random expectation.  
- The proportion of significant splits **decreased with increasing dendritic depth**, suggesting structured organization.  
- **FDR correction** confirmed the robustness of findings (≈2.6% remained significant).  
- **Machine Learning (Random Forest)** achieved ROC-AUC ≈ **0.73**, identifying depth, synapse counts, and structural features as top predictors.  
- **GLM analysis** validated that structural and connectivity variables significantly predict segregation.

---


##  Tools and Libraries
- **Python:** pandas, numpy, scipy, scikit-learn, statsmodels, matplotlib  
- **Statistical tests:** Fisher, Binomial, Chi-squared, FDR  
- **Machine Learning:** Random Forest (200 trees, max depth 15)  
- **GLM:** Binomial family with cluster-robust SEs  

---

##  Summary Conclusion
Synapse placement across neuronal branches **is not random**.  
The distribution reflects **organized, biologically meaningful structure**, influenced by neuron morphology and functional type.

---
