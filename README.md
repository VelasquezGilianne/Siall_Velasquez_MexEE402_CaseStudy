MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## Members

| Name | Student Number | Section |
|---|---|---|
| Siall, Mohammad Addnan L. |23-06554 |MEXE 4101 |
| Velasquez, Gilianne A. |23-00244 |MEXE 4101 |

## Notebook links

| Chapter | Siall | Velasquez |
|---|---|---|
| Ch1_2_3 | [link](https://colab.research.google.com/drive/11IgNhOBGKBHjY8JbxZuKkqRgPNIcEp9-) | [link](https://colab.research.google.com/drive/1Wd3RUYWeoFw3hq0SGV8CCfcu-Sw8l30S?usp=drive_link) |
| Ch4 | [link](https://colab.research.google.com/drive/1zbJqbtwNbeLdJ4z2qe6psNxZ4xJBvq1G)| [link](https://colab.research.google.com/drive/1hj2U2LnLJpSy4UZ8Pr9MvzLTzx5p9GnQ?usp=drive_link) |
| Ch5 | [link](https://colab.research.google.com/drive/1WNSboYuqDqM-sMxzvVjbUdlSaiA8uEQJ) | [link](https://colab.research.google.com/drive/1dsWLDwDpi5Uds-ll0KF3LsKbOohOgX1t?usp=drive_link) |
| Ch6 | [link](https://colab.research.google.com/drive/1Q2-7CZQPvw1_GSE4_TAJUcFTjw3CbamX) | [link](https://colab.research.google.com/drive/11nO6jsjo0Q7W4H47Ask-CqrAbtek3Vy0?usp=drive_link) |
| Ch7 | [link](https://colab.research.google.com/drive/1kf-6nhBGedsdh6SkIBBvc8cMM1Ob3RIc) | [link](https://colab.research.google.com/drive/19dbk1rqC9IMJgAyxFVliJDjM9mCmi9jP?usp=drive_link) |
| Ch8 | [link](https://colab.research.google.com/drive/1kvw6VpmbztUMvNyZC4kG_MFspJJsr3Aw) | [link](https://colab.research.google.com/drive/1sXMXlC0wAdtCcnSB6qp_TwTDlAykoHvU?usp=drive_link) |
| Ch9 | [link](https://colab.research.google.com/drive/1jO1hMQgcDf6sQcriuyT8v9zjsV5ZObJv) | [link](https://colab.research.google.com/drive/1pybjNwv4GC54c6eOBdKbPJwQTRLQJ8C5?usp=drive_link) |

## What we learned

### Chapter 1_2_3:
We learned that data preprocessing is an important step in machine learning because data is not always complete, organized, or ready to use. Exploring the dataset helps me understand the information it contains and identify missing values, incorrect data, or unnecessary columns that need to be addressed. We also learned that there are different ways to handle missing data, such as replacing missing values with suitable ones or removing rows with incomplete information. Aside from this, cleaning data is not just about removing errors but also making sure that the information is suitable for analysis and can be used properly. What surprised me was that preparing the data requires careful decisions because removing or changing certain information can also affect the results.

### Chapter 4: 
We learned that feature engineering helps make data more useful by creating new features or grouping existing values to reveal patterns that may not be obvious at first. We also understood that encoding is important because it allows categorical data, such as weather conditions or levels of quantity, to be represented in a way that machine learning models can understand. Through this chapter, We realized that the data does not always have to stay in its original form because it can be transformed to provide more useful information. What surprised me was that even simple calculations, such as dividing lemonade sales by temperature or ice cubes by temperature, could help explain the relationship between variables in a different way. It made me realize that creating new features can help us understand the data better and give machine learning models more useful information to learn from. 

### Chapter 5:
We learned that scaling helps make numerical features more comparable by adjusting their values to a similar range. We also understood that there are different scaling methods, such as StandardScaler and MinMaxScaler, and that each method adjusts the data differently. Through this chapter, We realized that scaling can help prevent features with larger numerical values from having too much influence on certain machine learning models. What surprised me was that even if two features are equally important, the one with larger numbers could have a greater effect on the model. We also learned that scaling is not always necessary because it depends on the algorithm being used. 

### Chapter 6: 
We learned that outliers are values that are very different from most of the data and that they can be detected using methods such as Z-score and IQR. We also understood that these methods use different ways to determine whether a value is considered an outlier. Through this chapter, We realized that unusual values should not immediately be removed because they might still contain useful information. What surprised me was that the value 100 was considered an outlier using the IQR method but not the Z-score method. This helped me understand that the results can vary depending on the method used, so it is important to examine the data carefully before deciding what to do with an outlier. 

### Chapter 7:
  This chapter was all about feature selection and we learnt how filtering out useless data so the language learning models can be trained better. We learnt the different philosophies behind it: filter methods use correlation, wrapper methods use overall scoring, and embedded methods act like a sculptor chipping away data during training. The biggest surprise to us was when we ran the wrapper method of RFECV, printing out the features selected showed a long list of warnings. We first assumed it to be an error but just before the warning, we observed it already selected the 'assignments completed'. The final table itself was rather surprising too as even though filter, and embedded have overlapping feature, all three selection method choices were unique.  

### Chapter 8:
  What we learnt from this chapter is the construction of a preprocessing pipeline. This meant shifting from manual, time-consuming data preparation, to a more automated and sequential process. Instead of performing imputation and scaling in individual cells, it was performed as is in a single cell. To us, this taught that if you want to keep a workflow clean and less redundant in a single cell, a pipeline usage is highly efficient.

### Chapter 9 :
  This chapter gave us the chance to put preprocessing techniques learnt from the previous lessons such as: data cleaning, transformation, reduction, discretization, and encoding, into real-world practice. However, the most important takeaway was the use of data visualization. Plots like bar graphs, boxplots, histograms, point plots, distribution graphs, and heatmaps allows us to see exactly what the data represents in a clean, orderly way. Much like preprocessing makes data easier for a machine learning model to train on, visualization makes data easier for us to understand.

## Errors we found

### Error found on CHAPTER 6:

Error: `outliers = data[np.abs(z_scores) > 3]`
Corrected Version: `outliers = data[np.abs(z_scores) > 2]`

The error is in the threshold. The z-score of 100 is only 2.615, which is less than 3, so the ``condition np.abs(z_scores) > 3`` returns an empty array and 100 is not flagged even though it is clearly an outlier. This happens because 100 itself raises the mean and standard deviation, which lowers its own z-score. With a small dataset of only eight values, a z-score above 3 is hard to reach. Changing the threshold to 2 fixes this, since 2.615 > 2 while every other value has an absolute z-score below 0.6, so the output becomes Outliers: ``[100].``

### Error found on CHAPTER 7:

Error: `selector = RFECV(estimator, step=1, cv=5)`

Corrected Version: `selector = RFECV(estimator, step=1, cv=3)`

The error is in the number of cross-validation folds. With cv=5, the dataset is split into five folds, and each fold must contain enough samples to score. The warning “R^2 score is not well-defined with less than two samples” shows that some test folds contain only one sample, which means the dataset is too small for five folds. R² cannot be computed on a single sample, so every fold returns an undefined score and the selection becomes unreliable. Changing to cv=3 creates larger test folds, each with at least two samples, so R² can be computed and the warnings disappear.

### Errors found on CHAPTER 9:

Error: `plt.hist(data['Age'].dropna(), alpha=0.5, label='Before discretization')`

Corrected Version: `plt.hist(data['Age'].dropna(), alpha=0.5, label='After discretization')`

The label is wrong. The histogram shows the categories Adult, Elderly, and Child on the x-axis, which means data['Age'] was already discretized when this plot was made. Since the plot shows the data after discretization, the label should be ‘After discretization’ instead of ‘Before discretization’.


Error: `plt.hist(titanic_preprocessed[:,2], alpha=0.5, label='After discretization')`

Corrected Version: `plt.hist(titanic_preprocessed[:,0], alpha=0.5, label='Before discretization')`

The wrong column is plotted. titanic_preprocessed[:,2] only contains the values 0.0 and 1.0, so it is a binary or encoded column and does not show the age distribution. Column 0 holds the original continuous age values, so titanic_preprocessed[:,0] is the correct choice, and it should be labeled ‘Before discretization’.

## Note on AI tools

We used AI as a supporting tool to help us correct the errors we identified in the code. After locating the possible errors, we provided the incorrect and expected lines of code to the AI and used its explanations to better understand why the changes were necessary. AI helped us compare the codes, identify differences in parameters, labels, and data being used, and explain how these errors could affect the results of the program. However, we still reviewed the suggested corrections and made sure that they were consistent with the concepts and procedures discussed in the notebook.

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
