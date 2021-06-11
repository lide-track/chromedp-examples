# 关于chromedp例子


[ENGLISH](README.md)

此文件夹包含各种用于使用的代码示例[`chromedp`][1]. godoc页面包含了许多[简单的例子][2]，它们通常是自包含的， 而这个存储库包含更复杂的示例这往往需要Internet访问或外部组件。

请注意，当`chromedp`包被重写时，这些例子可能打破。此外，由于这些例子是为特定的网站编写的，有一个很好的机会，当前的选择器等中断后的网站他们反对改变。

虽然我们已尽一切努力确保这些例子是最新的，希望这里提供的示例偶尔会出错。

要归档问题，请使用[chromedp的问题跟踪器][3]。

## 构建和运行一个示例

您可以用通常的Go way构建和运行这些示例:

```sh
# retrieve examples
$ go get -u -d github.com/lide-track/examples

# run example <prog>
$ go run $GOPATH/src/github.com/chromedp/examples/<prog>/main.go

# build example <prog>
$ go build -o <prog> github.com/chromedp/examples/<prog> && ./<prog>
```
### 可用的例子

以下示例目前可用:

<!-- the following section is updated by running `go run gen.go` -->
<!-- START EXAMPLES -->
| Example                           | Description                                                                  |
|-----------------------------------|------------------------------------------------------------------------------|
| [click2](/click2)                 | 使用选择器单击元素                                        |
| [click](/click)                   | 使用选择器单击元素                                        |
| [cookie](/cookie)                 | 设置HTTP cookie的请求                                                |
| [download_file](/download_file)   | 无头文件下载                                                   |
| [download_image](/download_image) | 无头图片下载                                                  |
| [emulate](/emulate)               | 模拟一个特定的设备，比如iPhone                                  |
| [eval](/eval)                     | 计算javascript并检索结果                                  |
| [headers](/headers)               | 添加额外的HTTP头到浏览器请求                                   |
| [keys](/keys)                     | 向元素发送键事件                                                |
| [logic](/logic)                   | 更复杂的逻辑超出了简单的操作                                     |
| [pdf](/pdf)                       | 捕获一个页面的PDF                                                      |
| [proxy](/proxy)                   | 验证需要验证的代理服务器                    |
| [remote](/remote)                 | 连接到现有的Chrome DevTools实例使用一个远程WebSocket URL |
| [screenshot](/screenshot)         | 取特定元素和整个浏览器视口的截图   |
| [submit](/submit)                 | 填写并提交表格                                                   |
| [subtree](/subtree)               | 填充和移动DOM的一个子树                                     |
| [text2](/text2)                   | 从特定元素中提取文本                                         |
| [text](/text)                     | 从特定元素中提取文本                                         |
| [upload](/upload)                 | 在表单上上传文件                                                      |
| [visible](/visible)               | 等待元素是可见的                                             |
<!-- END EXAMPLES -->

## 贡献

Pull Requests和对这个项目的贡献被极大地鼓励欢迎!“chromedp”项目总是需要新的例子，需要天才开发人员(比如你自己!)提交修复现有例子时它们会中断(例如，当一个网站的布局/HTML改变时)。

[1]: https://github.com/chromedp/chromedp
[2]: https://godoc.org/github.com/chromedp/chromedp#pkg-examples
[3]: https://github.com/chromedp/chromedp/issues
