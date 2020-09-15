# Papers on Explainable Machine Learning

> Motivated from this [GitHub repository](https://github.com/anguyen8/XAI-papers) with different focus. Papers marked in **bold** are recommended by myself.

## Table of Content
- [Papers on Explainable Machine Learning](#papers-on-explainable-machine-learning)
  - [Table of Content](#table-of-content)
  - [1. General Idea](#1-general-idea)
    - [Survey](#survey)
    - [Understanding Interpretability](#understanding-interpretability)
  - [2. Interpretable Models](#2-interpretable-models)
    - [Mimic Learning](#mimic-learning)
  - [3. Understanding Black Box Models](#3-understanding-black-box-models)
    - [Feature Importance](#feature-importance)
  - [4. Explainable ML for Human](#4-explainable-ml-for-human)
    - [Interactive ML](#interactive-ml)
  - [5. Evaluate Interpretability](#5-evaluate-interpretability)
  - [6. Others](#6-others)
    - [Medical Application](#medical-application)
  - [Useful Resources](#useful-resources)
    - [Courses](#courses)
    - [Toolbox](#toolbox)
  - [Research Groups](#research-groups)

## 1. General Idea

### Survey
- Techniques for Interpretable Machine Learning. *Du et al. 2018* [pdf](https://arxiv.org/pdf/1808.00033.pdf)
  <details><summary>notes</summary>

  - interpretable models (adding interpretable constraints, mimic learning) 
  - post-hoc global explanation, and post-hoc local explanation
  </details>

- **Explaining Explanations: An Overview of Interpretability of Machine Learning. *Gilpin et al. 2019*** [pdf](https://arxiv.org/pdf/1806.00069.pdf)
  <details><summary>notes</summary>

  - *tradeoff* between **Interpretability** and **completeness**: 
    - **Interpretability**: describe the internals of a system in a way that is *understandable* to human.
    - **completeness**: describe the operation of a systm in an accurate way.  
  </details>

- **Interpretable machine learning: definitions, methods, and applications. *Murdoch et al. 2019*** [pdf](https://arxiv.org/pdf/1901.04592v1.pdf) 

### Understanding Interpretability

- The Mythos of Model Interpretability. *Lipton, 2016* [pdf](https://arxiv.org/abs/1606.03490)

- Towards A Rigorous Science of Interpretable Machine Learning. *Doshi-Velez & Kim. 2017* [pdf](https://arxiv.org/pdf/1702.08608.pdf)

## 2. Interpretable Models

- Intelligible Models for HealthCare: Predicting Pneumonia Risk and Hospital 30-day Readmission. *Caruana et. al., 2015* [pdf](https://dl.acm.org/doi/pdf/10.1145/2783258.2788613) | [InterpretableML](https://github.com/interpretml/interpret)
  <details><summary>notes</summary>

  - GAM-based
  </details>
- Interpretable Decision Sets: A Joint Framework for Description and Prediction. *Lakkaraju et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2939672.2939874)
  <details><summary>notes</summary>

  - Rule based
  </details>

### Mimic Learning
> Use interpretable models to approximate blackbox learning;  similar to the imitation learning in RL.

- Distilling Knowledge from Deep Networks with Applications to Healthcare Domain. *Che el. al. 2015* [pdf](https://arxiv.org/pdf/1512.03542.pdf) 
- GENESIM: genetic extraction of a single, interpretable model. *Vandewiele et. al. 2016* [pdf](https://arxiv.org/pdf/1611.05722.pdf)

## 3. Understanding Black Box Models

> Post hoc interpretability
>

- "Why Should I Trust You?" Explaining the Predictions of Any Classifier. *Ribeiro et. al., 2016* [pdf](http://sameersingh.org/files/papers/lime-kdd16.pdf) | [LIME](https://github.com/marcotcr/lime)

- A Unified Approach to Interpreting Model Predictions. Lundberg & Lee, 2017 [pdf](http://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf) | [SHAP](https://github.com/slundberg/shap)

- Interpretability Beyond Feature Attribution:  Quantitative Testing with Concept Activation Vectors (TCAV), *Kim et. al. 2018* [pdf](http://proceedings.mlr.press/v80/kim18d/kim18d.pdf)

- Faithful and Customizable Explanations of Black Box Models. *Lakkaraju et. al. 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3306618.3314229)

### Feature Importance

- Permutation importance: a corrected feature importance measure. *Altmann et. al. 2010* [link](https://academic.oup.com/bioinformatics/article/26/10/1340/193348) | [sklearn](https://scikit-learn.org/stable/modules/permutation_importance.html)



## 4. Explainable ML for Human

> XAI for HCI

- Trends and Trajectories for Explainable, Accountable and Intelligible Systems: An HCI Research Agenda. *Abdul et. al., 2018* [pdf](https://www.cs.ubc.ca/~conati/522/532b-2019/papers/LinExplanationSurveyCHI2018Survey.pdf)

- Interpreting Interpretability: Understanding Data Scientists' Use of Interpretability Tools for Machine Learning. *Kaur et. al., 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3313831.3376219)

- Explaining models: an empirical study of how explanations impact fairness judgment. *Dodge et. al., 2019* [pdf](https://arxiv.org/pdf/1901.07694.pdf)

- Human-Centered Tools for Coping with Imperfect Algorithms During Medical Decision-Making. *Cai et. al, 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300234)

- **Designing Theory-Driven User-Centric Explainable AI. *Wang et. al., 2019*** [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300831)

- Designing Alternative Representations of Confusion Matrices to Support Non-Expert Public Understanding of Algorithm Performance. Shen et. al., 2020 [pdf](https://www.andrew.cmu.edu/user//hongs/files/CM_CSCW2020.pdf)


### Interactive ML

- Interacting with Predictions: Visual Inspection of Black-box Machine Learning Models. *Krause et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2858036.2858529)

## 5. Evaluate Interpretability

- Human Evaluation of Models Built for Interpretability.  *Lage et. al., 2019* [pdf](https://aaai.org/ojs/index.php/HCOMP/article/view/5280/5132)

- Beyond Accuracy: Behavioral Testing of NLP Models with Checklist. *Ribeiro et. al., 2020* [pdf](https://arxiv.org/pdf/2005.04118.pdf) @ ACL 2020 Best Paper


## 6. Others

### Medical Application

- AdaCare: Explainable Clinical Health Status Representation Learning via Scale-Adaptive Feature Extraction and Recalibration. Ma et. al., 2020 [pdf](https://www.aaai.org/ojs/index.php/AAAI/article/download/5427/5283)

- RetainVis: Visual Analytics with Interpretable and Interactive Recurrent Neural Networks on Electronic Medical Records. Kwon et. al., 2018 [pdf](https://ieeexplore.ieee.org/iel7/2945/4359476/08440842.pdf)



## Useful Resources

### Courses

- [Interpretability and Explainability in Machine Learning, Fall 2019](https://interpretable-ml-class.github.io/) @ Harvard University (Hima Lakkaraju)

### Toolbox

- InterpretML [GitHub](https://github.com/interpretml/interpret)


## Research Groups

- [Laboratory of Explainable Artificial Intelligence for Medicine and Science (AIMS)](https://suinlee.cs.washington.edu) @ UW