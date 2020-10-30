# python 零基础上手小课程记录

- print("输出/n输出")
- 变量：```leader = "松江"```
  - 变量名一般小写
  - 字符串str：```name = "myy"```
  - 整型int：```age = 18```
  - 浮点型 float：```height = 1.57```
  - ```print("输出/n输出", end="")``` 输出不换行
  - ```print("输出/n输出     " + "2")``` 加号左右必须都是字符串，空格可以输出找齐
- 语句执行报错 IndentationError: unindent does not match any outer indentation level，原因：新的Python语法不支持代码对齐中混用TAB和空格
- 条件

  ```python
    if 8 > 6 :
      print("if 8 > 6")
      print(8 > 6)
      if 8 > 6 :
        print("嵌套")
      else :
        print("")
    elif 8 > 6:
      print("elif")
    else :
      print("else")
  ```

- 逻辑运算

  ```python
    if 8 > 6 and 8 < 9:
      print("and")
    else :
      print("")

    if 8 > 6 or 8 > 9:
      print("or")
    else :
      print("")

    if 1 != 6 not (8 > 9):
      print("not")
    else :
      print("")
  ```

- 列表：保存同一类简单的数据

  ```python
    books = ["三国演义", "红楼梦", "西游记", "水浒传"]
    print("索引")
    print(books[2])

    print("反向索引")
    print(books[-1])

    print("范围索引-左闭右开")
    print(books[1 : 4])
    print(books[1 : -2])

    print("尾部追加")
    books.append("资治通鉴")

    print("插入，参数1：索引，参数2：被插入项")
    books.insert(2,"道德经")

    print("更新数据")
    books[1] = "儒林外史"

    print("删除数据")
    books.pop(1)
  ```

- 字典

  ```python
    lisa = {"name": "lisa", "age": 12}
    print("获取")
    age = lisa["age"]
    print("新增")
    lisa["weight"] = 345
    print("删除")
    lisa.pop("name")
  ```

- 循环

  ```python
    print("不定次循环while")
    i = 1
    result = 3
    while i <= 10 :
      print(result)
      result = result * 3
      i = i + 1
    print("end")

    print("定次循环for")
    books = ["三国演义", "红楼梦", "西游记", "水浒传"]
    for book in books:
      print(book)

    print("range生成有序数据-左闭右开-[10,11,12,13,14]")
    for i in range(10,15)
      print(i)


    table = [
      [1,2,3,4,5],
      [6,7,8,8,9],
      [11,23,11,22,33]
    ]
    for col in table:
      for row in col:
        print(row)
      print("------------")
  ```

- 课程ending demo

  ```python
    movies = []
    m1 = {"year":1900,"title":"1"}
    m2 = {"year":1910,"title":"2"}
    m3 = {"year":1950,"title":"3"}
    m4 = {"year":1900,"title":"4"}
    movies.append(m1)
    movies.append(m2)
    movies.append(m3)
    movies.append(m4)
    y = 1950
    for m in movies:
      if m["year"] == y:
        print(m)
  ```

  - 接下来...
    - Python web
    - 数据库
    - 爬虫
