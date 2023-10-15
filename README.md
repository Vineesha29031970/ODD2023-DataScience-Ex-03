# Ex-03 Univariate Analysis

# AIM:

To read the given data and perform the univariate analysis with different types of plots.

# EXPLAINATION:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# ALGORITHM:

Step1:
Read the given data set using standard libraries.

Step2:
Get the information about the data.

Step3:
Remove the null values from the data.

Step4:
Mention the datatypes from the data.

Step5:
Count the values from the data.

Step6:
Do plots like sepallength,species,sepalwidth.

# PROGRAM:

# Superstore CSV File:

```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```

# Diabetes CSV File:
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```

# Employee Salary CSV File:
```

import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```

# Output:
# Superstore Output:

<img width="549" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/d63b77d4-c320-44ff-9a4e-8cb2e3d21b7e">


<img width="567" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/9d6656cd-0934-4d4c-8d60-13d5e5a23df5">


<img width="575" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/d61d208c-3729-4036-8d15-92efba5a783e">


<img width="557" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/02fba1d7-a23a-41a6-a72f-53c3f2e1bf79">


<img width="481" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/96c63dfd-ac8f-4e45-acbb-c73871335cf0">


# Diabetes Output:

<img width="575" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/b5105453-d787-4f34-ba8b-6b31a0931f14">


<img width="568" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/1753b767-b01d-4488-8136-ff2e2899e85f">


<img width="574" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/e4234e29-c01d-417f-b93a-bbf1a27e7d21">


<img width="560" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/296d1c0e-6abb-49f8-bfbc-a2a625a9ff70">


<img width="523" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/8304689a-3a11-4e42-90d3-e4866d59efb4">


<img width="526" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/00cbe473-546e-4bcb-855b-f7ba978fbd72">


<img width="457" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/2894b741-b3d9-48b1-b3a5-c73123097d18">


# Employee Salary Output:

<img width="518" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/657fe022-7064-470a-b056-0d9ee29a5799">


<img width="548" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/45916983-3e6f-429d-9f09-757bc590b8df">


<img width="469" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/8bf37689-a504-4f76-8d6d-d93811a58fa6">


<img width="614" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/9edaa1cf-e948-4b51-95fa-e7aff1ddba5a">


<img width="405" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/c8692c67-10b0-4582-8650-9f80cf3c4f31">


<img width="593" alt="image" src="https://github.com/Vineesha29031970/ODD2023-DataScience-Ex-03/assets/133136880/95ca0a6c-d067-470d-b6ef-21f354878383">


# Result:

Hence the given CSV File was verified successfully with the help of the Univariate Analysis technique.
