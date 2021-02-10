<p align="center">
  <a href="https://github.com/Mentors4EDU">
    <img src="https://miro.medium.com/max/1024/0*4ty0Adbdg4dsVBo3.png" width="320" alt="Hello World">
  </a>
</p>

<p align="center">
This is a repo for some past practice IPython notebooks, projects, portfolio work and assignments
</p>

### Commands:

**Import:**
```python
import pandas as pd
```

**Reading a CSV:**
```python
df  = pd.read_csv("Directory/File.csv")
```
**Printing:** 
```python 
print(df)
```

**Import an Image:**
```python
from IPython.display import Image
Image(filename='/home/user/directory/imagename.png')
```

**Yes/No Columns:**
```python
filename_df['EXAMPLE'] = [1 if e == 'Yes' else 0 for e in filename_df['EXAMPLE']]
```
**Data Frames:**
```python
df = pd.DataFrame([(.2, .3), (.0, .6), (.6, .0), (.2, .1)],
columns=['yes', 'no'])
```
**Categories w/ Print:**
```python
df_Category = pd.get_dummies(df['Category'])
df_Example = pd.get_dummies(df['Example'])
df_concat = pd.concat([df, df_Category, df_Example], axis=1)
print (df_concat.head())
```
**Set Font**
```python
plt.rc("font", size=8)
```
**Set Style:**
```python
sns.set(style="white")
sns.set(style="whitegrid", color_codes=True)
```
**Data Unique:**
```python
data['Category'].unique
```
**X/Y Predict**
```python
y_true = [df]
y_pred = [df.unique]
confusion_matrix(y_true, y_pred)
```
**Confusion Matrix:**
```python
confusion_matrix(y_true, y_pred)
```
**Density Plot:**
```python
df.plot()
df.plot(kind='density')
```
**Search Missing Values:**
```python
df = pd.read_csv('Downloads/ExampleFile.csv', dtype=str)
missing_values = ["n/a", "na", "--"]
df = pd.read_csv("Downloads/ExampleFile.csv", na_values = missing_values)
print(df['Example'])
```
**Data Type Object:**
```python
d = {'col1': [1, 2], 'col2': [3, 4]}
df = pd.DataFrame(data=d)
df.dtypes
dtype: object
```
**Calculate Mean:**
```python
def calculate_mean(n):
    s = sum("example")
    N = len(n)
    mean = s / N
    return mean
print(mean)
```
**Group by Mean:**  
*Source: https://datatofish.com/use-pandas-to-calculate-stats-from-an-imported-csv-file/*
```python
groupby_mean1 = df.groupby(['Sample1']).mean() 
groupby_count1 = df.groupby(['Sample1']).count()
groupby_mean2 = df.groupby(['Sample2']).mean() 
groupby_count2 = df.groupby(['Sample2']).count()
print ('Sum of values, grouped by sample1: ' + str(groupby_mean1))
print ('Sum of values, grouped by sample2: ' + str(groupby_mean2))
```
**Data:**
```python
data= d['Example']
```
**Scatter Plots:**
```python
plt.scatter(data, example, edgecolors='r')
```
**Plot Labels:**
```python
plt.xlabel('Label1')
plt.ylabel('Label2')
plt.title('TitleExample')
plt.show()
```
**Data Frame (Drop):**
```
df = df.drop(columns=['SAMPLE1', 'SAMPLE2'])
```
**Print Head:**
```
print (df.head())
```
