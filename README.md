# Ex03-Univariate-Analysis
#Code
import pandas as pd
df=pd.read_csv("/content/SuperStore.csv")
df.head()
![Screenshot (51)](https://user-images.githubusercontent.com/96919035/228148500-8b82aed5-0701-48f4-87b0-696031b3cea7.png)

df.info()
![Screenshot (52)](https://user-images.githubusercontent.com/96919035/228148620-94f312cf-2778-4be7-b026-bf2af6280368.png)

df.dtypes
![Screenshot (53)](https://user-images.githubusercontent.com/96919035/228148689-d6327416-2859-42eb-b45c-4216d9290783.png)

df['Postal Code'].value_counts()
df['Sales'].value_counts()
![Screenshot (54)](https://user-images.githubusercontent.com/96919035/228148768-1aa5cd31-45db-4074-8d17-0d340df80fd5.png)

df.describe()
![Screenshot (55)](https://user-images.githubusercontent.com/96919035/228148900-8888dfca-70dc-4606-8ae6-925e5d20769a.png)

import seaborn as sns
sns.boxplot(x="Postal Code" , data=df)
![Screenshot (56)](https://user-images.githubusercontent.com/96919035/228148974-9fc1f003-eee1-4506-ad63-3f4c5a8b7348.png)

import seaborn as sns
sns.boxplot(x="Sales" , data=df)
![Screenshot (57)](https://user-images.githubusercontent.com/96919035/228149082-ae61140f-5524-4a9d-8e36-c7ae00aafe7f.png)

sns.countplot(x="Postal Code",data=df)
![Screenshot (58)](https://user-images.githubusercontent.com/96919035/228149160-7fbc039d-0e0d-4e4e-93dc-5c392036603e.png)

sns.distplot(df["Postal Code"])
![Screenshot (59)](https://user-images.githubusercontent.com/96919035/228149252-8c57c673-953d-4d1b-9513-634b08e3254e.png)

sns.distplot(df["Sales"])
![Screenshot (60)](https://user-images.githubusercontent.com/96919035/228149337-56c66cad-e571-4f6e-8c17-368f8b2374b4.png)
