# Udacity Data Science Nanodegree projects

This repository contains mostly Jupyter notebooks delivered as projects in the [Data Scientist Nanodegree by Udacity](https://www.udacity.com/course/data-scientist-nanodegree--nd025)

## Data Science Blog
Jupyter notebook analyzing data from the 2020 Stack Overflow survey
The CSV with the data needed in the notebook can be downloaded from [StackOverflow](https://insights.stackoverflow.com/survey)

### Motivation

The motivation for this project is to gather data-driven analysis of programming languages usage, trends and their possible connection to job satisfaction.

### Libraries used
- pandas 1.2.1
- scikit-learn 0.24.1

### Files
- [Jupyter notebook](https://github.com/mpejcoch/data-science-nanodegree/blob/main/1-data-science-blog/programming-languages-sosurvey.ipynb)
- survey_results_public.csv Needs to be downloaded from [StackOverflow](https://insights.stackoverflow.com/survey) for the notebook to run correctly.

### CRISP
#### Business Understanding
As an individual or a company, you will stand before a choice of technology. In particular a choice of a programming language is a complicated affair as it is something that might require a great cost when training or hiring new programmers. Figuring out the current status and trends will assist in the process. Can the choice of a programming language also influence job satisfaction of the developer?

#### Data Understanding
Over 60000 developers have answered questions about their personality, job, professional and personal preferences and salary. One question was which programming language or languages they are currently using and the next one which one they would like to learn next year.

More in the **Language popularity** section of the notebook.

#### Data Preparation
Dropping rows with incomplete answers is necessary in order to be able to run the models. Categorical variables need to be expanded to dummy variables. See more in the **Job Satisfaction** section of the notebook.

#### Modeling
I have chosen two models for the prediction of job satisfaction. **Linear Regression** and a **neural network**. Only about 0.6% of the variability of the job satisfaction data can be explained by the programming language choice. A neural network can be trained to 0.32 score, which is still too little to give reliable predictions.

#### Evaluation / Summary of the results

In the [notebook](https://github.com/mpejcoch/data-science-nanodegree/blob/main/1-data-science-blog/programming-languages-sosurvey.ipynb), you will find an analysis of:
- programming languages used
- trends for the next year
- a model to predict job satisfaction based on programming languages used

While **JavaScript** and **HTML/CSS** dominate the current ranking, **Rust** and **Julia** seem to be the trensetters.
The conclusion is that the information on programming languages used by a person is not enough to predict job satisfaction of an individual.

#### Deployment
The analysis and the model can be re-run with the new release of the survey, given that the structure of the questions remains similar. Simply by downloading the new dataset and running the notebook.

### Acknowledgements

Thanks to StackOverflow for providing the data, Udacity lectors and reviewers for guiding me through the process and all contributors of StackOverflow, especially _udibr_ for saving me a lot of time because of the simple and effective [NaN filter](https://stackoverflow.com/questions/11620914/removing-nan-values-from-an-array).