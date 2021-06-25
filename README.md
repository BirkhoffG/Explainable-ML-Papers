# Papers on Explainable Machine Learning

This repository includes a collection of awesome research papers on **Explainable Machine Learning** (also referred as Explainable AI/XAI, Interpretable Machine Learning). As a rapidly emerging field, it can be frustrated when starting researching this field buried by enormous amount of papers (and un-unified terminologies). I hope this repository can help new ML researchers/practitioners to learn about this field with lesser pain and stress.

Unlike most repositories you find in GitHub which maintain a comprehensive list of resources in Explainable ML, I try to keep this list short to make it less intimating for beginners. It is definitely an objective selection which is based on my preferences and research tastes. 

> Papers marked in **bold** are highly recommended to read.

## 1. General Idea

### Survey

- The Mythos of Model Interpretability. *Lipton, 2016* [pdf](https://arxiv.org/abs/1606.03490)

- Open the Black Box Data-Driven Explanation of Black Box Decision Systems. *Pedreschi et al.* [pdf](https://arxiv.org/pdf/1806.09936.pdf) 

- Techniques for Interpretable Machine Learning. *Du et al. 2018* [pdf](https://arxiv.org/pdf/1808.00033.pdf)
  <details><summary>notes</summary>

  - interpretable models (adding interpretable constraints, mimic learning) 
  - post-hoc global explanation, and post-hoc local explanation
  </details>

- Explaining Explanations in AI. *Mittelstadt et. al., 2019* [pdf](https://arxiv.org/pdf/1811.01439.pdf)

- **Explanation in artificial intelligence: Insights from the social sciences. *Miller, 2019*** [pdf](https://www.sciencedirect.com/science/article/pii/S0004370218305988)

- **Explaining Explanations: An Overview of Interpretability of Machine Learning. *Gilpin et al. 2019*** [pdf](https://arxiv.org/pdf/1806.00069.pdf)
  <details><summary>notes</summary>

  - *tradeoff* between **Interpretability** and **completeness**: 
    - **Interpretability**: describe the internals of a system in a way that is *understandable* to human.
    - **completeness**: describe the operation of a systm in an accurate way.  
  </details>

- **Interpretable machine learning: definitions, methods, and applications. *Murdoch et al. 2019*** [pdf](https://arxiv.org/pdf/1901.04592v1.pdf) 
  
- Explaining Deep Neural Networks. *Camburu, 2020* [pdf](https://arxiv.org/pdf/2010.01496.pdf)


## 2. Global Explanation

### Interpretable Models

- **Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead.** *Rudin, 2019* [pdf](https://www.nature.com/articles/s42256-019-0048-x.pdf)

**Generalized Addictive Model**

- Accurate intelligible models with pairwise interactions. *Lou et. al., 2013* [pdf](http://www.cs.cornell.edu/~yinlou/papers/lou-kdd13.pdf)

- Intelligible Models for HealthCare: Predicting Pneumonia Risk and Hospital 30-day Readmission. *Caruana et. al., 2015* [pdf](https://dl.acm.org/doi/pdf/10.1145/2783258.2788613) | [InterpretableML](https://github.com/interpretml/interpret)

**Rule-based Method**

- Interpretable classifiers using rules and Bayesian analysis: Building a better stroke prediction model. *Letham et. al., 2015* [pdf](https://arxiv.org/pdf/1511.01644.pdf)

- Interpretable Decision Sets: A Joint Framework for Description and Prediction. *Lakkaraju et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2939672.2939874)

**Scoring System**

- Optimized Scoring Systems: Toward Trust in Machine Learning for Healthcare and Criminal Justice. *Rudin, 2018* [pdf](https://pubsonline.informs.org/doi/pdf/10.1287/inte.2018.0957)


### Model Distillation
> Use interpretable models to approximate blackbox learning;  similar to the imitation learning in RL.

- Distill-and-Compare: Auditing Black-Box Models Using Transparent Model Distillation. *Tan et. al., 2018* [pdf](https://arxiv.org/pdf/1710.06169.pdf)

- Faithful and Customizable Explanations of Black Box Models. *Lakkaraju et. al. 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3306618.3314229)


### Representation-based Explanation

- Interpretability Beyond Feature Attribution:  Quantitative Testing with Concept Activation Vectors (TCAV), *Kim et. al. 2018* [pdf](http://proceedings.mlr.press/v80/kim18d/kim18d.pdf)

- This Looks Like That: Deep Learning for Interpretable Image Recognition. *Chen et al., 2019* [pdf](http://arxiv.org/abs/1806.10574)
  <details><summary>Related papers</summary>

  - This Looks Like That, Because ... Explaining Prototypes for Interpretable Image Recognition. *Nauta et al., 2020* [pdf](https://arxiv.org/pdf/2011.02863.pdf)
  - Learning to Explain With Complemental Examples. *Kanehira & Harada, 2019* [pdf](https://openaccess.thecvf.com/content_CVPR_2019/papers/Kanehira_Learning_to_Explain_With_Complemental_Examples_CVPR_2019_paper.pdf)
  </details>

### Self-Explaining Neural Network
> Also offers example-based explanation


- Towards Robust Interpretability with Self-Explaining Neural Networks. *Alvarez-Melis et. al., 2018* [pdf](http://papers.nips.cc/paper/8003-towards-robust-interpretability-with-self-explaining-neural-networks.pdf) 

- Deep Weighted Averaging Classifiers. *Card et al., 2019* [pdf](http://arxiv.org/pdf/1811.02579.pdf)


## 3. Local Explanation

> Note: cumulating multiple local explanations can be viewed as constructing a global explanation.

### Feature-based Explanation

- Permutation importance: a corrected feature importance measure. *Altmann et. al. 2010* [link](https://academic.oup.com/bioinformatics/article/26/10/1340/193348) | [sklearn](https://scikit-learn.org/stable/modules/permutation_importance.html)

- **"Why Should I Trust You?" Explaining the Predictions of Any Classifier. *Ribeiro et. al., 2016*** [pdf](http://sameersingh.org/files/papers/lime-kdd16.pdf) | [LIME](https://github.com/marcotcr/lime)

- A Unified Approach to Interpreting Model Predictions. Lundberg & Lee, 2017 [pdf](http://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf) | [SHAP](https://github.com/slundberg/shap)

- Anchors: High-Precision Model-Agnostic Explanations. *Ribeiro et. al. 2018* [pdf](https://homes.cs.washington.edu/~marcotcr/aaai18.pdf)

### Example-based Explanation

- Examples are not enough, learn to criticize! Criticism for Interpretability. *Kim et. al., 2016* [pdf](https://beenkim.github.io/papers/KIM2016NIPS_MMD.pdf)

### Counterfactual Explanation

> Also referred as algorithmic recourse or contrastive explanation.

- Counterfactual Explanations for Machine Learning: A Review. *Verma et al., 2020* [pdf](https://arxiv.org/pdf/2010.10596.pdf)
- A survey of algorithmic recourse: definitions, formulations, solutions, and prospects. *Karimi et al., 2020* [pdf](http://arxiv.org/pdf/2010.04050.pdf)

**Minimize distance counterfactuals**

- Counterfactual Explanations Without Opening the Black Box: Automated Decisions and the GDPR. *Wachter et. al., 2017* [pdf](https://arxiv.org/ftp/arxiv/papers/1711/1711.00399.pdf)

- Explaining Machine Learning Classifiers through Diverse Counterfactual Explanations. *Mothilal et al., 2019* [pdf](https://arxiv.org/pdf/1905.07697.pdf)

**Minimize cost (algorithmic recourse)**

- Actionable Recourse in Linear Classification. *Ustun et al., 2019* [pdf](https://arxiv.org/pdf/1809.06514.pdf)

- Algorithmic Recourse: from Counterfactual Explanations to Interventions. *Karimi et al., 2021* [pdf](https://arxiv.org/pdf/2002.06278.pdf)

**Causal constraints**

- Preserving Causal Constraints in Counterfactual Explanations for Machine Learning Classifiers. *Mahajan et al., 2020* [pdf](http://arxiv.org/pdf/1912.03277.pdf)


## 4. Explainability in Human-in-the-loop ML

> HCI's perspective of Explainable ML

- Interacting with Predictions: Visual Inspection of Black-box Machine Learning Models. *Krause et. al., 2016* [pdf](https://dl.acm.org/doi/pdf/10.1145/2858036.2858529)
- Human-centered Machine Learning: a Machine-in-the-loop Approach. *Tan, 2018* [blog](https://medium.com/@ChenhaoTan/human-centered-machine-learning-a-machine-in-the-loop-approach-ed024db34fe7)
- Trends and Trajectories for Explainable, Accountable and Intelligible Systems: An HCI Research Agenda. *Abdul et. al., 2018* [pdf](https://www.cs.ubc.ca/~conati/522/532b-2019/papers/LinExplanationSurveyCHI2018Survey.pdf)
- Explaining models: an empirical study of how explanations impact fairness judgment. *Dodge et. al., 2019* [pdf](https://arxiv.org/pdf/1901.07694.pdf)
- Human-Centered Tools for Coping with Imperfect Algorithms During Medical Decision-Making. *Cai et. al, 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300234)
- **Designing Theory-Driven User-Centric Explainable AI. *Wang et. al., 2019*** [pdf](https://dl.acm.org/doi/pdf/10.1145/3290605.3300831)
- **Does the Whole Exceed its Parts? The Effect of AI Explanations on Complementary Team Performance.** *Bansal et al., 2021* [pdf](https://arxiv.org/pdf/2006.14779.pdf)


## 5. Evaluate Explainable ML

> Evaluation of explainable ML can be loosely categorized into two classes:
> - *faithfulness* on evaluating how well the explanation reflects the true inner behavior of the black-box model.
> - *interpretability* on evaluating how understandable the explanation to human.

- The Price of Interpretability. *Bertsimas et. al., 2019* [pdf](http://www.mit.edu/~jaillet/general/1907.03419.pdf)

- Beyond Accuracy: Behavioral Testing of NLP Models with Checklist. *Ribeiro et. al., 2020* [pdf](https://arxiv.org/pdf/2005.04118.pdf) @ ACL 2020 Best Paper

### Evaluating Faithfulness

> Evaluate whether or not the explanation faithfully reflects how model works (it turns out that 100% faithfully is often not the case in post-hoc explanations).

- Sanity Checks for Saliency Maps *Adebayo et al., 2018* [pdf](https://papers.nips.cc/paper/2018/file/294a8ed24b1ad22ec2e7efea049b8737-Paper.pdf)
- Towards Faithfully Interpretable NLP Systems: How should we define and evaluate faithfulness? *Jacovi & Goldberg, 2020* [ACL](https://www.aclweb.org/anthology/2020.acl-main.386/)

**Robust Explanation**

- Interpretation of Neural Networks Is Fragile. *Ghorbani et. al., 2019* [pdf](https://www.aaai.org/ojs/index.php/AAAI/article/view/4252)

- Fooling LIME and SHAP: Adversarial Attacks on Post hoc Explanation Methods. *Slack et. al., 2020* [pdf](https://arxiv.org/pdf/1911.02508.pdf)

- Robust and Stable Black Box Explanations. *Lakkaraju et. al., 2020* [pdf](https://proceedings.icml.cc/static/paper_files/icml/2020/5945-Paper.pdf)
### Evaluating Interpretability
> Evaluate interpretability (does the explanations make sense to human or not).

- **Towards A Rigorous Science of Interpretable Machine Learning.** *Doshi-Velez & Kim. 2017* [pdf](https://arxiv.org/pdf/1702.08608.pdf)
- 'It's Reducing a Human Being to a Percentage'; Perceptions of Justice in Algorithmic Decisions *Binns et al., 2018* [pdf](https://arxiv.org/pdf/1801.10408)
- Human Evaluation of Models Built for Interpretability.  *Lage et. al., 2019* [pdf](https://aaai.org/ojs/index.php/HCOMP/article/view/5280/5132)
- Interpreting Interpretability: Understanding Data Scientists' Use of Interpretability Tools for Machine Learning. *Kaur et. al., 2019* [pdf](https://dl.acm.org/doi/pdf/10.1145/3313831.3376219)
- Manipulating and Measuring Model Interpretability. *Poursabzi-Sangdeh et al., 2021* [pdf](https://arxiv.org/pdf/1802.07810.pdf)

## 6. Useful Resources

### Courses & Talks

- **Tutorial on Explainable ML** [Website](https://explainml-tutorial.github.io/)
- Interpretability and Explainability in Machine Learning, Fall 2019 *@ Harvard University by Hima Lakkaraju* [Course](https://interpretable-ml-class.github.io/)
- Human-centered Machine Learning *@University of Colorado Boulder by Chenhao Tan* [course](https://github.com/BoulderDS/human-centered-machine-learning)
- Model Explainability Forum *by TWIML AI Podcast* [YouTube](https://www.youtube.com/watch?v=B2QBnVnbt7A) | [link](https://twimlai.com/2020-model-explainability-forum/)

### Collections of Resources
- XAI-Papers [GitHub](https://github.com/anguyen8/XAI-papers)

### Toolbox

- InterpretML [GitHub](https://github.com/interpretml/interpret)

