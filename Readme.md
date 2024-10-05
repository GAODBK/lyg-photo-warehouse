[这是图片仓库的 json 链接](https://api.github.com/repos/GAODBK/lyg-photo-warehouse/contents)


```
jsd.cdn.zzko.cn √

cdn.jsdmirror.com √

cdn.jsdelivr.net √
```


```java
public class UrlConverter {
    public static String convertUrl(String inputUrl) {
        // 检查输入字符串是否包含 raw.githubusercontent.com
        if (inputUrl.contains("https://raw.githubusercontent.com/")) {
            // 使用正则表达式替换 URL 的相关部分
            String outputUrl = inputUrl.replace("https://raw.githubusercontent.com/", "https://cdn.jsdelivr.net/gh/");
            // 替换 master 之前的部分为 @ 符号
            outputUrl = outputUrl.replace("/main/", "@main/");
            return outputUrl;
        } else {
            // 如果输入 URL 不符合预期格式，返回原字符串
            return inputUrl;
        }
    }
}
```

```C#
using System;
class Program
{
    static string ConvertUrl(string inputUrl)
    {
        // 检查输入字符串是否包含 raw.githubusercontent.com
        if (inputUrl.Contains("https://raw.githubusercontent.com/"))
        {
            // 使用 Replace 方法替换 URL 中的部分
            string outputUrl = inputUrl.Replace("https://raw.githubusercontent.com/", "https://jsd.cdn.zzko.cn/gh/");
            // 替换 /master/ 为 @master/
            outputUrl = outputUrl.Replace("/main/", "@main/");
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
        let outputUrl = inputUrl.replace("https://raw.githubusercontent.com/", "https://cdn.jsdmirror.com/gh/");
        // 替换 /master/ 为 @master/
        outputUrl = outputUrl.replace("/main/", "@main/");
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
