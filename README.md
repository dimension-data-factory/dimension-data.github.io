# 一. Japan export data Summary

* data source: [&darr;&darr;Japan Customs->serch entrance](https://www.customs.go.jp/toukei/srch/indexe.htm?M=05&P=0)
* date range: [1988~latest]
* types: import and export
* other related data: [&darr;&darr;Download-country codes](./japan_io/country_code_list.csv), [&darr;&darr;Download-customes_branch_code](./japan_io/custom_branch_code_name.csv)


# 二. field description

|field name|description|example| other |
|:---|:---|:---|:---|
|type | import or export | enum: `import`, `export` |  |
|hs_code | 6-digits hscode. | `090210`, `010614` |  |
| url_for_verify | static url, to verify data | as shown in the json bellow|  |
|mark|to distinguish page types|enum : `Result of Search`, `No Result`, `Unpublished`||
|COUNTRY|target country|`110 VIETNAM`||
|UNIT1||||
|UNIT2||`KG`||
|QUANTITY1_CURRENT_MONTH||375||
|QUANTITY2_CURRENT_MONTH||1373||
|VALUE_CURRENT_MONTH||||
|QUANTITY1_CUMULATIVE_YEAR_TO_DATE||||
|QUANTITY2_CUMULATIVE_YEAR_TO_DATE||375||
|VALUE_CUMULATIVE_YEAR_TO_DATE||1373||
|idx_start|num of search result records shown in page <br>`Indicate 1 to 51 case ( 1 / 1 pages) in the results of retrieval 51 cases`|||
|idx_end|same as above|||
|page_start|same as above|||
|page_end|same as above|||
|idx_total|same as above|||

> **json example**
>
>>
```
{
    "type": "export",
    "hscode": "090210",
    "url_for_verify": "https://www.customs.go.jp/toukei/srch/indexe.htm?M=05&P=1,1,,,,,,,,1,0,2024,0,1,0,2,090210,,,,,,,,,,1,,,,,,,,,,,1,1,,,,,,,,,,200",
    "mark": "Result of Search",
    "COUNTRY": "110 VIETNAM",
    "UNIT1": " ",
    "UNIT2": "KG",
    "QUANTITY1_CURRENT_MONTH": " ",
    "QUANTITY2_CURRENT_MONTH": "375",
    "VALUE_CURRENT_MONTH": "1373",
    "QUANTITY1_CUMULATIVE_YEAR_TO_DATE": " ",
    "QUANTITY2_CUMULATIVE_YEAR_TO_DATE": "375",
    "VALUE_CUMULATIVE_YEAR_TO_DATE": "1373",
    "idx_start": "1",
    "idx_end": "51",
    "page_start": "1",
    "page_end": "1",
    "idx_total": "51"
}
```

# 三. Download examples

[&darr;&darr;japan customs export examples](./japan_io/export_example_010614_090210.csv)

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




# 四.contact

1. email: [dimension_data@163.com](mailto:dimension_data@163.com)
2. WeChat:<br>
<img src="./imgs/wechat.jpeg" width=30%/>
