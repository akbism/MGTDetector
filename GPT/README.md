To reproduce the research, please create a GPT folder and set it as the root path.
Keep all data (text files or csv files) in respective folders inside the GPT folder.

Then run the scripts as per the below sequence:
- 1_detectGPT_and_GPTZero.ipynb
This should provide the DetectGPT, GPTZero labels, probability and several scores including perplexity, perplexity per line, burstiness etc. 

- 2_EDA.ipynb
This script should provide the exploratory data analysis over the datasets. We can find the Lexical diversity, The Flesch reading ease test score, The automated readability index (ARI) etc.
IT also provides several analaysis at token and sentence level.

- 3_Feature_Engg.ipynb
This script is still in-proecss. It is supposed to create manual features.

- 4_roberta-base-openai-detector.ipynb
This script is to run RoBERTa Sequence Classifier for the binary classification problem of machine generated text detection.

- 5_attacker.ipynb
This script should provide a simple method to find the most important words for the RoBERTa detector. Then, replace the top 10-15 words by low probability synonyms and provide the modified text.
