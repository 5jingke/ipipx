[ipip.net](http://www.ipip.net/) IP location data for Golang (datx)
===

## 安装

	go get -u github.com/chentao/ipipx

## 使用
	import （
		"fmt"
		"github.com/chentao/ipipx"
	）

	func init() {
		if err := ipipx.Init("/path/to/datx/file"); err != nil {
			panic(err)
		}
	}

	func main() {
		loc, err := ipipx.Find("116.228.111.18")
		if err != nil {
			fmt.Println("err:", err)
			return
		}
		fmt.Println(loc)
	}

## 许可证

基于 [MIT](https://github.com/chentao/ipipx/blob/master/LICENSE) 协议发布
