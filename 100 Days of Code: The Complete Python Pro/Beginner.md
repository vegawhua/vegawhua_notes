## Running Operation
- Debug


## Function
- `print()`
- `input()`
- `len()`
- `type()` - data type check
- Format
  - Omit 0 - **round()**  
    `round(formula, round num to x decimal places)` - e.g. `round(8 / 3, 2)` = 2.67
  - Reserve 0 - **.format()**  
    `"{target format}".format(value)` - e.g. `sum = "{:.2f}".format(sum)`
  - .lower() / .upper() - e.g. ex3.5
  - .count("a") - count the string elements - e.g. ex3.5

## Data Variable
- **Naming Rules** - made your code readable

## Primitive原始的 Data Type
- `String` - A string of characters
- `Integer` - whole numbers without decimal
- `Float` - nums have decimal places
- `Boolean` - True or False
### Manipulation
- **String**  
  Subscript下标 - `'Hello'[0]` = 'H'
- **Data type convertion**(type casting)  数据类型强制转换  
  `str(num)` OR `float(str)`
- **Mathematical Operation**
  - **Arithmetic Operators** 算术  
    `+` `-` `*` `/` `**` `//` `%`-取模
    floor division 整除 - e.g. `8 // 3` = 2
  - **Assignment Operators** 赋值  
    `=` `+=` `-=` `*=` `/=` `%=` `//=` `**=` `&=` `|=` `^=` `>>=` `<<=`
  - **Comparison Operators** 比较
    `>` `<` `>=` `<=` `==` `!=`
  - **Logical Operators** 逻辑
    `and` `or` `not`
  - Have a certain level of priority:  
    PEMDAS - Parenthese `()` | Exponents指数 `**` | Multiplication `*` Division `/` | Addition `+` Subtraction `-`
- **Output format**
  - f-String - no need to do type casting  
    ```
    score = 0  
    height = 1.8  
    isWinning = True   
    print(f"your score is {score}, your height is {height}, you are winning is {is Winning}.")
    ```
    Result:
    ```
    your score is 0, your height is 1.8, you are winning is True.
    ```

## Conditional Statement
- if/else Statement
  - elif
  - nested if/else statement 嵌套
  - multiple if/else 多重 - check multiple conditions



### Warning 
String should not be concatenated with int, I always forget to transform the data type.

## Dict
- `\`
\* "escape" character, `\n` - new line, `\t` - tab, `\r` - enter
- **Definition**
  - modulo 模除
  - remainder 余数
  - syntax highlight 句法高亮
  - indent 空格
  - indentation level 缩进级别

## Recommend Tool
- Thonny: good tool for python beginner, demonstrate how the computer run every step.
