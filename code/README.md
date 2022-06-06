# Movie Recommendation System Project
#### submitted files:
report.pdf
code/
   -- Movie_Recommendation_System.ipynb (please run this file)
   -- Movie_Recommendation_System.pdf (preview for my code)
   -- README.md (instructions to run the code)

The following are the instructions to run my code:

1. Open Movie_Recommendation_System.ipynb in Jupyter Notebook.

2. Set variable "case": for testing user-based cosine similarity, case = 1;
for testing user-based Pearson correlation, case = 2.

3. Set boolean variable "is_IUF": is_IUF = true, when testing 1.2 - 1. Inverse user frequency;
Set boolean variable "case_modification": case_modification = true, when testing 1.2 - 2. case
modification.

4. Set boolean variable "is_std": is_std = true, when testing my own algorithm based on movie controversy.

5. Run all the code blocks before the markdown cell "Algorithms -- User-based Collaborating Filtering" (remember when
  predicting different test files, the test userid range needed to be changed accordingly in some code blocks, you can find where to change by checking the code comment)

6. Run different Data Process block when implementing different algorithms:

--For user-based collaborating filtering (including basic cosine similarity, basic Pearson Correlation, extension to basic Pearson Correlation with IUF, extension to basic Pearson Correlation with case modification, my own algorithm), run the code cell under "Algorithms -- User-based Collaborating Filtering"; Then skip item-based code block and Slope One code block, go to "Check Result and Write to Output File", write to the output txt file.

--For item-based collaborating filtering, skip user-based collaborating filtering code block, only run code blocks under item-based collaborating filtering, then write to output txt file.

--For Slope one, skip user-based, item-based collaborating filtering code block, only run code blocks under Slope One, then write to output txt file.

7. You can validate your output file by running code blocks under "Validate result files" to make sure there's no null value, value > 5, or value <= 0.

8. When combining the results from two different files (each are the result files from different algorithms) to get the average
rating, run the code blocks under "Combining two algorithms results to get average rating". (for example, combine std_case with iuf_case, combine slope_one with std_iuf_case etc.) Then write to output files.
