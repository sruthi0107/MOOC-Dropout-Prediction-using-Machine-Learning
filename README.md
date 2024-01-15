# MOOC-Dropout-Prediction-using-Machine-Learning

This repository contains the code for the Dropout prediction in online courses using Machine Learning. The KDDCup-15 dataset was used in this work. The link to the dataset is given [here](http://moocdata.cn/challenges/kdd-cup-2015)

## Abstract
Online learning has gained traction over recent years, especially since online education has become more widespread. However, it comes with its own set of challenges of 
which high dropout is still a major one. Identifying at-risk learners at an early stage is pivotal to offering personalized attention that can potentially prevent them from dropping out from the online courses. This work proposes two methods to analyze students’ progress in an online course and subsequently identify dropout prone students. The first method performs fusion of course activity features by concatenating previous weeks’ features before training. The second method extracts course activity features from the start date of the courses to a current week instead of concatenating as the first method does. A set of machine learning models and an ensemble framework were trained and tested on these two types of feature sets. On evaluating the models, the benchmark dataset KDDCup15 has been used, where the first method yielded an F1-score 91% while the second method yielded a score 92%. It was observed that both feature fusion methods produce comparable results although we expected that the concatenation of the features over 
time would produce better results. We also found that using features over a longer duration of time can help in achieving better performance. Further, ensemble model consistently outperformed the base classifiers.

## Implementation details
- 10 out of 39 courses were used
- Run the required_train_users_generation.ipynb and required_test_users_generation.ipynb to get the logs for the courses that were considered
- To run the training scripts for method-1 and method-2, navigate inside the respective folder and run notebooks/training_method1 and notebooks/training_method2.
- For further details, refer to [this](https://doi.org/10.1109/ICKECS56523.2022.10059775) paper.

## Results
- The graphs below depict the Accuracy vs weeks and AUC vs weeks curve for Method-1
(Graphs/weeks_vs_accuracy_method1)
(Graphs/weeks_vs_AUC_method1)
- The graphs below depict the Accuracy vs weeks and AUC vs weeks curve for Method-2
  Graphs/weeks_vs_accuracy_method2)
  Graphs/weeks_vs_AUC_method2)

## Citation
If you use this work in your research, kindly cite this paper. The citation for the paper is as follows: 
```
@INPROCEEDINGS{10059775,
  author={Srinivasan, Sruthi and Dewan, M. Ali Akber},
  booktitle={2022 International Conference on Knowledge Engineering and Communication Systems (ICKES)}, 
  title={An Ensemble Framework for Dropout Prediction in Online Learning}, 
  year={2022},
  volume={},
  number={},
  pages={1-7},
  doi={10.1109/ICKECS56523.2022.10059775}}
```
