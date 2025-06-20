# kotlin(感谢https://www.w3schools.com/)

## Kotlin 是什么？

Kotlin 是一种现代、流行的编程语言，由 JetBrains 于 2016 年发布。

[由于它与Java](https://www.w3schools.com/java/default.asp)（最流行的编程语言之一）兼容，因此变得非常流行，这意味着 Java 代码（和库）可以在 Kotlin 程序中使用。

Kotlin 用于：

- 移动应用程序（特别是 Android 应用程序）
- Web 开发
- 服务器端应用程序
- 数据科学
- 还有更多！

------

## 为什么要使用 Kotlin？

- Kotlin 与 Java 完全兼容

- Kotlin 可在不同的平台上运行（Windows、Mac、Linux、Raspberry Pi 等）

- Kotlin 简洁且安全

- Kotlin 很容易学习，特别是如果你已经了解 Java

- Kotlin 是免费使用的

- 庞大的社区/支持

## otlin IDE

  开始使用 Kotlin 最简单的方法是使用 IDE。

  IDE（集成开发环境）用于编辑和编译代码。

  在本章中，我们将使用 IntelliJ（由创建 Kotlin 的同一批人开发），可以从<https://www.jetbrains.com/idea/download/>免费下载。

------

## Kotlin 安装

  下载并安装 IntelliJ 后，单击 **“新建项目”**按钮即可开始使用 IntelliJ：

  然后点击左侧菜单中的“Kotlin”，并输入项目名称：

  接下来，我们需要安装 JDK（Java 开发工具包）来启动并运行我们的 Kotlin 项目。点击“项目 JDK”菜单，选择“下载 JDK”，然后选择版本和供应商（例如 AdoptOpenJDK 11），然后点击“下载”按钮：

  下载并安装 JDK 后，从选择菜单中选择它，然后单击“下一步”按钮，最后单击“完成”：

  现在我们可以开始构建 Kotlin 项目了。不必担心 IntelliJ 中各种按钮和功能。现在，只需打开 src（源）文件夹，然后按照下图所示的步骤创建一个 kotlin 文件：

  选择“文件”选项并为您的 Kotlin 文件添加一个名称，例如“Main”：

  现在，您已经创建了第一个 Kotlin 文件 (Main.kt)。让我们在其中添加一些 Kotlin 代码，然后运行程序来查看其运行情况。在 Main.kt 文件中，添加以下代码：

  Main.kt

  ```
  fun main() {
    println("Hello World")
  }
  ```

  如果您不理解上面的代码，也不用担心——我们将在后面的章节中详细讨论。现在，我们先来关注如何运行代码。点击顶部导航栏上的“运行”按钮，然后点击“运行”，并选择“Mainkt”。

  接下来，IntelliJ 将构建你的项目，并运行 Kotlin 文件。输出将如下所示：

  如您所见，代码的输出是“Hello World”，这意味着您现在已经编写并执行了您的第一个 Kotlin 程序！

------

  ## 在 W3Schools 学习 Kotlin

  在 w3schools.com 学习 Kotlin 时，您可以使用我们的“亲自尝试”工具，该工具会同时显示代码和结果。这将帮助您在后续学习中更轻松地理解每个部分：

  ### Main.kt

  代码：

  ```
  fun main() {
    println("Hello World")
  }
  ```

  结果：

  `Hello World`

  ## Kotlin 语法

  在上一章中，我们创建了一个名为的 Kotlin 文件`Main.kt`，并使用以下代码将“Hello World”打印到屏幕上：

  ### 例子

  ```
  fun main() {
    println("Hello World")
  }
  ```

   

  ### 示例解释

  关键字`fun`用于声明函数。函数是用于执行特定任务的代码块。在上面的例子中，它声明了`main()`函数。

  函数`main()`是每个 Kotlin 程序中都会看到的东西。它用于**执行**`main()`代码。函数花括号内的任何代码都`{}`将被**执行**。

  例如，`println()`函数位于`main()`函数内部，这意味着它将被执行。该`println()`函数用于输出/打印文本，在我们的示例中，它将输出“Hello World”。

  **需要了解：**在 Kotlin 中，代码语句不必以分号 ( `;`) 结尾（其他编程语言通常需要分号，例如[Java](https://www.w3schools.com/java/default.asp)、[C++](https://www.w3schools.com/cpp/default.asp)、[C#](https://www.w3schools.com/cs/default.asp)等）。

------

  ## 主要参数

  在 Kotlin 1.3 版本之前，需要使用`main()`带参数的函数，例如：`fun main(args : Array<String>)`。上面的示例必须像这样写才能正常工作：

  ### 例子

  ```
  fun main(args : Array<String>) {
    println("Hello World")

  ```

  ## Kotlin 输出（打印）

  该`println()`函数用于输出值/打印文本：

  ### 例子

  ```
  fun main() {
    println("Hello World")
  }
  ```

   

  你可以添加任意数量的`println()`函数。注意，每个函数都会添加一行：

  ### 例子

  ```
  fun main() {
    println("Hello World!")
    println("I am learning Kotlin.")
    println("It is awesome!")
  }
  ```

   

  您还可以打印数字并执行数学计算：

  ### 例子

  ```
  fun main() {
    println(3 + 3)
  }
  ```

   

------

  ## print() 函数

  还有一个`print()`函数，与 类似`println()`。唯一的区别是，它不会在输出末尾插入新行：

  ### 例子

  ```
  fun main() {
    print("Hello World! ")
    print("I am learning Kotlin. ")
    print("It is awesome!")
  }
  ```

  Kotlin 评论

注释可用于解释 Kotlin 代码，使其更具可读性。它还可用于在测试替代代码时阻止执行。

------

## 单行注释

单行注释以两个正斜杠 ( `//`) 开头。

Kotlin 会忽略该行和行尾之间的任何文本`//`（不会执行）。

此示例在代码行前使用单行注释：

### 例子

```
// This is a comment
println("Hello World") 
```

 

此示例在代码行末尾使用单行注释：

### 例子

```
println("Hello World")  // This is a comment
```

 

------

## 多行注释

多行注释以 开始`/*`并以 结束`*/`。

`/*`和之间的任何文本都`*/`将被 Kotlin 忽略。

此示例使用多行注释（注释块）来解释代码：

### 例子

```
/* The code below will print the words Hello World
to the screen, and it is amazing */
println("Hello World")  
```

 Kotlin 变量

变量是存储数据值的容器。

要创建变量，请使用`var`或`val`，并使用等号 ( ) 为其赋值`=`：

### 句法

```
var variableName = value
val variableName = value
```

### 例子

```
var name = "John"
val birthyear = 1975

println(name)          // Print the value of name
println(birthyear)     // Print the value of birthyear
```

 

`var`和之间的区别`val`在于，用`var`关键字 声明的变量**可以被更改/修改**，而`val`变量 **不能**。

------

## 变量类型

与许多其他编程语言不同，Kotlin 中的变量不需要用指定的 *类型*声明（例如，如果您熟悉的话，可以用“String”表示文本，用“Int”表示数字）。

要在 Kotlin 中创建一个存储文本的变量和另一个存储数字的变量，请看以下示例：

### 例子

```
var name = "John"      // String (text)
val birthyear = 1975   // Int (number)

println(name)          // Print the value of name
println(birthyear)     // Print the value of birthyear
```

 

Kotlin 足够聪明，能够理解**“John”**是一个`String`（文本），而**1975**是一个`Int` （数字）变量。

但是，如果您坚持的话，可以指定类型：

### 例子

```
var name: String = "John" // String
val birthyear: Int = 1975 // Int

println(name)
println(birthyear)
```

 

你也可以声明一个变量而不赋值，稍后再赋值。**但是**，这只有在指定类型时才可行：

### 例子

这很好用：

```
var name: String
name = "John"
println(name)
```

 

### 例子

这将产生一个错误：

```
var name
name = "John"
println(name)
```

## Kotlin 数据类型

在 Kotlin 中，变量的*类型由其值决定：*

### 例子

```
val myNum = 5             // Int
val myDoubleNum = 5.99    // Double
val myLetter = 'D'        // Char
val myBoolean = true      // Boolean
val myText = "Hello"      // String
```

 

但是，您从上一章了解到，如果需要，可以指定类型：

### 例子

```
val myNum: Int = 5                // Int
val myDoubleNum: Double = 5.99    // Double
val myLetter: Char = 'D'          // Char
val myBoolean: Boolean = true     // Boolean
val myText: String = "Hello"      // String
```

 

有时你必须指定类型，但通常不需要。无论如何，了解不同类型代表什么总是有益的。

稍后您将了解更多有关**何时需要**指定类型的信息。

数据类型分为不同的组：

- 数字
- 人物
- 布尔值
- 字符串
- 数组

------

## 数字

数字类型分为两类：

**整数类型**存储整数，无论正数还是负数（例如 123 或 -456），不包含小数。有效类型 为`Byte`、` Short`和。`Int``Long`

**浮点类型**表示带有小数部分的数字，包含一个或多个小数。有两种类型：` Float`和`Double`。

如果没有指定数字变量的类型，则通常会返回`Int`整数和`Double`浮点数。

------

## 整数类型

### 字节

该`Byte`数据类型可以存储从 -128 到 127 的整数。`Int`当您确定值在 -128 和 127 之间时，可以使用它来代替或其他整数类型以节省内存：

### 例子

```
val myNum: Byte = 100
println(myNum)
```

 

### 短的

该`Short`数据类型可以存储从 -32768 到 32767 的整数：

### 例子

```
val myNum: Short = 5000
println(myNum)
```

 

### 整数

该`Int`数据类型可以存储从 -2147483648 到 2147483647 的整数：

### 例子

```
val myNum: Int = 100000
println(myNum)
```

 

### 长的

该`Long`数据类型可以存储从 -9223372036854775808 到 9223372036854775807 的整数。当 `Int`数值不够大时使用。您也可以选择以“L”结尾：

### 例子

```
val myNum: Long = 15000000000L
println(myNum)
```

 

------

## Int 和 Long 之间的区别

整数是`Int`不超过 2147483647 的数字。如果超出此范围，则定义为`Long`：

### 例子

```
val myNum1 = 2147483647  // Int
val myNum2 = 2147483648  // Long
```

------

------

## 浮点类型

浮点类型表示带有小数的数字，例如 9.99 或 3.14515。

和数据类型`Float`可以`Double`存储小数：

### 浮点示例

```
val myNum: Float = 5.75F
println(myNum)
```

 

### 双重示例

```
val myNum: Double = 19.99
println(myNum)
```

 

使用`Float`或`Double`？

浮点值的精度表示小数点后可以保留多少位数字。浮点值的精度只有六到七位小数，而变量的精度大约为 15 位。因此，对于大多数计算来说，使用浮点数更为**安全**。`Float``Double``Double`

还要注意，类型的值应该`Float`以“F”结尾。

### 科学数字

浮点数也可以是用“e”或“E”表示10的幂的科学数：

### 例子

```
val myNum1: Float = 35E3F
val myNum2: Double = 12E4
println(myNum1)
println(myNum2)
```

 

------

## 布尔值

数据`Boolean`类型只能采用以下值`true`或`false`：

### 例子

```
val isKotlinFun: Boolean = true
val isFishTasty: Boolean = false
println(isKotlinFun)   // Outputs true
println(isFishTasty)   // Outputs false 
```

 

布尔值主要用于条件测试，您将在后面的章节中了解更多相关内容。

------

## 字符

该`Char`数据类型用于存储 **单个**字符。char 值必须用**单**引号括起来，例如 'A' 或 'c'：

### 例子

```
val myGrade: Char = 'B'
println(myGrade)
```

 

与 Java 不同，您无法使用 ASCII 值来显示某些字符。值 66 在 Java 中会输出“B”，但在 Kotlin 中会引发错误：

### 例子

```
val myLetter: Char = 66
println(myLetter) // Error
```

------

## 字符串

该`String`数据类型用于存储字符序列（文本）。字符串值必须用 **双**引号括起来：

### 例子

```
val myText: String = "Hello World"
println(myText)
```

 

您将在[字符串章节](https://www.w3schools.com/kotlin/kotlin_strings.php)中了解有关字符串的更多信息。

------

## 数组

数组用于在单个变量中存储多个值，而不是为每个值声明单独的变量。

您将在[数组章节](https://www.w3schools.com/kotlin/kotlin_arrays.php)中了解有关数组的更多信息。

------

## 类型转换

类型转换是将一种数据类型的值转换为另一种类型。

[在 Kotlin 中，数字类型的转换与Java](https://www.w3schools.com/java/default.asp)不同。例如，无法使用以下代码将一个`Int`类型转换为另一个类型：`Long`

### 例子

```
val x: Int = 5
val y: Long = x
println(y) // Error: Type mismatch 
```

 

要将数字数据类型转换为另一种类型，必须使用以下函数之一：`toByte()`，，，，，或：`toShort()``toInt()``toLong()``toFloat()``toDouble()``toChar()`

### 例子

```
val x: Int = 5
val y: Long = x.toLong()
println(y)
```

## Kotlin 运算符

运算符用于对变量和值执行运算。

该值称为操作数，而操作（在两个操作数之间执行）由**运算符**定义：

| 操作数 | 操作员 | 操作数 |
| ------ | ------ | ------ |
| 100    | +      | 50     |

在下面的例子中，数字 100 和 50 是**操作数**， `+`符号是**运算符**：

### 例子

```
var x = 100 + 50
```



尽管该`+`运算符通常用于将两个值相加（如上例所示），但它也可以用于将变量与值或变量与变量相加：

### 例子

```
var sum1 = 100 + 50       // 150 (100 + 50)
var sum2 = sum1 + 250     // 400 (150 + 250)
var sum3 = sum2 + sum2    // 800 (400 + 400)
```



Kotlin 将运算符分为以下几类：

- 算术运算符
- 赋值运算符
- 比较运算符
- 逻辑运算符

------

## 算术运算符

算术运算符用于执行常见的数学运算。

| Operator | Name           | Description                      | Example | Try it                                                       |
| -------- | -------------- | -------------------------------- | ------- | ------------------------------------------------------------ |
| +        | Addition       | Adds together two values         | x + y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_add) |
| -        | Subtraction    | Subtracts one value from another | x - y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_sub) |
| *        | Multiplication | Multiplies two values            | x * y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_mult) |
| /        | Division       | Divides one value from another   | x / y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_div) |
| %        | Modulus        | Returns the division remainder   | x % y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_mod) |
| ++       | Increment      | Increases the value by 1         | ++x     | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_inc) |
| --       | Decrement      | Decreases the value by 1         | --x     | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_dec) |

