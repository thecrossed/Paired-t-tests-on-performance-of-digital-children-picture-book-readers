# Paired-t-tests-on-performance-of-digital-children-picture-book-readers
In this project, I made two matrices illustrating paired t-test results(score difference and p-value) on the performance of 
digital children picture book readers.

The dataset contains 111,536 rows of user learning data unequally distributed on 72 digital books. The user page(sentence) score was 
evaluated from a third-party service embedded in our program. Our content team planned to use this evaluation score as an indicator 
to classify content difficulty levels. This analysis offered an overview for further research.

My main steps are listed below: 
1) collect initial data from our database with SQL commands;
2) remove extreme values and null values;
3) aggregate the mean page(sentence) score of each book as the book score;
4) merge the book title data into this dataset;
5) group every two books into a pair, 2,556 pairs in total;
6) select the common readers in each pair;
7) calculate the paired t-test result (score difference and p-value) on book score in each pair; 
8) visualize the 2,556 score differences into a matrix; the darker the color, the lower the book score;
Please see **score_difference_matrix.png**
9) visualize the 2,556 p-values into a matrix; the darker the color, the lower the p-value(the more significant of the result).
Please see **pvalue_matrix.png**

For detailed code, please see **Paired T-Test Matrix on Performance of Digital Children Picture Book Readers.ipynb**.
