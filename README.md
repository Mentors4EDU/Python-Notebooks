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
