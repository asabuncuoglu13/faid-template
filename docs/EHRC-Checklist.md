# Using FAID in Scope of EHRC’s AI Guidance

FAID (Fair AI Development) is an open-source fairness monitoring and management tool that developers can integrate into their machine learning (ML) pipelines. As the developers of FAID, it is also our shared responsibility to guide other developers on how to integrate FAID in a fairness by design approach.

In this document we will use the term “AI infused systems” as an umbrella term for all the systems that learn from previously collected data to define pattern-based rules.

## Integrating an open-source project into your codebase

As AI models become more widespread, it’s increasingly important to evaluate open-source tools from a human rights perspective. Traditionally, auditing open-source libraries has focused on performance, security, and privacy. However, with AI models now being core components in many libraries and APIs, these audits must also consider the impact on human rights and fairness. Additionally, as new AI-first programming languages emerge—designed to support various modalities, inference engines, and training methods—there is a need to integrate human rights and fairness assessments into every stage of the auditing process for open-source libraries.

## Data flow of FAID

The following diagram illustrates a high-level overview of FAID's dataflow. Note that the library does not interact with model training data or system-level data. It only collects metadata information if the developer explicitly decides to include it into fairness management flow.

![Overview of metadata flow](./media/faid-flow-overview-wlibs.png)

## Checklist After Integrating FAID

**The below list is adopted from [EHRC](https://www.equalityhumanrights.com/guidance/artificial-intelligence-checklist-public-bodies-england). You can also customise this checklist for integrating other open source software based on your needs.**

1. [ ] We know the meaning of the following protected characteristics and what are the implications of using them in the AI-infused systems. (Protected attributes: Age, disability, gender reassignment, pregnancy and maternity (which includes breastfeeding), race, religion or belief, sex, sexual orientation.)
2. [ ] We identified if and how we (or others on your behalf) use the developed model, and considered how the regulations applies.
3. [ ] We collected necessary evidence to identify and address any research and implementation gaps that can cause a discriminative harm.
4. [ ] We reviewed how the AI could affect people with different protected characteristics either positively or negatively.
5. [ ] We assessed the potential and actual impact by looking at the equality evidence to evaluate if the AI model can potentially cause discrimination.
6. [ ] We assessed the potential and actual impact by looking at the equality evidence to evaluate if the AI model can potentially help eliminate discrimination.
7. [ ] We assessed the potential and actual impact by looking at the equality evidence to evaluate if the AI model can potentially contribute to advancing equality of opportunity.
8. [ ] We assessed the potential and actual impact by looking at the equality evidence to evaluate if the AI model can potentially affect good relations.
9. [ ] We used the results of the equality impact assessment when developing the AI-related features.
10. [ ] We recorded the fairness decisions and considerations throughout the development regularly.

**Below is adopted from [fairlearn](https://fairlearn.org/), which is originally published by Jacobs and Wallach, called “construct validity:” We can use it to detailly analyse if 4,5,6,7,8 are assured.**

1. [ ] Do the measurements produced by the model appear plausible on the surface?

2. [ ] Is there a single understanding of the theoretical construct, or is it contested and context-dependent?

3. [ ] Does the model contain the observable properties and related unobservable theoretical constructs specific to the construct of interest?

4. [ ] Does the model appropriately capture relationships between the construct of interest and the measured observable properties and related unobservable theoretical constructs?

5. [ ] Do the measurements obtained correlate with other established measurements for which construct validity has been established?

6. [ ] Do the measurements for the construct of interest correlate appropriately with related constructs?

7. [ ] Are the measurements obtained predictive of relevant observable properties or other unobservable theoretical constructs?

8. [ ] Are the hypotheses emerging from the measurements substantively interesting and relevant?

9. [ ] What are the societal impacts and consequences of using the measurements?

10. [ ] How is the world shaped by using the measurements, and what societal outcomes do we desire?

**And, below is adopted from [Ethics Guidelines for Trustworthy AI](https://digital-strategy.ec.europa.eu/en/library/ethics-guidelines-trustworthy-ai) (EU High-Level Expert Group, 2019):**

11. [ ] We established a strategy or a set of procedures to avoid creating or reinforcing unfair bias in the AI system, both regarding the use of input data as well as for the algorithm design.
    - Did you assess and acknowledge the possible limitations stemming from the composition of the used data sets?
    - Did you consider diversity and representativeness of users in the data? Did you test for specific populations or problematic use cases?
    - Did you research and use available technical tools to improve your understanding of the data, model and performance?
    - Did you put in place processes to test and monitor for potential biases during the development, deployment and use phase of the system?

12. [ ] We ensured a mechanism that allows others to flag issues related to bias, discrimination or poor performance of the AI system.
    - Did you establish clear steps and ways of communicating on how and to whom such issues can be raised?
    - Did you consider others, potentially indirectly affected by the AI system, in addition to the (end)-users?
    - Did you assess whether there is any possible decision variability that can occur under the same conditions?
    - If so, did you consider what the possible causes of this could be?
    - In case of variability, did you establish a measurement or assessment mechanism of the potential impact of such variability on fundamental rights?

13. [ ] We ensured an adequate working definition of “fairness” that we apply in designing AI systems.
    - Is your definition commonly used? Did you consider other definitions before choosing this one?
    - Did you ensure a quantitative analysis or metrics to measure and test the applied definition of fairness?
    - Did you establish mechanisms to ensure fairness in your AI systems? Did you consider other potential mechanisms?


## Useful FAID Features Fill Out this Checklist

1. For the checklist items 5, 6, 7, and 8, developers can directly use FAID’s comparison feature.

```
#TODO: Add example use
```
 
2. For the checklist items 11, 12, and 13, developers can directly use FAID’s evaluation metrics and fairness indicators.

```
#TODO: Add example use
```

