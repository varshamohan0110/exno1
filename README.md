# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output

```
import pandas as pd
data=pd.read_csv('sampleids.csv')
data
```

# output

<img width="892" height="705" alt="image" src="https://github.com/user-attachments/assets/cf26a0c4-1ead-4db6-84dd-0d7340060264" />




```
data.info()

```


# output

<img width="412" height="410" alt="image" src="https://github.com/user-attachments/assets/31465220-d246-4262-916b-810b17a243f1" />



```
data.describe()
```


# output

<img width="822" height="287" alt="image" src="https://github.com/user-attachments/assets/8a0bdcdf-6971-4138-bb04-0600648f7584" />




```
data.isnull()
```



# output

<img width="772" height="703" alt="image" src="https://github.com/user-attachments/assets/e1ebae8c-78fb-4061-9f75-52f44494429f" />



```
data.isnull().sum()
```


# output

<img width="150" height="291" alt="image" src="https://github.com/user-attachments/assets/00bacf2f-61b4-4ab7-baf0-4fe80628db1e" />



```
data.notnull()
```



# output

<img width="759" height="711" alt="image" src="https://github.com/user-attachments/assets/99836c28-3e1a-44f7-b611-bf82ee7646ab" />



```
data.notnull().sum()
```


# output

<img width="137" height="285" alt="image" src="https://github.com/user-attachments/assets/d354be8e-12ae-4ba6-bd04-47ce29df9bba" />



```
data.dropna()
```


# output

<img width="890" height="454" alt="image" src="https://github.com/user-attachments/assets/b97b5715-86db-4654-b7e2-f63ea4c19dcc" />



```
data.dropna(axis=1)
```



# output

<img width="894" height="445" alt="image" src="https://github.com/user-attachments/assets/fc1f2c4e-27b3-402e-a13b-100a429c6639" />




```
data.dropna(axis=0)
```



# output

<img width="889" height="457" alt="image" src="https://github.com/user-attachments/assets/3da63193-d9d1-43da-abe2-831f80aeb7aa" />




```
data1.fillna('Data Science')
```



# output

<img width="1287" height="387" alt="image" src="https://github.com/user-attachments/assets/6c739595-131b-48bb-95b1-9bf83e45adad" />



```
data1.fillna(method='ffill')
```



# output

<img width="1244" height="449" alt="image" src="https://github.com/user-attachments/assets/eeb889fd-35d3-46bf-ab3c-0a97fc25cb5b" />



```
data1.fillna(method='bfill')
```



# output

<img width="1243" height="440" alt="image" src="https://github.com/user-attachments/assets/7cd48abf-a376-4993-ba5a-f5dc0bac1e4e" />



```
data1['Credit_History'].ffill()
```



# output

<img width="512" height="275" alt="image" src="https://github.com/user-attachments/assets/2d84923d-a5c4-44f5-8775-03fa01f2bd1a" />



```
data['M4'].fillna(value=data['M4'].mean())
```



# output

<img width="266" height="312" alt="image" src="https://github.com/user-attachments/assets/c39c2e5b-72ca-4779-ac14-3ddd54c1e898" />


# Result

Thus the programs are executed successfully.
