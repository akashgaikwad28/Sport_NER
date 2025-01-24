# ner-sports-task

## Problem statement

The objective of this task is to build an NLP model that can extract specific pieces of information from sports certificates. Thye information needed to be extracted includes - 
1. Participent name
2. Winning position
3. Sports name
4. Year of organization

The task is to develop a model that can read and extract these pieces of information from the set of certificates. The model should also be adaptable to new certificates that means, if given a new type of certificate, model should be able to learn from it and then accurately extract the relevant information.

## Solution proposed

Since this is a task of Named Entity Recognition, 2 models have been used. To extract a person name, pre-trained BERT model has been used. To extract the Winning position, sports name and year of organization, spacy model has been used. 

## Dataset used
The dataset has been provided with 300 certificates. The data has been manually extracted and is intended for training purposes.

## Teck stack used
1. Python 
2. FastAPI
3. Deep learning
4. Natural language processing
5. BERT model
6. Spacy model

## How to run

Step 1. Cloning the repository
```
git clone https://github.com/saikumar0605/ner-sports-certificate
```

Step 2. Create conda environment
```bash
conda create -p env python==3.9 -y
```

Step 3. Install necessary requirements
```bash
pip install -r requirements.txt
```

Step 4. Rub the app.py file for training the model
```bash
python app.py
```

Step 5. For inferencing run the prediction.py file. 
```bash
python prediction.py
```
