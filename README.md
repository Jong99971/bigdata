데이터 정제 코드

import pandas as pd

df = pd.read_csv('/content/예적금.csv')
print(df.columns)
column_1 = '기본'
column_2 = '최고'

filtered_df = df[df[column_2] > df[column_1]]

print(filtered_df)

데이터 시각화 코드

import pandas as pd
import seaborn as sns

df=pd.read_csv('/content/예적금.csv')
print(df)
sns.lineplot(data=df,x='basic',y='max')
