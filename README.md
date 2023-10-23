# Hate_speech_detection

Model_1_Finetune.ipynb - contains the proposed model architecture with BiLSTM and CNN layers. It is fine-tuned with an augmented dataset with balanced classes obtained from https://data.mendeley.com/datasets/9sxpkmm8xn/1 (Mody et al., (2023))

Model_2_Finetune.ipynb - contains the base-RoBERTa model finetuned with the same dataset as that of Model-1 for comparison in performances. 

Preprocessing.ipynb - contains the preprocessing steps taken to refine the test datasets. 

Testing Model_1.ipynb - Jupyter notebook that contains the tested results for the 3 datasets of choice after the data has been preprocessed 

Testing_Model_2.ipynb - Jupyter notebook that contains the tested results for the 3 datasets with Model-2 

GR_fine_model_Model_1.ipynb- Jupyter notebook with Model-1 being finetuned with the Gab_reddit dataset from https://data.mendeley.com/datasets/9sxpkmm8xn/1 (Mody et al (2023))

Test datasets - file containing the preprocessed test datasets used. 
- gab_again2.csv - Gab 
- cleaned_reddit4.csv - Reddit 
- cleaned_tweets01.csv - Twitter

Disclaimer: The Models 1 and 2 have been trained on a dataset with 726,120 samples. Thus, the saved dictionaries of fine-tuned models are of sizes ranging from 300-520 MB. 

Each notebook has a different name for the model class to ensure that the model architecture and parameters remain same while loading the model state dict. Any changes to the model’s architecture can cause issues.
