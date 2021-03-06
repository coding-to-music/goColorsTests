
 <h2 align="center">Examples of using color in Go</h2>

<br/>
&nbsp;

<p align="center">
 <img width="600px" src="https://github.com/coding-to-music/goColorsTests/blob/main/go-run-main.png?raw=true" align="center" alt="Using Colors in Go" />
 

&nbsp;
&nbsp;
<br/>
<br/>
Source of the code is [HERE](https://gist.github.com/ik5/d8ecde700972d4378d87)
<br/>

&nbsp;

Good article about using Color in golang [HERE](https://twinnation.org/articles/35/how-to-add-colors-to-your-console-terminal-output-in-go)

Simon Tony wrote a Medium article [Terminal color render by Golang](https://medium.com/@inhereat/terminal-color-rendering-tool-library-support-8-16-colors-256-colors-by-golang-a68fb8deee86)


&nbsp;

<br/>
<p align="center">
 <img width="600px" src="https://github.com/coding-to-music/goColorsTests/blob/main/twinnation-go-colors.png?raw=true" align="center" alt="Using Colors in Go" />
<br/>
&nbsp;

## Define like this:
```bash
package color

import "runtime"

var Reset   = "\033[0m"
var Red     = "\033[31m"
var Green   = "\033[32m"
var Yellow  = "\033[33m"
var Blue    = "\033[34m"
var Purple  = "\033[35m"
var Cyan    = "\033[36m"
var Gray    = "\033[37m"
var White   = "\033[97m"


func init() {
	if runtime.GOOS == "windows" {
		Reset   = ""
		Red     = ""
		Green   = ""
		Yellow  = ""
		Blue    = ""
		Purple  = ""
		Cyan    = ""
		Gray    = ""
		White   = ""
	}
}
```

## Invoke like this:

```bash
func main() {
    fmt.Println(color.White + "This is White" + color.Reset)
    fmt.Println(color.Red + "This is Red" + color.Reset)
    fmt.Println(color.Green + "This is Green" + color.Reset)
    fmt.Println(color.Yellow + "This is Yellow" + color.Reset)
    fmt.Println(color.Blue + "This is Blue" + color.Reset)
    fmt.Println(color.Purple + "This is Purple" + color.Reset)
    fmt.Println(color.Cyan + "This is Cyan" + color.Reset)
    fmt.Println(color.Gray + "This is Gray" + color.Reset)
}
```
&nbsp;
<br/>
<p align="center">
 <img width="600px" src="https://github.com/coding-to-music/goColorsTests/blob/main/fatih-color.jpg?raw=true" align="center" alt="" />
 
 
Go fatih/color Package docs are [HERE](https://github.com/fatih/color)<br/>

<p align="center">
 <img width="600px" src="https://github.com/coding-to-music/goColorsTests/blob/main/SimonTonyMedium.png?raw=true" align="center" alt="" />


 <br/>
&nbsp;

Simon Tony wrote a Medium article [Terminal color render by Golang](https://medium.com/@inhereat/terminal-color-rendering-tool-library-support-8-16-colors-256-colors-by-golang-a68fb8deee86)

<p align="center">
 <img width="600px" src="https://github.com/coding-to-music/goColorsTests/blob/main/SimonTonyColors2.jpg?raw=true" align="center" alt="" />

