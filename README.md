RUN EXPERIMENT:

- experiment (single task).ipynb
- experiment (multi-task).ipynb

The only difference between the two is that, in the multi-task version, the model is also trained on an auxiliary task to classify the verbs into regular or irregular.

At the top of the notebook, hyperparameters can be adjusted. You can also indicate whether you want to train on type/token frequency, 
and whether you want to do experiment 1, 2, or both (as referred to in my thesis). After that, you can just 'run all'. 
At the bottom all results are saved into one excel file.
- input: all text and xslx files that are in the same folder
- output: one xlsx file that is compatible with the analysis (sgt or mtsk) notebook to analyse all results. This each line in excel is one run.


ANALYSIS:

- analysis (single task).ipynb
- analysis (multi-task).ipynb

Again, the only difference is the multi-task version containing label performance analysis because of the added auxiliary task. 

The analysis notebook assumes that experiments 1 and 2 are executed (i.e. computes overall and aggregate results based on 5 folds each run 5 times)

Make sure to open the right Excel file, and 'run all' for the analysis results as presented in my thesis
- input: xlsx file as created by the experiment notebook



DATA:

- AHresults.xlsx - A&H production probabilities (human data Wug Test)
- AHresults.xlsx - A&H ratings (human data Wug Test)
- wugs_ortho.txt - orthographic representation of all Wug Test inputs and outputs (only used for visualisation in analysis nb)
- KCamericanwugs.txt - phonetic representation from K&C repository for the 58 nonce verbs of A&H's Wug Test
- reg.txt, irreg1.txt, irreg2.txt - phonetic representations of regular, irregular 1 and irregular 2 inflections of A&H Wug Test nonce verbs (by K&C as well)
- KCamerican.txt - CELEX dataset from K&C repository (equal to A&H dataset but in American English transcription by K&C)
- my_dataset.txt - CELEX dataset that I extracted from the online CELEX database myself
- missing.txt - verbs that are missing from the A&H CELEX dataset (KCamerican.txt)


K&C repository: https://github.com/ckirov/RevisitPinkerAndPrince/tree/master
