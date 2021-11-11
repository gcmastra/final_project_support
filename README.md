# data_final_project - 20211106
Copy of README that was stored in other team repository. I deleted it from the branch on the other repo to prevent it from wiping out the main README

## Christopher Mastrangelo
First feature branch- week one - data download and ETL in prep for exploratory data analysis stage

Some observations
 - In the future we might want to name branches after features instead of our names
 - I created my own /Resources folder to contain the CSV file(s) - one file so far for this first commit
 - When we merge the branches back into main we are going to have more than one folder with CSV files - we will need to decide on what to do about that
 - When I merge this branch with main, will my README file replace the other README or will they be merged/appended somehow? I guess we will find out 

### Steps so far - as of Saturday 11.6.2021

Here is a section of the dataframe created from importing the CSV file "Basic_stats.csv" from Kaggle NFL data.
This is just a table of player information which we might not need for the Machine Learning but could be a layer in one of the visualizations later.
![image](https://user-images.githubusercontent.com/86205000/140647104-caf87d59-5b48-498a-b429-be920fb38933.png)

I used this file because it was the first on the list on Kaggle.  Using it as an intial test to import, ETL, then upload to PostGres.
Example of ETL will be to drop columns with null values like age or high school.  Some columns may not be needed like birthday or age.
Example of where this could be used in dashboard is if we have a visualization with actual players, we can use this to display names.
The player_ID column might be useful if we do any additional webscraping from the same NFL source data.

The Jupyter Notebook file saved in this repo contains the steps used to perform the ETL.  Please refer to this file:
https://github.com/gcmastra/final_project_support/blob/82b4a0e1870cf23f5ddce49ad21fcfaf2ec5b65d/NFL_ETL_practice2.ipynb
<br>Actually this is NOT the most recent version of the notebook.  There is a newer version that has all the steps in the ETL for this file.  I will locate that and paste it in as soon as I find it.

Initially I will do all the steps using one file to get all the pieces working.  For 2nd and subsequent files the process should go faster and more smoothly.

### AWS RDS used to create PostGres 12-8-1 instance 

After the instance was created on AWS, this is what it looked like after I created a new table using the cleaned CSV file from the previous step 

![image](https://github.com/gcmastra/final_project_support/blob/82b4a0e1870cf23f5ddce49ad21fcfaf2ec5b65d/img1_to_submit.JPG)




