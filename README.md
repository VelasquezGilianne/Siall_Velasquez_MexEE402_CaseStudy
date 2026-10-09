# MexEE 402: Data Preprocessing Case Study

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

Chapter 1_2_3: I learned that data preprocessing is an important step in machine learning because data is not always complete, organized, or ready to use. Exploring the dataset helps me understand the information it contains and identify missing values, incorrect data, or unnecessary columns that need to be addressed. I also learned that there are different ways to handle missing data, such as replacing missing values with suitable ones or removing rows with incomplete information. Aside from this, cleaning data is not just about removing errors but also making sure that the information is suitable for analysis and can be used properly. What surprised me was that preparing the data requires careful decisions because removing or changing certain information can also affect the results.

Chapter 4: I learned that feature engineering helps make data more useful by creating new features or grouping existing values to reveal patterns that may not be obvious at first. I also understood that encoding is important because it allows categorical data, such as weather conditions or levels of quantity, to be represented in a way that machine learning models can understand. Through this chapter, I realized that the data does not always have to stay in its original form because it can be transformed to provide more useful information. What surprised me was that even simple calculations, such as dividing lemonade sales by temperature or ice cubes by temperature, could help explain the relationship between variables in a different way. It made me realize that creating new features can help us understand the data better and give machine learning models more useful information to learn from. 

Chapter 5: I learned that scaling helps make numerical features more comparable by adjusting their values to a similar range. I also understood that there are different scaling methods, such as StandardScaler and MinMaxScaler, and that each method adjusts the data differently. Through this chapter, I realized that scaling can help prevent features with larger numerical values from having too much influence on certain machine learning models. What surprised me was that even if two features are equally important, the one with larger numbers could have a greater effect on the model. I also learned that scaling is not always necessary because it depends on the algorithm being used. 

Chapter 6: I learned that outliers are values that are very different from most of the data and that they can be detected using methods such as Z-score and IQR. I also understood that these methods use different ways to determine whether a value is considered an outlier. Through this chapter, I realized that unusual values should not immediately be removed because they might still contain useful information. What surprised me was that the value 100 was considered an outlier using the IQR method but not the Z-score method. This helped me understand that the results can vary depending on the method used, so it is important to examine the data carefully before deciding what to do with an outlier. 

  Chapter 7:
  This chapter was all about feature selection and we learnt how filtering out useless data so the language learning models can be trained better. We learnt the different philosophies behind it: filter methods use correlation, wrapper methods use overall scoring, and embedded methods act like a sculptor chipping away data during training. The biggest surprise to us was when we ran the wrapper method of RFECV, printing out the features selected showed a long list of warnings. We first assumed it to be an error but just before the warning, we observed it already selected the 'assignments completed'. The final table itself was rather surprising too as even though filter, and embedded have overlapping feature, all three selection method choices were unique.  

  Chapter 8:
  What we learnt from this chapter is the construction of a preprocessing pipeline. This meant shifting from manual, time-consuming data preparation, to a more automated and sequential process. Instead of performing imputation and scaling in individual cells, it was performed as is in a single cell. To us, this taught that if you want to keep a workflow clean and less redundant in a single cell, a pipeline usage is highly efficient.

  Chapter 9 :
  This chapter gave us the chance to put preprocessing techniques learnt from the previous lessons such as: data cleaning, transformation, reduction, discretization, and encoding, into real-world practice. However, the most important takeaway was the use of data visualization. Plots like bar graphs, boxplots, histograms, point plots, distribution graphs, and heatmaps allows us to see exactly what the data represents in a clean, orderly way. Much like preprocessing makes data easier for a machine learning model to train on, visualization makes data easier for us to understand.

## Errors we found

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

## Note on AI tools

Say whether you used an AI tool, and what for. This is not a penalty.
Hiding it is.

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
