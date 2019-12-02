### :nht-child(n+1)表示周期性选择，n是计数器，从0开始，括号里面的数字从1开始；里面写0不会返回任何元素，写1正常返回第一个元素。

### 用例：隔行换色，每四行一循环换色

```
table tbody tr:nth-child(8n+1) td{
    background-color: #000;
  }
  table tbody tr:nth-child(8n+2) td{
    background-color: #000;
  }
  table tbody tr:nth-child(8n+3) td{
    background-color: #000;
  }
  table tbody tr:nth-child(8n+4) td{
    background-color: #000;
  }
```
#### 两行一循环换色 就是4n+1、4n+2
#### 三行一循环换色 就是6n+1、6n+2、6n+3
#### 四行一循环换色 就是8n+1、8n+2、8n+3、8n+4
