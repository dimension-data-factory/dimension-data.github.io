```python

```


```python
import pandas as pd
```


```python
df = pd.read_csv('./input/export_example_010614_090210.csv', dtype={'CW_HSCODE': str})
```


```python

```


```python

```


```python
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>_id</th>
      <th>CW_HSCODE</th>
      <th>url_for_verify</th>
      <th>foreign_id</th>
      <th>mark</th>
      <th>COUNTRY</th>
      <th>UNIT1</th>
      <th>UNIT2</th>
      <th>QUANTITY1_CURRENT_MONTH</th>
      <th>QUANTITY2_CURRENT_MONTH</th>
      <th>VALUE_CURRENT_MONTH</th>
      <th>QUANTITY1_CUMULATIVE_YEAR_TO_DATE</th>
      <th>QUANTITY2_CUMULATIVE_YEAR_TO_DATE</th>
      <th>VALUE_CUMULATIVE_YEAR_TO_DATE</th>
      <th>idx_start</th>
      <th>idx_end</th>
      <th>page_start</th>
      <th>page_end</th>
      <th>idx_total</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>670d21ea631a82b8a8a3089e</td>
      <td>090210</td>
      <td>https://www.customs.go.jp/toukei/srch/indexe.h...</td>
      <td>67092f6ee303cd06213c553e</td>
      <td>Result of Search</td>
      <td>(100 TOKYO)TOTAL</td>
      <td></td>
      <td>KG</td>
      <td></td>
      <td>15570.0</td>
      <td>69715.0</td>
      <td></td>
      <td>15570.0</td>
      <td>69715.0</td>
      <td>1.0</td>
      <td>51.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>51.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>670d21ea631a82b8a8a3089f</td>
      <td>090210</td>
      <td>https://www.customs.go.jp/toukei/srch/indexe.h...</td>
      <td>67092f6ee303cd06213c553e</td>
      <td>Result of Search</td>
      <td>(0902.10-100  )TOTAL</td>
      <td></td>
      <td>KG</td>
      <td></td>
      <td>9079.0</td>
      <td>41957.0</td>
      <td></td>
      <td>9079.0</td>
      <td>41957.0</td>
      <td>1.0</td>
      <td>51.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>51.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>670d21ea631a82b8a8a308a0</td>
      <td>090210</td>
      <td>https://www.customs.go.jp/toukei/srch/indexe.h...</td>
      <td>67092f6ee303cd06213c553e</td>
      <td>Result of Search</td>
      <td>105 CHINA</td>
      <td></td>
      <td>KG</td>
      <td></td>
      <td>111.0</td>
      <td>2387.0</td>
      <td></td>
      <td>111.0</td>
      <td>2387.0</td>
      <td>1.0</td>
      <td>51.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>51.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>670d21ea631a82b8a8a308a1</td>
      <td>090210</td>
      <td>https://www.customs.go.jp/toukei/srch/indexe.h...</td>
      <td>67092f6ee303cd06213c553e</td>
      <td>Result of Search</td>
      <td>106 TAIWAN</td>
      <td></td>
      <td>KG</td>
      <td></td>
      <td>1000.0</td>
      <td>1780.0</td>
      <td></td>
      <td>1000.0</td>
      <td>1780.0</td>
      <td>1.0</td>
      <td>51.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>51.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>670d21ea631a82b8a8a308a2</td>
      <td>090210</td>
      <td>https://www.customs.go.jp/toukei/srch/indexe.h...</td>
      <td>67092f6ee303cd06213c553e</td>
      <td>Result of Search</td>
      <td>108 HG KONG</td>
      <td></td>
      <td>KG</td>
      <td></td>
      <td>1968.0</td>
      <td>13212.0</td>
      <td></td>
      <td>1968.0</td>
      <td>13212.0</td>
      <td>1.0</td>
      <td>51.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>51.0</td>
    </tr>
  </tbody>
</table>
</div>




```python

```

[数据样例](./input/exec)


```python

```
