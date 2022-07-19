
World Billionaire Analysis in Python

```

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
import plotly.express as px
df = pd.read_csv("https://raw.githubusercontent.com/amankharwal/Website-data/master/Billionaire.csv")
df.head()
```
![image](https://user-images.githubusercontent.com/64798994/179675237-ffb237a7-d58e-44f9-8dbb-5b742081e5a0.png)

```
#Data Cleaning and transformation
df['NetWorth']=df['NetWorth'].apply(lambda x:x.strip('$'))
df['NetWorth']=df['NetWorth'].apply(lambda x:x.strip('B'))
df['NetWorth']=pd.to_numeric(df['NetWorth'])
df.head()

```
#Output
![image](https://user-images.githubusercontent.com/64798994/179676875-09ccc6dd-e33d-49e1-a4ad-386286954bc1.png)

```


```























This site was built using [GitHub Pages](https://pages.github.com/)
