[17mon](http://www.ipip.net/) IP location data for Golang (datx)
===

## 安装

	go get -u github.com/chentao/ip17monx

## 使用
	import （
		"fmt"
		"github.com/chentao/ip17monx"
	）

	func init() {
		if err := ip17monx.Init("/path/to/datx/file"); err != nil {
			panic(err)
		}
	}

	func main() {
		loc, err := ip17monx.Find("116.228.111.18")
		if err != nil {
			fmt.Println("err:", err)
			return
		}
		fmt.Println(loc)
	}

## 许可证

基于 [MIT](https://github.com/wangtuanjie/ip17mon/blob/master/LICENSE) 协议发布
