os.rename

```
import os

files = os.listdir('/Users/liusheng/3-情商课/歪歪兔父母学院：情商教育篇')

for filename in files:
    newname = filename.replace('【.mp3','.mp3',-1)
    os.rename(filename,newname)
    print (newname)
```