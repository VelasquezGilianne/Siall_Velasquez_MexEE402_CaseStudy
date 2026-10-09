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

| Chapter | Member 1 | Member 2 |
|---|---|---|
| Ch1_2_3 | https://colab.research.google.com/drive/11IgNhOBGKBHjY8JbxZuKkqRgPNIcEp9- | https://colab.research.google.com/drive/1Wd3RUYWeoFw3hq0SGV8CCfcu-Sw8l30S?usp=drive_link |
| Ch4 | https://colab.research.google.com/drive/1zbJqbtwNbeLdJ4z2qe6psNxZ4xJBvq1G| https://colab.research.google.com/drive/1hj2U2LnLJpSy4UZ8Pr9MvzLTzx5p9GnQ?usp=drive_link |
| Ch5 | https://colab.research.google.com/drive/1WNSboYuqDqM-sMxzvVjbUdlSaiA8uEQJ | https://colab.research.google.com/drive/1dsWLDwDpi5Uds-ll0KF3LsKbOohOgX1t?usp=drive_link |
| Ch6 | https://colab.research.google.com/drive/1Q2-7CZQPvw1_GSE4_TAJUcFTjw3CbamX | https://colab.research.google.com/drive/11nO6jsjo0Q7W4H47Ask-CqrAbtek3Vy0?usp=drive_link |
| Ch7 | https://colab.research.google.com/drive/1kf-6nhBGedsdh6SkIBBvc8cMM1Ob3RIc | https://colab.research.google.com/drive/19dbk1rqC9IMJgAyxFVliJDjM9mCmi9jP?usp=drive_link |
| Ch8 | https://colab.research.google.com/drive/1kvw6VpmbztUMvNyZC4kG_MFspJJsr3Aw | https://colab.research.google.com/drive/1sXMXlC0wAdtCcnSB6qp_TwTDlAykoHvU?usp=drive_link |
| Ch9 | https://colab.research.google.com/drive/1jO1hMQgcDf6sQcriuyT8v9zjsV5ZObJv | https://colab.research.google.com/drive/1pybjNwv4GC54c6eOBdKbPJwQTRLQJ8C5?usp=drive_link |

## What we learned

One short paragraph per chapter, Ch1_2_3 to Ch9. Say what the chapter taught
you and what surprised you. Not what the library does, but what you understood.

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
