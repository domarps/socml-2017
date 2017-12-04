## Interpretability
- ill-specified field
- There are different motivations for interpretability
- The interpretability of models also varies with context

#### Definitions

##### Desire for agency

* How some trigger (e.g., a couple of features) is elucidating a different behavior to the system. How each feature ended up contributing to the behavior

* The goal of interpretability also creates mismatches on what the notion of interpretability is

* Some causal representation or what the ultimate objective is can also influence interpretability

##### Causality

* Given a model, how the inputs influence the model? Sometimes i is easier to talk about case uses: how can the model help the target users to make decisions? End-users are interested in having a backup reasoning about what their results mean

* Sometimes what the end-user wants to use may not be aligned with the truth. Ethics and responsibility may play an important and complicated model

* What to do when the results of a model (e.g., decision tree) do not agree with the results of a predictive model (neural network)? Providing good information targeted to the end-user gains their trust

##### Interpretability as rhetoric

* building trust with end-users by providing “convincing” arguments for them to accept/use a model. Simplicity of language and/or language that is targeted to a specific audience may be key

##### Misnomers and interpretability

* Technical terms have different meanings, what “modeling” means in ML has a different interpretation for different fields

* For humans, we can have different levels of complexity for explanations. Choosing an adequate level for an end-user is also an important factor.

* If we can say that a model works with a certain level of confidence (statistically speaking), then it should not be hard to convince an end-user about the model’s interpretability.

* It is dangerous to take a bottom-up approach in order to justify research. The ML field is in need of more UX studies that could help with interpretability issues. More of these studies can help the research process.

* It is important that the notion of interpretability originates from human reasoning.

## Industry and Interpretability

For the use in industry and with actual end-users, sometimes accuracy is sacrificed for interpretability: a particular model provides a better explanation for them than a more accurate one. End-users also sometimes provide expert feedback that contradict the results of a model and the researcher has to look at more data and understand if the contradiction is the result of a failure from the model or just an inaccuracy. The hardest step for a researcher is to choose what to do next: how to gather more data? What kinds of queries she should be exploring? What are the following steps?

Some options to decide on what to do next may include some feature visualization, for example: how to tweak a neuron in order to activate more?: using jitter (shift by one pixel between updates), ask for an image that activates the neuron
For automated machine learning, when we don’t know the model in advance, the calculation of a feature importance matrix (what factors can influence the model most) could help to convey the meaning of the results.

The way we interpret linear models is inadequate. The explanation about a model and its format are factors to consider when providing a way to interpret a model for the end-user.

The idea of interpretability regarding linear models stems from Occam’s Razor and some experiments require complexity in order to be able to interpret them.

Journal of research: https://distill.pub/

