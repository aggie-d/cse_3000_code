# code_3000
Collection of Assignments for CSE 3000: Contemporary Issues in Computer Science and Engineering

_Note_: Odd-numbered assignments are in HuskyCT, while even-numbered assignments are found in this repo and can be submitted to Gradescope via a Github connection.

## Personal Statement on Ethics

I am entering the CS workforce soon, and the ethical nightmare I most want to avoid is building something that harms people who never knew they were part of it. The course modules in this repo deal with these kinds of "nigthmares". The mods cover topics like models that never use a protected attribute but still produce biased outcomes through proxies like zip code, "anonymized" data can be linked back to real people, and weighing compute vs. the environment.

From that, the value I hold is accountability to the people affected by what I build, especially those who have no say in it. I want to be able to explain a model's behavior, and I care how my work affects the people that use it, not only whether it scores well. I hold this value because code that I write won't just be graded, but other people will rely on it, and they will trust it without being able to check it.

In practice, that means there are things I can't do. I can't relaease a model  without checking whether its outcomes differ across groups, and I can't call data "anonymous" without testing whether it can be re-identified through other ways. I also won't treat a strong accuracy number as a benchmark to show that something is fair, safe, or finished. Accuracy is an engineering goal, not an ethical one, and according to Chapter 5, these 2 things cannot be lumped together.

To ensure I stick to this statement, I plan to build these checks into my workflow instead of trying to tack them onto the end of a project. I can use the things I learned in these homework assignemnts to help, such as auditing for bias with SHAP, attempting re-identification before releasing data, and considering the energy cost of the compute I use. Additionally I will also ask for differing perspectives from others to review my work. 

## Outline of Assignments

### Module 02: Bot Predictor
Your goal is to build a machine learning model using given data and a Python template. You'll make changes to the GradientBoostingClassifer in mod02_build_bot_predictor.py and then test your changes in mod02_test_bot_predictor.ipynb. Can you minimize the misclassification rate on the test set?

### Module 04: Model Bias
You are given a model that was built to predict a mystery variable using zip code, income, and education level. The variable "group" represents a demographic that is prohibited and was NOT used in the model. Your goal is to use the SHAP package to review this model for bias.

### Module 06: Data De-Anonymization
Your goal is to connect anonymized data back to its source data and check the match rate. To complete this activity, write functions in the "deanonymize" script to (1) link the records in the two datasets and (2) calculate the rate at which you are successful doing so. 

### Module 08: Sustainability in Computing
You will be given a toy dataset and have the opportunity to explore the potential effects of choosing sustainable energy sources to perform computations. You'll code the energy calculation in "sustainability calculations" script, and then you can review the results of various decisions in the "check calculations" notebook. 
