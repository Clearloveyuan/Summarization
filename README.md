# Summarization


## How to obtain json version of XSUM dataset

1. Download dataset from the website

```
cd summarization
mkdir data
cd data
wget http://bollin.inf.ed.ac.uk/public/direct/XSUM-EMNLP18-Summary-Data-Original.tar.gz --no-check-certificate
tar -zxvf XSUM-EMNLP18-Summary-Data-Original.tar.gz
```

2. Download the label_id and seperate the dataset

```
wget https://github.com/EdinburghNLP/XSum/raw/master/XSum-Dataset/XSum-TRAINING-DEV-TEST-SPLIT-90-5-5.json 
python xsum_split.py bbc-summary-data XSum-TRAINING-DEV-TEST-SPLIT-90-5-5.json xsum
```

3. Use the dataprocess.ipynb to save the dataset in json version



