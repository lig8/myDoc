### 数据类型





#### print函数

> 1、Print: 将信息显示在命令窗口中，输出光标定位在最后一个字符之后；
>
> 2、Println：将信息显示在命令窗口中，输出光标换行定位在下一行开头，相当于print(\n)
>
> 3、Printf: 将信息进行格式化显示在命令窗口中，输出光标定位在最后一个字符之后,



#### 数据类型

> Go 的数据类型主要有 string, int, float, bool等



#### 变量

> 1、go语言用var关键字定义变量，一次可以定义一个或多个变量
>
> 2、可以在定义变量的同时给变量赋值
>
> 3、变量如果没有指定类型，可以在赋值时自适应确定类型
>
> 4、可以用 ' := ' 符号快捷完成赋值与类型识别

```go
package main
import "fmt"

func main() {
	var str1 = "hello world"
	fmt.Println(str1)

	var a, b int = 8, 10
	fmt.Printf("a=%d,b=%d \n", a, b)

	var c, d int
	c, d = 5, 9
	fmt.Print("c=", c, " d=", d, "\n")

	e, f := 7, 8
	fmt.Printf("e+f=%d\n", e+f)

	var g int
	var h string
	var i bool
	fmt.Println(g, "\n", h, "\n", i)
}
```



```go
$ go run ../hello.go
hello world
a=8,b=10
c=5 d=9
e+f=15
0

 false
```