------

------

## Kotlin 赋值运算符

赋值运算符用于为变量赋值。

在下面的例子中，我们使用**赋值运算**符（`=`）将值**10赋给名为****x**的变量：

### 例子

```
var x = 10
```



**加法赋值运算**符（`+=`）将一个值添加到变量中：

### 例子

```
var x = 10
x += 5
```



所有赋值运算符的列表：

| Operator | Example | Same As   | Try it                                                       |
| -------- | ------- | --------- | ------------------------------------------------------------ |
| =        | x = 5   | x = 5     | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass1) |
| +=       | x += 3  | x = x + 3 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass2) |
| -=       | x -= 3  | x = x - 3 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass3) |
| *=       | x *= 3  | x = x * 3 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass4) |
| /=       | x /= 3  | x = x / 3 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass5) |
| %=       | x %= 3  | x = x % 3 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_ass6) |

------

## Kotlin 比较运算符

比较运算符用于比较两个值，并返回一个`Boolean` 值：要么`true`，要么`false`。

| Operator | Name                     | Example | Try it                                                       |
| -------- | ------------------------ | ------- | ------------------------------------------------------------ |
| ==       | Equal to                 | x == y  | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare1) |
| !=       | Not equal                | x != y  | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare2) |
| >        | Greater than             | x > y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare3) |
| <        | Less than                | x < y   | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare4) |
| >=       | Greater than or equal to | x >= y  | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare5) |
| <=       | Less than or equal to    | x <= y  | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_compare6) |

