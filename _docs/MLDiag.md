## MLDiag

MLDiag introduces several model tests to ensure its robustness and disposal to go to production.
We categorize theses tests into several categories and different scenario related to the model task.

### Descriptive
Descriptive tests highlight some model failures or success regarding dataset statistics.

| Test| Data | Target(s)|  Description |  
|:---:|:---:|:---:|:---:|
|Length| Text| Classification, NER | how data length impacts model errors (e.g. a text classification model always fails on short texts |
|Similar| Text, Image| Classification | does the model make always the same error (e.g. a classification model that fails in a whole category or in a cluster of very similar data |


### Invariance
Inputs data are perturbed while measuring there impact on model prediction. 
This is closely related to data augmentation techniques, 
where we apply perturbations to inputs during training while preserving the original label. 
The problem with a `brut force` data augmentation is its computation cost. 
Using MLDiag tests, we can observe which perturbations affect the current model.
We then define the set of augmentations that improve model consistency.

The list of implemented model invariance tests is the following:

| Test| Data | Target(s)|  Invariance |  
|:---:|:---:|:---:|:---:|
|Spell| Text| Classification, NER|spelling mistakes|
|Pronoun| Text| Classification, NER| changing pronoun words|
|Sent-Order| Text| Classification, NER| sentence disorder|
|Rotation| Image| Classification, Detection| image rotation |
|Occlusion| Image| Classification, Detection| partial object occlusion |

