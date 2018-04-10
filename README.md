# mykaggle

Kaggle setup for dummies


Steps to participate in kaggle competitions:

Stage 1:
1. Set up kaggle CLI

Install kaggle-cli into your laptop by the following commmand

pip install kaggle-cli

2. create kaggle account

Create your kaggle account and kaggle specific username and password. This is different from signing in using a third party login like google.

3. Accept participation rules

- Go to kaggle.com
- login
- go the specific competition you want to participate in.
- accept competition rules
- go 

4. download data
- go to kaggle competition's data page. you will find competition name in the api command
- next go to terminal
- change to the folder you want to download data in using 'cd <insert folder name>'
- download data using the command

kg download -u <insert username> -p <insert password> -c <insert competition name exactly as copied earlier>

5. You are all set for the next stage

Stage 2:

1. Set up your data in terms of training set, validation set
- unzip your data
- divide your data into training and validation

2. build your ML model
- choose algorithm
- run algorithm
- validate your algorithm using validation dataset

Stage 3:

1. Once you have a model you want to submit, score the test dataset(which you kept in the test folder) using your model. 
2. create the submission dataset in the format provided by kaggle. You will find this submission format in a csv file accompanying your data. you can also check this in the data tab of the kaggle competition
3. Submit to kaggle. You can do this in two ways:
  1. upload to website: if you have a copy of the csv file with the final scores in your desktop/laptop you can go to competition page in the kaggle website and upload the file
  2. from kaggle cli:
    - change to directory where your submission file is using the terminal
    - type the following from the terminal
    kg submit <insert submission fil name> -u <insert username> -p <insert password> -c <insert competition name> -m "<insert any message inside quotes>"
    




