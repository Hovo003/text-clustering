# text-clustering
Clustering of questions and evaluating based on original labels

Project Structure
data/: Contains the initial dataset only.

prompts/: Includes 3 prompt files used to guide Mistral, a large language model, in clustering the questions.

outputs/: Contains:

CSV files with the clustered questions (each labeled under the instruction column).

A JSON file (labels_for_evaluation.json) used for evaluation purposes.

For each prompt:

A CSV file is generated containing the clustered questions, with instruction, name, and description columns.

A corresponding JSON file summarizes the results, including the name, description, and the number of questions assigned to each cluster.

Code Overview
LLM_pipeline.ipynb: This Jupyter notebook provides a step-by-step walkthrough of the entire clustering and evaluation process.

It performs clustering using all three prompts.

It evaluates the quality of clustering against original labels.

The best-performing prompt is identified as Prompt 1.

Evaluation results can be found in the final section of the notebook (last output cell).

Output Summary
The best clustering result is summarized in: Mistral_prompt1_final_cluster_summary.json
