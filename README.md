# Papers on Explainable Machine Learning

> This repository includes a collection of awesome research papers on Explainable ML. It is particularly helpful for researchers to get started in this emerging field. Please raise an [issue](https://github.com/BirkhoffG/Explainable-ML-Papers/issues) if you have any comments or suggestions.

> Papers marked in **bold** are recommended by myself.

## Table of Content
- [Papers on Explainable Machine Learning](#papers-on-explainable-machine-learning)
  - [Table of Content](#table-of-content)
  - [1. General Idea](#1-general-idea)
    - [Survey](#survey)
    - [Understanding Interpretability](#understanding-interpretability)
  - [2. Interpretable Models](#2-interpretable-models)
    - [Generalized Addictive Model](#generalized-addictive-model)
    - [Rule-based Method](#rule-based-method)
    - [Mimic Learning](#mimic-learning)
  - [3. Understanding Black Box Models](#3-understanding-black-box-models)
    - [Counterfactual Explanation](#counterfactual-explanation)
    - [Example-based Explanation](#example-based-explanation)
    - [Feature-based Explanation](#feature-based-explanation)
    - [Self-Explaining Neural Network](#self-explaining-neural-network)
  - [4. Explainable ML for Human](#4-explainable-ml-for-human)
    - [Interactive ML](#interactive-ml)
  - [5. Evaluate Interpretability](#5-evaluate-interpretability)
    - [Robust Explanation](#robust-explanation)
  - [6. Others](#6-others)
    - [Medical Application](#medical-application)
  - [Useful Resources](#useful-resources)
    - [Courses & Talks](#courses--talks)
    - [Toolbox](#toolbox)

## 1. General Idea

### Survey

- A Survey Of Methods For Explaining Black Box Models. *Guidotti et. al., 2018* [pdf](https://arxiv.org/pdf/1802.01933.pdf)

- Techniques for Interpretable Machine Learning. *Du et al. 2018* [pdf](https://arxiv.org/pdf/1808.00033.pdf)
  <details><summary>notes</summary>

  - interpretable models (adding interpretable constraints, mimic learning) 
  - post-hoc global explanation, and post-hoc local explanation
  </details>

- Personalized explanation in machine learning: A conceptualization. *Schneider & Handali, 2019* [pdf](https://arxiv.org/ftp/arxiv/papers/1901/1901.00770.pdf)

- Explanation in artificial intelligence: Insights from the social sciences. *Miller, 2019* [pdf](https://www.sciencedirect.com/science/article/pii/S0004370218305988)

- **Explaining Explanations: An Overview of Interpretability of Machine Learning. *Gilpin et al. 2019*** [pdf](https://arxiv.org/pdf/1806.00069.pdf)
  <details><summary>notes</summary>

  - *tradeoff* between **Interpretability** and **completeness**: 
    - **Interpretability**: describe the internals of a system in a way that is *understandable* to human.
    - **completeness**: describe the operation of a systm in an accurate way.  
  </details>

- **Interpretable machine learning: definitions, methods, and applications. *Murdoch et al. 2019*** [pdf](https://arxiv.org/pdf/1901.04592v1.pdf) 

- Opportunities and Challenges in Explainable Artificial Intelligence (XAI): A Survey. *Das & Rad, 2020* [pdf](https://arxiv.org/pdf/2006.11371.pdf)

### Understanding Interpretability

- The Mythos of Model Interpretability. *Lipton, 2016* [pdf](https://arxiv.org/abs/1606.03490)

- Towards A Rigorous Science of Interpretable Machine Learning. *Doshi-Velez & Kim. 2017* [pdf](https://arxiv.org/pdf/1702.08608.pdf)

- Explaining Explanations in AI. *Mittelstadt et. al., 2018* [pdf](https://arxiv.org/pdf/1811.01439.pdf)

## 2. Interpretable Models

- To Explain or to Predict?. *Galit Shmueli, 2010* [pdf](https://www.stat.berkeley.edu/~aldous/157/Papers/shmueli.pdf)

- **Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead.** *Rudin, 2019* [pdf](https://www.nature.com/articles/s42256-019-0048-x.pdf)

### Generalized Addictive Model

- Accurate intelligible models with pairwise interactions. *Lou et. al., 2013* [pdf](http://www.cs.cornell.edu/~yinlou/papers/lou-kdd13.pdf)

- Intelligible Models for HealthCare: Predicting Pneumonia Risk and Hospital 30-day Readmission. *Caruana et. al., 2015* [pdf](https://dl.acm.org/doi/pdf/10.1145/2783258.2788613) | [InterpretableML](https://github.com/interpretml/interpret)

- Neural Additive Models: Interpretable Machine Learning with Neural Nets. *Agarwal et. al., 2020* [pdf](http://arxiv.org/pdf/2004.13912.pdf)

- How Interpretable and Trustworthy are GAMs? *Chang et. al., 2020* [pdf](http://arxiv.org/pdf/2006.06466.pdf)

### Rule-based Method
- Interpretable classifiers using rules and Bayesian analysis: Building a better stroke prediction model. *Letham et. al., 2015* [pdf](https://arxiv.org/pdf/1511.01644.pdf)

- Interpretable Decision Sets: A Joint Framework for Description and Prediction. *Lakkaraju et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2939672.2939874)

- Optimized Scoring Systems: Toward Trust in Machine Learning for Healthcare and Criminal Justice. *Rudin, 2018* [pdf](https://pubsonline.informs.org/doi/pdf/10.1287/inte.2018.0957)


### Mimic Learning
> Use interpretable models to approximate blackbox learning;  similar to the imitation learning in RL.

- Distilling Knowledge from Deep Networks with Applications to Healthcare Domain. *Che el. al. 2015* [pdf](https://arxiv.org/pdf/1512.03542.pdf) 

- GENESIM: genetic extraction of a single, interpretable model. *Vandewiele et. al. 2016* [pdf](https://arxiv.org/pdf/1611.05722.pdf)

- Distill-and-Compare: Auditing Black-Box Models Using Transparent Model Distillation. *Tan et. al., 2018* [pdf](https://arxiv.org/pdf/1710.06169.pdf)

- Faithful and Customizable Explanations of Black Box Models. *Lakkaraju et. al. 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3306618.3314229)


## 3. Understanding Black Box Models

> Post hoc interpretability
>

- Open the Black BoxData-Driven Explanation of Black Box Decision Systems. *Pedreschi et al.* [pdf](https://arxiv.org/pdf/1806.09936.pdf) 

- Explaining Deep Neural Networks. *Camburu, 2020* [pdf](https://arxiv.org/pdf/2010.01496.pdf)

- Generative causal explanations of black-box classifiers. *O'Shaughnessy et. al., 2020* [pdf](https://arxiv.org/pdf/2006.13913.pdf)

- **Abduction-Based Explanations for Machine Learning Models. *Ignatiev et. al. 2019*** [AAAI](https://aaai.org/ojs/index.php/AAAI/article/view/3964)

### Counterfactual Explanation

- **Counterfactual Explanations Without Opening the Black Box: Automated Decisions and the GDPR. *Wachter et. al., 2017*** [pdf](https://arxiv.org/ftp/arxiv/papers/1711/1711.00399.pdf)

- Counterfactual Visual Explanations. *Goyal et. al., 2019* [pdf](https://arxiv.org/pdf/1904.07451.pdf) 

- The Hidden Assumptions Behind Counterfactual Explanations and Principal Reasons. *Barocas et. al, 2019* [pdf](https://arxiv.org/pdf/1912.04930.pdf)

- **Explaining Machine Learning Classifiers through Diverse Counterfactual Explanations**. *Mothilal et al., 2019* [pdf](https://arxiv.org/pdf/1905.07697.pdf)

- Generative Counterfactual Introspection for Explainable Deep Learning. *Liu et. al., 2019* [pdf](https://arxiv.org/pdf/1907.03077.pdf)

- Counterfactual Explanation Algorithms for Behavioral and Textual Data. *Ramon et al., 2019* [pdf](http://arxiv.org/pdf/1912.01819.pdf)

- Preserving Causal Constraints in Counterfactual Explanations for Machine Learning Classifiers. *Mahajan et al., 2020* [pdf](http://arxiv.org/pdf/1912.03277.pdf)

- Multi-Objective Counterfactual Explanations. *DandlEmail et al., 2020* [link](https://link.springer.com/chapter/10.1007/978-3-030-58112-1_31)

### Example-based Explanation

- Examples are not enough, learn to criticize! Criticism for Interpretability. *Kim et. al., 2016* [pdf](https://beenkim.github.io/papers/KIM2016NIPS_MMD.pdf)

- Interpretability Beyond Feature Attribution:  Quantitative Testing with Concept Activation Vectors (TCAV), *Kim et. al. 2018* [pdf](http://proceedings.mlr.press/v80/kim18d/kim18d.pdf)


### Feature-based Explanation

- Permutation importance: a corrected feature importance measure. *Altmann et. al. 2010* [link](https://academic.oup.com/bioinformatics/article/26/10/1340/193348) | [sklearn](https://scikit-learn.org/stable/modules/permutation_importance.html)

- **"Why Should I Trust You?" Explaining the Predictions of Any Classifier. *Ribeiro et. al., 2016*** [pdf](http://sameersingh.org/files/papers/lime-kdd16.pdf) | [LIME](https://github.com/marcotcr/lime)

- A Unified Approach to Interpreting Model Predictions. Lundberg & Lee, 2017 [pdf](http://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf) | [SHAP](https://github.com/slundberg/shap)

- Anchors: High-Precision Model-Agnostic Explanations. *Ribeiro et. al. 2018* [pdf](https://homes.cs.washington.edu/~marcotcr/aaai18.pdf)

### Self-Explaining Neural Network
> Also offers example-based explanation

- Deep Learning for Case-Based Reasoning through Prototypes: A Neural Network that Explains Its Predictions. *Li et. al., 2017* [pdf](https://arxiv.org/pdf/1710.04806.pdf) 

- This Looks Like That: Deep Learning for Interpretable Image Recognition. *Chen et al., 2019* [pdf](http://arxiv.org/abs/1806.10574)

- Towards Robust Interpretability with Self-Explaining Neural Networks. *Alvarez-Melis et. al., 2018* [pdf](http://papers.nips.cc/paper/8003-towards-robust-interpretability-with-self-explaining-neural-networks.pdf) 
  <details><summary>Other versions</summary>

  - Self-Explaining Neural Networks. *Alvarez-Melis et. al.,* [pdf](http://people.csail.mit.edu/davidam/docs/SENN.pdf)
  - Self-Explaining Neural Networks: A Review. *Elbaghdadi, et. al., 2020* [blog](https://omarelb.github.io/self-explaining-neural-networks/) | [report](https://amanhussain.com/files/Self_Explaining_Neural_Networks_A_review_with_Extensions.pdf)
  </details>

- Learning to Explain With Complemental Examples. *Kanehira & Harada, 2019* [pdf](https://openaccess.thecvf.com/content_CVPR_2019/papers/Kanehira_Learning_to_Explain_With_Complemental_Examples_CVPR_2019_paper.pdf)

- Self-explaining AI as an Alternative to Interpretable AI. *Elton, 2020* [preprint](https://www.researchgate.net/publication/339228221_Self-explaining_AI_as_an_alternative_to_interpretable_AI)

## 4. Explainable ML for Human

> XAI for HCI

- Trends and Trajectories for Explainable, Accountable and Intelligible Systems: An HCI Research Agenda. *Abdul et. al., 2018* [pdf](https://www.cs.ubc.ca/~conati/522/532b-2019/papers/LinExplanationSurveyCHI2018Survey.pdf)

- How do Humans Understand Explanations from Machine Learning Systems? An Evaluation of the Human-Interpretability of Explanation. *Narayanan et. al., 2018* [pdf](https://arxiv.org/pdf/1802.00682.pdf)

- Interpreting Interpretability: Understanding Data Scientists' Use of Interpretability Tools for Machine Learning. *Kaur et. al., 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3313831.3376219)

- Explaining models: an empirical study of how explanations impact fairness judgment. *Dodge et. al., 2019* [pdf](https://arxiv.org/pdf/1901.07694.pdf)

- Human-Centered Tools for Coping with Imperfect Algorithms During Medical Decision-Making. *Cai et. al, 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300234)

- **Designing Theory-Driven User-Centric Explainable AI. *Wang et. al., 2019*** [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300831)

- Can we do better explanations? A proposal of User-Centered Explainable AI. *Ribera & Lapedriza, 2019* [pdf](http://ceur-ws.org/Vol-2327/IUI19WS-ExSS2019-12.pdf)

- Designing Alternative Representations of Confusion Matrices to Support Non-Expert Public Understanding of Algorithm Performance. Shen et. al., 2020 [pdf](https://www.andrew.cmu.edu/user//hongs/files/CM_CSCW2020.pdf)


### Interactive ML

- Interacting with Predictions: Visual Inspection of Black-box Machine Learning Models. *Krause et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2858036.2858529)

## 5. Evaluate Interpretability

- Quantifying Interpretability and Trust in Machine Learning Systems. *Schmidt & Biessmann, 2019* [pdf](https://arxiv.org/ftp/arxiv/papers/1901/1901.08558.pdf)

- The Price of Interpretability. *Bertsimas et. al., 2019* [pdf](http://www.mit.edu/~jaillet/general/1907.03419.pdf)

- Human Evaluation of Models Built for Interpretability.  *Lage et. al., 2019* [pdf](https://aaai.org/ojs/index.php/HCOMP/article/view/5280/5132)

- Beyond Accuracy: Behavioral Testing of NLP Models with Checklist. *Ribeiro et. al., 2020* [pdf](https://arxiv.org/pdf/2005.04118.pdf) @ ACL 2020 Best Paper


### Robust Explanation

- Interpretation of Neural Networks Is Fragile. *Ghorbani et. al., 2019* [pdf](https://www.aaai.org/ojs/index.php/AAAI/article/view/4252)

- Fooling LIME and SHAP: Adversarial Attacks on Post hoc Explanation Methods. *Slack et. al., 2020* [pdf](https://arxiv.org/pdf/1911.02508.pdf)

- Robust and Stable Black Box Explanations. *Lakkaraju et. al., 2020* [pdf](https://proceedings.icml.cc/static/paper_files/icml/2020/5945-Paper.pdf)

## 6. Others

### Medical Application

- AdaCare: Explainable Clinical Health Status Representation Learning via Scale-Adaptive Feature Extraction and Recalibration. Ma et. al., 2020 [pdf](https://www.aaai.org/ojs/index.php/AAAI/article/download/5427/5283)

- RetainVis: Visual Analytics with Interpretable and Interactive Recurrent Neural Networks on Electronic Medical Records. Kwon et. al., 2018 [pdf](https://ieeexplore.ieee.org/iel7/2945/4359476/08440842.pdf)



## Useful Resources

### Courses & Talks

- Interpretability and Explainability in Machine Learning, Fall 2019 *@ Harvard University by Hima Lakkaraju* [Course](https://interpretable-ml-class.github.io/)
- Human-centered Machine Learning *@University of Colorado Boulder by Chenhao Tan* [course](https://github.com/BoulderDS/human-centered-machine-learning)
- Model Explainability Forum *by TWIML AI Podcast* [YouTube](https://www.youtube.com/watch?v=B2QBnVnbt7A) | [link](https://twimlai.com/2020-model-explainability-forum/)
- XAI-Papers [GitHub](https://github.com/anguyen8/XAI-papers)

### Toolbox

- InterpretML [GitHub](https://github.com/interpretml/interpret)

