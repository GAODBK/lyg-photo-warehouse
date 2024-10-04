[这是图片仓库的 json 链接](https://api.github.com/repos/GAODBK/lyg-photo-warehouse/contents)



```java
public class UrlConverter {

    public static String convertUrl(String inputUrl) {
        // 检查输入字符串是否包含 raw.githubusercontent.com
        if (inputUrl.contains("https://raw.githubusercontent.com/")) {
            // 使用正则表达式替换 URL 的相关部分
            String outputUrl = inputUrl.replace("https://raw.githubusercontent.com/", "https://cdn.jsdelivr.net/gh/");
            // 替换 master 之前的部分为 @ 符号
            outputUrl = outputUrl.replace("/master/", "@master/");
            return outputUrl;
        } else {
            // 如果输入 URL 不符合预期格式，返回原字符串
            return inputUrl;
        }
    }

    public static void main(String[] args) {
        // 测试字符串1
        String inputUrl = "https://raw.githubusercontent.com/LinMoQC/gitTest/master/1656780415433.png";
        // 转换为字符串2
        String result = convertUrl(inputUrl);
        // 输出结果
        System.out.println("转换后的URL: " + result);
    }
}
```

```C#
using System;

class Program
{
    static void Main()
    {
        // 输入的字符串1
        string inputUrl = "https://raw.githubusercontent.com/LinMoQC/gitTest/master/1656780415433.png";
        
        // 调用转换函数获取结果
        string result = ConvertUrl(inputUrl);
        
        // 输出结果
        Console.WriteLine("转换后的URL: " + result);
    }

    static string ConvertUrl(string inputUrl)
    {
        // 检查输入字符串是否包含 raw.githubusercontent.com
        if (inputUrl.Contains("https://raw.githubusercontent.com/"))
        {
            // 使用 Replace 方法替换 URL 中的部分
            string outputUrl = inputUrl.Replace("https://raw.githubusercontent.com/", "https://cdn.jsdelivr.net/gh/");
            // 替换 /master/ 为 @master/
            outputUrl = outputUrl.Replace("/master/", "@master/");
            return outputUrl;
        }
        else
        {
            // 如果 URL 不符合预期格式，返回原字符串
            return inputUrl;
        }
    }
}
```

```js
function convertUrl(inputUrl) {
    // 检查输入的 URL 是否包含 raw.githubusercontent.com
    if (inputUrl.includes("https://raw.githubusercontent.com/")) {
        // 使用 replace 方法替换 URL 的相关部分
        let outputUrl = inputUrl.replace("https://raw.githubusercontent.com/", "https://cdn.jsdelivr.net/gh/");
        // 替换 /master/ 为 @master/
        outputUrl = outputUrl.replace("/master/", "@master/");
        return outputUrl;
    } else {
        // 如果 URL 不符合预期格式，返回原字符串
        return inputUrl;
    }
}
```



现在这个仓库是我的图库有几个项目的图片

例如：

- D:\code\FLUTTERCODE\Router-project\src\images

![手机商城](/14-59.png)



- D:\code\WEB_CODE\Router-project\src\images

![水果商城](/14-01.png)



- dfg

![ai](/15-00.png)