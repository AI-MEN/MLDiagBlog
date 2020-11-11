---
title: Related Work
description: Machine learning model evaluation and diagnosis
---
## Related Work

Recent works have tackled the model evaluation step.

Naike et al. proposed in this [paper](https://arxiv.org/pdf/1806.00692.pdf) 
in ICCL 2018 an evaluation methodology consisting of automatically constructed “stress tests” that allow to examine whether systems have the ability to make real inferential decisions. 
An evaluation of six sentence-encoder models on these stress tests reveals strengths and weaknesses of these models with respect to challenging linguistic phenomena.
`TODO` 

Belinkov and Binsk find in this [study](https://arxiv.org/pdf/1711.02173.pdf) 
in ICLR 2018 that state-of-the-art models fail to translate even moderately noisy texts that humans have no trouble comprehending. 
This study helped them to explore approaches that increase model robustness using structure-invariant word representations and robust training on noisy texts.
`TODO`

Odena et al. introduced in this [paper](http://proceedings.mlr.press/v97/odena19a/odena19a.pdf) 
in MLR 2019 testing techniques for neural networks that can discover errors occurring only for rare inputs, called *Coverage-Guided Fuzzing (CGF)* methods, 
which are random mutations of inputs guided by a coverage metric toward the goal of satisfying user-specified constraints.
`TODO` 

Rychalska et al performed in their [work](https://pdfs.semanticscholar.org/8562/5148efbf0e556f9ae8145f0873e7c98a74bf.pdf) 
of ICNIP 2019 adversarial training on selected aspects and checked its transferability to the improvement of models with various corruption types.
`TODO`

Ribeiro et al. introduced in this [paper](https://homes.cs.washington.edu/~marcotcr/acl20_checklist.pdf) 
in ACL 2020 a task-agnostic methodology for testing NLP models, called *CheckList*.
`TODO` 

Jordan proposed in his [blog](https://www.jeremyjordan.me/testing-ml/?utm_campaign=Data_Elixir&utm_source=Data_Elixir_300) 
in 2020 two behavior testing recipes to address the model testing step:
- *Pre-train tests* that allow us to identify some bugs early on and short-circuit a training job.
- *Post-train tests* use the trained model artifact to inspect behaviors for a variety of important scenarios that we define.
