# ConceptARC
Information and supplementary files for Moskvichev, , A., Odouard, V. V., and Mitchell, M., “The ConceptARC Benchmark: Evaluating Understanding and Generalization in the ARC Domain”, 2023.  

## Files
-	**ConceptARC Corpus**, in the `corpus` directory.  Each of the 16 concept groups consists of 10 tasks.  Each task includes 1–4 demonstrations and 3 test inputs.   Each task is described in a .json file that is the same format as in the [original ARC dataset](https://github.com/fchollet/ARC).  The JSON format gives the demonstration grids under “train”.  Each demonstration consists of an “input” and “output” grid, where the grid rows are represented as lists of numbers inside square brackets.  Each number corresponds to a pixel color in the grid.  The test inputs are given under “test”, with input and output grids represented in the same way as in the “train” section.

-	**ConceptARC Minimal Tasks**, in the `MinimalTasks` directory.  Each of the minimal tasks corresponds to one of the 16 concept groups, and is meant to be very simple.  We used these as 'attention checks' in our human studies, to make sure participants understood the overall task.  We did not include the Minimal Tasks in reporting our results on LLMs or on humans.  

- **ConceptARC Data**, in the file `data.xlsx`. This excel file contains all the data collected in our studies of human and machine solvers.   The Machine Solver Performance sheet gives the results of the first- and second-place ARC-Kaggle programs, as well as GPT-4, on every test input in ConceptARC.  (Each task contains three test inputs, which are indexed 0, 1, 2) The Human Performance sheet gives results for the human participants in our study.  Note, in the paper, we did not include results on the “minimal” problems that were used to screen human participants, but we do include them in this file.  

- **ARC Task Editor**, in the `editor` directory.  A visual editor that can be used to create or edit ARC tasks in a web browser.  This editor was developed by our group (and features some improvements over Chollet’s original ARC editor). The directory contains its own readme on how to use the editor (you simply open `index.html` in your browser). [Here is the original arc editor repository](https://github.com/victorvikram/arc-site.git).  

## URLs
[arXiv preprint](https://arxiv.org/abs/2305.07141)

[Original ARC dataset](https://github.com/fchollet/ARC)

## Citing the ConceptARC Corpus
Anyone is free to use the ConceptARC corpus for research.  If you do use it, please cite this GitHub repository and our paper.   

