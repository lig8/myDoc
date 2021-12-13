---

---



### for 语句

```go
package main
import "fmt"

func main() {
	var i int = 100
	for i > 98 {
		fmt.Println(i)
		i--
	}

	for j := 98; j < 100; j++ {
		fmt.Println(j)
	}

	var str1 string
	var var1 int = 0
	for {
		fmt.Print("input[exit] to exit:")
		fmt.Scanf("%s", &str1)
		if str1 == "exit" {
			break
		} else {
			var1++
			fmt.Printf("count = %d\n", var1)
		}
	}
}

```



### if...else...语句

```go
package main

import "fmt"

func main() {

	var a, b int

	fmt.Print("Please input value for a:")
	fmt.Scanf("%d", &a)
	fmt.Print("Please input value for b:")
	fmt.Scanf("%d", &b)

	if a > b {
		fmt.Println("a>b")
	} else {
		fmt.Println("a<b or a=b")
	}

	if c := 10; a > c {
		fmt.Println("a>c")
	} else if a == c {
		fmt.Println("a==c")
	} else {
		fmt.Println("a<c")
	}
}

```





### switch语句

```go
package main

import "fmt"

func main() {

	var a int
	fmt.Print("Please input value for a:")
	fmt.Scanf("%d", &a)

	switch a {
	case 1:
		fmt.Println("you input one")
		break
	case 2:
		fmt.Println("you input two")
		break
	case 3:
		fmt.Println("you input three")
		break
	case 4:
		fmt.Println("you input four")
		break
	default:
		fmt.Println("you input other")
	}

	CheckType := func(i interface{}) {
		switch t := i.(type) {
		case bool:
			fmt.Println("your type is bool")
			break
		case int:
			fmt.Println("your type is int")
			break
		default:
			fmt.Printf("your type is %T\n", t)
			break
		}
	}

	CheckType(true)
	CheckType(1)
	CheckType("hey")
}

```