[您将在布尔](https://www.w3schools.com/kotlin/kotlin_booleans.php)章节和 [条件](https://www.w3schools.com/kotlin/kotlin_conditions.php)中了解有关布尔值的更多信息。

------

## Kotlin 逻辑运算符

逻辑运算符用于确定变量或值之间的逻辑：

| Operator | Name        | Description                                             | Example          | Try it                                                       |
| -------- | ----------- | ------------------------------------------------------- | ---------------- | ------------------------------------------------------------ |
| &&       | Logical and | Returns true if both statements are true                | x < 5 &&  x < 10 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_logical1) |
| \|\|     | Logical or  | Returns true if one of the statements is true           | x < 5 \|\| x < 4 | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_logical2) |
| !        | Logical not | Reverse the result, returns false if the result is true |                  | [Try it »](https://www.w3schools.com/kotlin/trykotlin.php?filename=demo_oper_logical3) |

## Kotlin 字符串

字符串用于存储文本。

字符串包含用双引号括起来的字符集合：

### 例子

```
var greeting = "Hello"
```



[与Java](https://www.w3schools.com/java/default.asp)不同，您不必指定变量必须是 a `String`。Kotlin 足够聪明，能够理解上面示例中的问候语变量是 a ，`String`因为双引号。

但是，就像其他数据类型一样，如果您坚持的话，您可以指定类型：

### 例子

```
var greeting: String = "Hello"
```



**注意：**如果要创建一个`String`不分配值（稍后再分配值），则必须在声明变量时指定类型：

### 例子

这很好用：

```
var name: String
name = "John"
println(name)
```



### 例子

这将产生一个错误：

```
var name
name = "John"
println(name)
```



------

## 访问字符串

要访问字符串的字符（元素），必须参考**方括号** 内的**索引号。**

字符串索引从 0 开始。在下面的示例中，我们访问中的第一个和第三个元素` txt`：

### 例子

```
var txt = "Hello World"
println(txt[0]) // first element (H)
println(txt[2]) // third element (l)
```



[0] 是第一个元素。[1] 是第二个元素，[2] 是第三个元素，等等。

------

------

## 字符串长度

Kotlin 中的字符串是一个对象，它包含一些属性和函数，可以`.`通过在特定字符串变量后添加点字符 ( ) 来对字符串执行某些操作。例如，可以使用以下属性查找字符串的长度`length` ：

### 例子

```
var txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
println("The length of the txt string is: " + txt.length)
```



------

## 字符串函数

有许多可用的字符串函数，例如`toUpperCase()`和`toLowerCase()`：

### 例子

```
var txt = "Hello World"
println(txt.toUpperCase())   // Outputs "HELLO WORLD"
println(txt.toLowerCase())   // Outputs "hello world"
```



------

## 比较字符串

该函数比较两个字符串，如果相等则返回 0：`compareTo(*string*)`

### 例子

```
var txt1 = "Hello World"
var txt2 = "Hello World"
println(txt1.compareTo(txt2))  // Outputs 0 (they are equal)
```



------

## 在字符串中查找字符串

该`indexOf()`函数返回字符串中指定文本第一次出现的**索引（位置）（包括空格）：**

### 例子

```
var txt = "Please locate where 'locate' occurs!"
println(txt.indexOf("locate"))  // Outputs 7
```



请记住，Kotlin 从零开始计算位置。0
是字符串中的第一个位置，1 是第二个位置，2 是第三个位置……

------

## 字符串内的引号

要在字符串中使用引号，请使用单引号 ( `'`)：

### 例子

```
var txt1 = "It's alright"
var txt2 = "That's great"
```



------

## 字符串连接

运算符`+`可以在字符串之间使用，将它们相加以创建一个新字符串。这称为**连接**：

### 例子

```
var firstName = "John"
var lastName = "Doe"
println(firstName + " " + lastName)
```



请注意，我们添加了一个空文本（“”），以便在打印时在 firstName 和 lastName 之间创建一个空格。

您还可以使用该`plus()`函数连接两个字符串：

### 例子

```
var firstName = "John "
var lastName = "Doe"
println(firstName.plus(lastName))
```



------

## 字符串模板/插值

除了连接之外，您还可以使用“字符串模板”，这是一种在字符串中添加变量和表达式的简单方法。

只需用符号引用变量`$`：

### 例子

```
var firstName = "John"
var lastName = "Doe"
println("My name is $firstName $lastName")
```



“字符串模板”是 Kotlin 的一个热门功能，因为它可以减少代码量。例如，您无需像我们在字符串连接示例中那样在 firstName 和 lastName 之间指定空格。

## Kotlin 布尔值

在编程中，您经常需要一种只能具有两个值之一的数据类型，例如：

- 是/否
- 开 / 关
- 正确 / 错误

为此，Kotlin 有一个`Boolean`数据类型，可以采用值`true`或`false`。

------

## 布尔值

布尔类型可以用`Boolean`关键字声明，并且只能采用值`true`或`false`：

### 例子

```
val isKotlinFun: Boolean = true
val isFishTasty: Boolean = false
println(isKotlinFun)   // Outputs true
println(isFishTasty)   // Outputs false 
```



就像您在前面章节中学习过的其他数据类型一样，上面的示例也可以在不指定类型的情况下编写，因为 Kotlin 足够智能，可以理解变量是布尔值：

### 例子

```
val isKotlinFun = true
val isFishTasty = false
println(isKotlinFun)   // Outputs true
println(isFishTasty)   // Outputs false 
```



------

------

## 布尔表达式

布尔表达式**返回**一个布尔值：`true`或`false`。

您可以使用比较运算符（例如**大于**( `>`) 运算符）来判断表达式（或变量）是否为真：

### 例子

```
val x = 10
val y = 9
println(x > y) // Returns true, because 10 is greater than 9
```



或者更简单：

### 例子

```
println(10 > 9) // Returns true, because 10 is greater than 9
```



在下面的例子中，我们使用**等于**（`==`）运算符来评估表达式：

### 例子

```
val x = 10;
println(x == 10); // Returns true, because the value of x is equal to 10
```



### 例子

```
println(10 == 15); // Returns false, because 10 is not equal to 15
```

## Kotlin 条件和 If..Else

Kotlin 支持数学中常见的逻辑条件：

- 小于：a < b
- 小于或等于：a <= b
- 大于：a > b
- 大于或等于：a >= b
- 等于a == b
- 不等于：a != b

您可以使用这些条件针对不同的决策执行不同的操作。

Kotlin 具有以下条件：

- 用于`if`指定当指定条件为真时要执行的代码块
- 用于`else`指定当相同条件为假时要执行的代码块
- 如果第一个条件为假，则用于`else if`指定要测试的新条件
- 用于`when`指定要执行的许多备选代码块

**注意：**与 Java 不同，在 Kotlin 中，`if..else`它可以用作 **语句**或表达式**（**用于为变量赋值）。请参阅页面底部的示例以更好地理解它。

------

## Kotlin 如果

用于`if`指定在满足条件时执行的代码块`true`。

### 句法

```
if (condition) {
  // block of code to be executed if the condition is true
}
```

请注意，`if`是小写字母。大写字母（If 或 IF）将产生错误。

在下面的例子中，我们测试两个值来确定 20 是否大于 18。如果条件成立`true`，则打印一些文本：

### 例子

```
if (20 > 18) {
  println("20 is greater than 18")
}
```



我们还可以测试变量：

### 例子

```
val x = 20
val y = 18
if (x > y) {
  println("x is greater than y")
}
```



#### 示例解释

在上面的例子中，我们使用两个变量**x**和**y**来测试 x 是否大于 y（使用`>`运算符）。由于 x 等于 20，y 等于 18，而我们知道 20 大于 18，因此我们在屏幕上打印“x 大于 y”。

------

------

## Kotlin 其他

用于`else`指定在条件满足时执行的代码块`false`。

### 句法

```
if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
```

### 例子

```
val time = 20
if (time < 18) {
  println("Good day.")
} else {
  println("Good evening.")
}
// Outputs "Good evening."
```



#### 示例解释

在上面的例子中，时间 (20) 大于 18，所以条件为`false`，所以我们继续执行`else`条件并在屏幕上打印“Good evening”。如果时间小于 18，程序将打印“Good day”。

------

## Kotlin else if

如果第一个条件为 ，则用于`else if`指定新条件`false`。

### 句法

```
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
```

### 例子

```
val time = 22
if (time < 10) {
  println("Good morning.")
} else if (time < 20) {
  println("Good day.")
} else {
  println("Good evening.")
}
// Outputs "Good evening."
```



#### 示例解释

在上面的例子中，时间 (22) 大于 10，所以**第一个条件**是`false`。语句中的下一个条件 `else if`也是`false`，所以我们继续执行`else` 条件，因为**条件 1**和**条件 2**都是`false`- ，并在屏幕上打印“晚上好”。

但是，如果时间是 14，我们的程序就会打印“Good day”。

------

## Kotlin If..Else 表达式

在 Kotlin 中，您还可以将`if..else`语句用作表达式（将值分配给变量并返回它）：

### 例子

```
val time = 20
val greeting = if (time < 18) {
  "Good day."
} else {
  "Good evening."
}
println(greeting)
```



当用作`if`表达式时，还必须包含`else`（必需）。

**注意：**`{}` 当`if`只有一个语句时，可以省略花括号：

### 例子

```
fun main() {
  val time = 20
  val greeting = if (time < 18) "Good day." else "Good evening."
  println(greeting)
}
```



**提示：**此示例类似于 Java 中的“三元运算符”（简写 if...else）。Kotlin 何时

您无需编写许多`if..else`表达式，而可以使用`when` 表达式，这更容易阅读。

它用于选择要执行的多个代码块之一：

### 例子

使用星期几数字来计算星期几名称：

```
val day = 4

val result = when (day) {
  1 -> "Monday"
  2 -> "Tuesday"
  3 -> "Wednesday"
  4 -> "Thursday"
  5 -> "Friday"
  6 -> "Saturday"
  7 -> "Sunday"
  else -> "Invalid day."
}
println(result)

// Outputs "Thursday" (day 4)
```



该`when`表达式类似于`switch`Java中的语句。

工作原理如下：

- 变量`when`（**day**）被评估一次

- **将日期**变量的值与每个“分支”的值进行比较

- 每个分支都以一个值开始，后跟一个箭头 (->) 和一个结果

- 如果匹配，则执行相关的代码块

- `else`用于指定在没有匹配时运行的代码

- 在上面的例子中，值为`day`，`4`表示将打印“星期四”


## 循环

只要达到指定的条件，循环就可以执行一段代码。

循环很方便，因为它们可以节省时间、减少错误并使代码更具可读性。

------

## Kotlin While 循环

`while`只要满足指定的条件，循环就会循环遍历代码块`true`：

### 句法

```
while (condition) {
  // code block to be executed
}
```

在下面的例子中，只要计数器变量 (i) 小于 5，循环中的代码就会一遍又一遍地运行：

### 例子

```
var i = 0
while (i < 5) {
  println(i)
  i++
} 
```



**注意：**不要忘记增加条件中使用的变量，否则循环将永远不会结束。

------

------

## Do..While 循环

循环`do..while`是`while`循环的一个变体。此循环会在检查条件是否为真之前执行一次代码块，然后只要条件为真，它就会重复循环。

### 句法

```
do {
  // code block to be executed
}
while (condition);
```

下面的例子使用了一个`do/while`循环。即使条件为假，循环也总是会执行至少一次，因为代码块在条件测试之前就执行了：

### 例子

```
var i = 0
do {
  println(i)
  i++
  }
while (i < 5) 
```



不要忘记增加条件中使用的变量，否则循环将永远不会结束！

## Kotlin  break

该`break`语句用于跳出 **循环**。

此示例在 i 等于 4 时跳出循环：

### 例子

```
var i = 0
while (i < 10) {
  println(i)
  i++
  if (i == 4) {
    break
  }
}
```



------

## Kotlin  continue

如果发生指定条件，该`continue`语句将中断一次迭代（在循环中），并继续循环中的下一次迭代。

此示例跳过值 4：

### 例子

```
var i = 0
while (i < 10) {
  if (i == 4) {
    i++
    continue
  }
  println(i)
  i++
}
```

  Kotlin 数组

数组用于在单个变量中存储多个值，而不是为每个值创建单独的变量。

要创建数组，请使用`arrayOf()`函数，并将值放在其中的逗号分隔的列表中：

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
```

------

## 访问数组元素

您可以通过引用**方括号**内的**索引号**来访问数组元素。

在这个例子中，我们访问 automobile 中第一个元素的值：

### 例子

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
println(cars[0])
// Outputs Volvo 
```



**注意：**与字符串一样，数组索引从 0 开始：[0] 是第一个元素。 [1] 是第二个元素，等等。

------

## 更改数组元素

要更改特定元素的值，请参考索引号：

### 例子

```
cars[0] = "Opel"
```

### 例子

val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
cars[0] = "Opel"
println(cars[0])
// Now outputs Opel instead of Volvo



------

## 数组长度/大小

要找出数组有多少个元素，请使用以下`size`属性：

### 例子

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
println(cars.size)
// Outputs 4 
```



------

------

## 检查元素是否存在

您可以使用`in`运算符来检查数组中是否存在某个元素：

### 例子

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
if ("Volvo" in cars) {
  println("It exists!")
} else {
  println("It does not exist.")
}
```



------

## 循环遍历数组

通常，当您使用数组时，您需要循环遍历所有元素。

您可以使用循环遍历数组元素`for` ，您将在下一章中了解更多相关内容。

以下示例输出**汽车** 数组中的所有元素：

### 例子

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
for (x in cars) {
  println(x)
}
```

## Kotlin For 循环

通常，当您使用数组时，您需要循环遍历所有元素。

要循环遍历数组元素，请将`for` 循环与运算符一起使用`in`：

### 例子

输出cars数组中的所有元素：

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
for (x in cars) {
  println(x)
}
```



你可以循环遍历各种类型的数组。在上面的例子中，我们使用了一个字符串数组。

在下面的例子中，我们循环遍历一个整数数组：

### 例子

```
val nums = arrayOf(1, 5, 10, 15, 20)
for (x in nums) {
  println(x)
}
```



------

## 传统 For 循环

`for`与 Java 和其他编程语言不同， Kotlin 中没有传统的循环。

在 Kotlin 中，`for`循环用于循环遍历数组、范围和其他包含可计数值的内容。

您将在下一章中了解**有关范围的更多信息 - 这将创建一系列值。**

------

## Kotlin 范围

通过[`for`循环](https://www.w3schools.com/kotlin/kotlin_for_loop.php)，您还可以 使用“”创建值**范围**`..`：

### 例子

打印整个字母表：

```
for (chars in 'a'..'x') {
  println(chars)
}
```



您还可以创建数字范围：

### 例子

```
for (nums in 5..15) {
  println(nums)
} 
```



**注意：**第一个值和最后一个值包含在范围内。

------

## 检查值是否存在

您还可以使用`in`运算符来检查某个值是否存在于某个范围内：

### 例子

```
val nums = arrayOf(2, 4, 6, 8)
if (2 in nums) {
  println("It exists!")
} else {
  println("It does not exist.")
}
```



### 例子

```
val cars = arrayOf("Volvo", "BMW", "Ford", "Mazda")
if ("Volvo" in cars) {
  println("It exists!")
} else {
  println("It does not exist.")
} 
```



------

------

## 打破或延续范围

您还可以在范围/循环中使用`break`和关键字：`continue``for`

### 例子

`nums`当等于时停止循环`10`：

```
for (nums in 5..15) {
  if (nums == 10) {
    break
  }
  println(nums)
} 
```



### 例子

跳过循环中的值 10，继续下一次迭代：

```
for (nums in 5..15) {
  if (nums == 10) {
    continue
  }
  println(nums)
} 
```



## Kotlin 函数



函数是仅在被调用**时**运行的代码块。

您可以将数据（称为参数）传递到函数中。

函数用于执行某些操作，也称为**方法**。

------

## 预定义函数

看来你已经知道函数是什么了。你在本教程中一直在使用它！

例如，`println()`是一个函数。它用于将文本输出/打印到屏幕：

### 例子

```
fun main() {
  println("Hello World")
}
```



------

## 创建你自己的函数

要创建自己的函数，请使用`fun`关键字，并写下函数的名称，后跟括号**()**：

### 例子

创建一个名为“myFunction”的函数，该函数输出一些文本：

```
fun myFunction() {
  println("I just got executed!")
} 
```

------

## 调用函数

现在您已经创建了一个函数，您可以通过**调用**它来执行它 。

要在 Kotlin 中调用函数，请写下函数名称，后跟两个括号**()**。

在下面的例子中，`myFunction()`当它被调用时，将会打印一些文本（动作）：

### 例子

```
fun main() {
  myFunction() // Call myFunction
}

// Outputs "I just got executed!" 
```



如果需要，可以多次调用一个函数：

### 例子

```
fun main() {
  myFunction()
  myFunction()
  myFunction()
}

// I just got executed!
// I just got executed!
// I just got executed! 
```



------

------

## 函数参数

信息可以作为参数传递给函数。

参数在函数名称后的括号内指定。您可以添加任意数量的参数，只需用逗号分隔即可。请注意，必须指定每个参数的类型（Int、String 等）。

下面的示例有一个函数，它接受一个`String`叫做**fname**的函数作为参数。当函数被调用时，我们传递一个名字，该名字在函数内部用于打印全名：

### 例子

```
fun myFunction(fname: String) {
  println(fname + " Doe")
}

fun main() {
  myFunction("John")
  myFunction("Jane")
  myFunction("George")
}
  
// John Doe
// Jane Doe
// George Doe 
```



------

当一个**参数**被传递给函数时，它被称为**参数**。因此，从上面的例子来看：`fname`是**参数**， while `John`，`Jane`并且` George`是**参数**。

------

## 多个参数

您可以拥有任意数量的参数：

### 例子

```
fun myFunction(fname: String, age: Int) {
  println(fname + " is " + age)
}

fun main() {
  myFunction("John", 35)
  myFunction("Jane", 32)
  myFunction("George", 15)
}

// John is 35
// Jane is 32
// George is 15 
```



**注意：**使用多个参数时，函数调用的参数数量必须与参数数量相同，并且参数必须按相同的顺序传递。

------

## 返回值

在上面的例子中，我们使用了函数来输出一个值。在下面的例子中，我们将使用函数 **返回**一个值并将其赋给一个变量。

要返回一个值，请使用关键字，并在函数的括号后`return`指定 **返回类型**`Int`（在此示例中）：

### 例子

`Int`具有一个参数和`Int`返回类型的函数：

```
fun myFunction(x: Int): Int {
  return (x + 5)
}

fun main() {
  var result = myFunction(3)
  println(result)
}

// 8 (3 + 5) 
```



使用两个参数：

### 例子

`Int`具有两个参数和`Int`返回类型的函数：

```
fun myFunction(x: Int, y: Int): Int {
  return (x + y)
}

fun main() {
  var result = myFunction(3, 5)
  println(result)
}

// 8 (3 + 5) 
```



------

## 返回值的更短语法

还有一种更简洁的返回值语法。你可以使用`=`运算符，而`return` 无需指定返回类型。Kotlin 非常智能，可以自动识别返回值的类型：

### 例子

```
fun myFunction(x: Int, y: Int) = x + y

fun main() {
  var result = myFunction(3, 5)
  println(result)
}

// 8 (3 + 5) 
```



# Kotlin 类

## Kotlin——什么是 OOP？

OOP 代表**面向对象编程**。

过程编程是关于编写对数据执行操作的过程或方法，而面向对象编程是关于创建包含数据和方法的对象。

面向对象编程比过程编程有几个优点：

- OOP 更快、更容易执行
- OOP 为程序提供了清晰的结构
- OOP 有助于保持 Kotlin 代码 DRY“不要重复自己”，并使代码更易于维护、修改和调试
- OOP 可以用更少的代码和更短的开发时间创建完全可重用的应用程序

**提示：** “不要重复自己”（DRY）原则旨在减少代码的重复。您应该提取应用程序中常用的代码，并将它们放在一个地方重复使用，而不是重复使用。

------

## Kotlin - 什么是类和对象？

类和对象是面向对象编程的两个主要方面。

看下面的插图来了解类和对象之间的区别：
![75039132127](E:\code\kotlin\kotlin_learn\assets\1750391321274.png)

另一个例子：
![75039134913](E:\code\kotlin\kotlin_learn\assets\1750391349134.png)

因此，类是对象的模板，而对象是类的实例。

当创建单个对象时，它们会继承类中的所有变量和方法。

您将在下一章中学习更多有关类和对象的知识。

## Kotlin 类/对象

Kotlin 中的所有内容都与类和对象及其属性和函数相关联。例如：在现实生活中，汽车是一个**对象**。汽车具有**属性**，例如品牌、重量和颜色，以及 **功能**，例如驾驶和刹车。

类就像对象构造函数，或者创建对象的“蓝图”。

------

## 创建一个类

要创建一个类，请使用`class`关键字，并指定类的名称：

### 例子

创建一个**Car**类以及一些**属性**（品牌、型号和年份）

```
class Car {
  var brand = ""
  var model = ""
  var year = 0
} 
```

属性基本上是属于类的**变量**[**。**](https://www.w3schools.com/kotlin/kotlin_variables.php)

**值得了解的是：**为了更好地组织，以大写字母开头类名被认为是一种很好的做法。

------

## 创建对象

**现在我们可以使用名为Car**的类来创建对象。

在下面的示例中，我们创建一个名为 **c1的****Car**对象，然后使用点语法 ( ) 访问**c1**的属性，就像访问数组和字符串属性一样：`.`

### 例子

```
// Create a c1 object of the Car class
val c1 = Car()

// Access the properties and add some values to it
c1.brand = "Ford"
c1.model = "Mustang"
c1.year = 1969

println(c1.brand)   // Outputs Ford
println(c1.model)   // Outputs Mustang
println(c1.year)    // Outputs 1969 
```



------

------

## 多个对象

您可以创建一个类的多个对象：

### 例子

```
val c1 = Car()
c1.brand = "Ford"
c1.model = "Mustang"
c1.year = 1969

val c2 = Car()
c2.brand = "BMW"
c2.model = "X5"
c2.year = 1999

println(c1.brand)  // Ford
println(c2.brand)  // BMW
```

## Kotlin 构造函数

在上一章中，我们创建了一个类的对象，并在类内部指定了属性，如下所示：

### 例子

```
class Car {
  var brand = ""
  var model = ""
  var year = 0
}

fun main() {
  val c1 = Car()
  c1.brand = "Ford"
  c1.model = "Mustang"
  c1.year = 1969
}
```



在 Kotlin 中，有一种更快的方法来实现这一点，那就是使用**构造函数**。

构造函数就像一个特殊的[函数](https://www.w3schools.com/kotlin/kotlin_functions.php)，它`()` 通过在类名后使用两个括号来定义。你可以在括号内指定属性（就像将参数传递给常规函数一样）。

构造函数会在创建类的对象时初始化属性。只需记住指定属性/变量的类型即可：

### 例子

```
class Car(var brand: String, var model: String, var year: Int)

fun main() {
  val c1 = Car("Ford", "Mustang", 1969)
}
```



现在指定一个类的多个对象变得更加容易：

### 例子

```
class Car(var brand: String, var model: String, var year: Int)

fun main() {
  val c1 = Car("Ford", "Mustang", 1969)
  val c2 = Car("BMW", "X5", 1999)
  val c3 = Car("Tesla", "Model S", 2020)
}
```



## Kotlin 类函数

您还可以使用类内的[函数来执行某些操作：](https://www.w3schools.com/kotlin/kotlin_functions.php)

### 例子

在类内部创建一个`drive()`函数 `Car`并调用它：

```
class Car(var brand: String, var model: String, var year: Int) {
  // Class function
  fun drive() {
    println("Wrooom!")
  }
}

fun main() {
  val c1 = Car("Ford", "Mustang", 1969)
  
  // Call the function
  c1.drive()
}
```



**提示：**当一个函数在类内部声明时，它被称为*类函数*或 *成员函数*。

**注意：**当创建类的对象时，它可以访问所有类函数。

------

## 类函数参数

与常规函数一样，您可以将参数传递给类函数：

### 例子

创建两个函数：`drive()`和`speed()`，并将参数传递给 `speed()`函数：

```
class Car(var brand: String, var model: String, var year: Int) {
  // Class function
  fun drive() {
    println("Wrooom!")
  }
  
  // Class function with parameters
  fun speed(maxSpeed: Int) {
    println("Max speed is: " + maxSpeed)
  }
}

fun main() {
  val c1 = Car("Ford", "Mustang", 1969)
  
  // Call the functions
  c1.drive()
  c1.speed(200)
}
```



## Kotlin 继承（子类和超类）

在 Kotlin 中，可以将类的属性和函数从一个类继承到另一个类。我们将“继承概念”分为两类：

- **子类**（子）——从另一个类继承的类
- **超类**（父类）——被继承的类

在下面的例子中， （子类）从类（超类）`MyChildClass`继承了属性：` MyParentClass`

### 例子

```
// Superclass
open class MyParentClass {
  val x = 5
}

// Subclass
class MyChildClass: MyParentClass() {
  fun myFunction() {
    println(x) // x is now inherited from the superclass
  }
}

// Create an object of MyChildClass and call myFunction
fun main() {
  val myObj = MyChildClass()
  myObj.myFunction()
} 
```



## 示例解释

**在超类**`open`/parent前面使用关键字，使该类成为其他类应该继承属性和函数的类。

**要从类继承，请指定子类**的名称，后跟冒号，然后是**超类**`:`的名称。

#### 为什么以及何时使用“继承”？

\- 它对于代码可重用性很有用：创建新类时重用现有类的属性和函数。




