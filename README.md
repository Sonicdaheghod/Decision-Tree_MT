# Decision Tree- Body Performance Dataset
<img width="487" alt="image" src="https://github.com/Sonicdaheghod/Decision-Tree_MT/assets/68253811/89bcec8b-f544-47f6-988f-47c7340fe6ed">

By: Megan Tran
## Table of Contents
* [Purpose of Program](#Purpose-of-program)
* [Technologies](#technologies)
* [Setup](#setup)
* [Using the Program](#using-the-program)
* [Acknowledgements](#acknowledgements)
  
## Purpose of Program
This program was created to understand the basics behind the Decision Tree algorithm for data classificaiton. 

## Technologies
Languages/ Technologies used:

* Jupyter Notebook

* Python3

## Setup
Download the necessary packages:
```
pip install scikit-learn
pip install pandas
pip install matplotlib
pip install numpy
```
Check to see if version of Python/Python3 (if on jupyter Notebook) is used, this is to ensure packages work properly. Python 3.8 or better is recommended.

```
import sys
sys.version
```
## Using the Program

Use any csv dataset you like for this project. 
* use pandas to reformat the data
<img width="501" alt="image" src="https://github.com/Sonicdaheghod/Decision-Tree_MT/assets/68253811/2384a542-12b7-4e66-b321-27f0873c9392">

The Decision Tree Mode only processes numerical values, so if the dataset has strings as data points, they must be changed to numerical values. This can be done doing this:

```
#create dictionary to convert letters to numbers for respective columns in dataset
letters_to_num_bodyPerf = {
    "A" : 1,
    "B" : 2,
    "C" : 3,
    "D" : 4,
    
}

gender_to_num = {
    "F" : 0,
    "M" : 1
    
    
}

df['the_class'] = df['the_class'].map(letters_to_num_bodyPerf)
df['gender'] = df['gender'].map(gender_to_num)

#making new file for dataset to use
df.to_csv('modified_bodyPerformance.csv', index=False)
```

## Acknowledgements
* Tutorial by Misra Turp: https://youtu.be/wxS5P7yDHRA?t=581
* Data from kukuroo3: https://www.kaggle.com/datasets/kukuroo3/body-performance-data

