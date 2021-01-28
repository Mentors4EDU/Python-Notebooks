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
