# unsupervised-machine-learning-challenge
Module 20 Challenge

# Background
You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.

# Part 1: Prepare the Data
Read myopia.csv into a Pandas DataFrame.

![image](https://user-images.githubusercontent.com/112498067/222933123-9fb734ef-fb1f-467d-8e8c-ba5b9778a679.png)

Remove the "MYOPIC" column from the dataset.

![image](https://user-images.githubusercontent.com/112498067/222933137-1d1186eb-7c04-4d41-9337-22b05fd5d1a4.png)

Standardize your dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

![image](https://user-images.githubusercontent.com/112498067/222933156-57414412-1320-4729-9cd9-884b36bf7010.png)
![image](https://user-images.githubusercontent.com/112498067/222933165-8ae4ec2a-954d-4662-8399-6d6c27bb4ffa.png)
![image](https://user-images.githubusercontent.com/112498067/222933168-78b6b273-4935-485e-987e-17fcb23c6be9.png)

# Part 2: Apply Dimensionality Reduction
Perform dimensionality reduction with PCA. How did the number of the features change?
![image](https://user-images.githubusercontent.com/112498067/222933185-b1c5796f-ff47-45a7-af44-83bc88ab0a33.png)

Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.

Create a scatter plot of the t-SNE output. Are there distinct clusters?

![image](https://user-images.githubusercontent.com/112498067/222933231-453649c4-6381-483e-86c5-90b1e2125e9a.png)

# Part 3: Perform a Cluster Analysis with K-means

Create an elbow plot to identify the best number of clusters. Make sure to do the following:

- Use a for loop to determine the inertia for each k between 1 through 10.

- If possible, determine where the elbow of the plot is, and at which value of k it appears.

![image](https://user-images.githubusercontent.com/112498067/222933270-e74be444-f25f-433f-8cec-05c1da25efde.png)

# Part 4: Make a Recommendation

Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook. Can the patients be clustered? If so, into how many clusters?

![image](https://user-images.githubusercontent.com/112498067/222933307-e847f43b-5026-4739-8107-f7d2c0539b44.png)





