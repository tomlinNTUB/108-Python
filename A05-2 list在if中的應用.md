# A05-2 list在if中的應用



## (1) 程式範例
``` python
#-------------------------------
# 以list作為多種可接受值的判斷
#-------------------------------

# 輸入年齡
a = input('輸入年齡:')

# 年齡轉成整數
try:
    a = int(a)
except:
    print('請輸入整數')
    exit()

# 判斷
if a in [10, 13, 14, 17, 20]:
    print('年齡{}符合條件'.format(a))
else:
    print('年齡{}不符合條件'.format(a)) 
```

### 測試
``` python
輸入年齡:10
>> 年齡10符合條件

輸入年齡:30
>> 年齡30不符合條件
```


## (2) 程式範例
``` python
#-------------------------------
# 以list作為多種不可接受值的判斷
#-------------------------------

# 輸入年齡
a = input('輸入年齡:')

# 年齡轉成整數
try:
    a = int(a)
except:
    print('請輸入整數')
    exit()

# 判斷
if a not in [10, 13, 14, 17, 20]:
    print('年齡{}不在特定歲數中'.format(a))
else:
    print('年齡{}在特定歲數中'.format(a))  
```

### 測試
``` python
輸入年齡:10
>> 年齡10在特定歲數中

輸入年齡:30
>> 年齡30不在特定歲數中
```



## (3) 程式範例
``` python
# 建立一個存放多個詞的list
s = ['不僅', '不但', '不光', '不單', '不只', '不外乎', '不如', '不妨', '不盡然', '不得', '不怕']

# 進行判斷是否存在
k = '不可'

if k in s:
    print('存在"{}"這個詞'.format(k))
else:
    print('不存在"{}"這個詞'.format(k))
```

### 測試
``` python
>> 不存在"不可"這個詞
```
