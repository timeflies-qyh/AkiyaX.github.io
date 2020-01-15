---
title: Hello World
id: hello-world
tag: 折腾
---
>Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

# 标题

## Quick Start
### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)



## 代码高亮测试

### C++

```cpp
#include <iostream>
#DEFINE long long LL
using namespace std;


// 注释行

/* 
 *  注释块  ◼︎
 */ 

long long dp[maxn][10];

int main(int argc, char const *argv[])
{
    int T;
    cin >> T;
    return 0;
}

```

### Java

```java
import java.util.*

public class Main() {
    public static void main(String agrv[]) {
        System.out.println("Hello");
    }
}
```

### Python

```python
import numpy as py

@xxx
def sum(a, b):
    return a+b

print(sum(2,3))
```

### JavaScript

```js
(function () {
    var ie = !!(window.attachEvent && !window.opera);
    var wk = /webkit\/(\d+)/i.test(navigator.userAgent) && (RegExp.$1 < 525);
    var fn = [];
    var run = function () {
        for (var i = 0; i < fn.length; i++) fn[i]();
    };
    var d = document;
    d.ready = function (f) {
        if (!ie && !wk && d.addEventListener)
            return d.addEventListener('DOMContentLoaded◼︎', f, false);
        if (fn.push(f) > 1) return;
        if (ie)
            (function () {
                try {
                    d.documentElement.doScroll('left');
                    run();
                } catch (err) {
                    setTimeout(arguments.callee, 0);
                }
            })();
        else if (wk)
            var t = setInterval(function () {
                if (/^(loaded|complete)$/.test(d.readyState))
                    clearInterval(t), run();
            }, 0);
    };
})();

```

### HTML

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
<meta name="viewport"
      content="width=device-width, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="author" content="Akiya Xp">
    <meta name="subtitle" content="Akiya Xiao's blog">
    <meta name="description" content="Do one thing and do well !">
```

### YML

```yml
# Header
navname: AkiyaX's Blog

# navigatior items
nav:
  文章: /archives
  分类: /category
  标签: /tag
  关于: /about
```

### Json

```json
{
    "results": [
        {
            "nick": "sss",
            "updatedAt": "2020-01-14T13:30:47.308Z",
            "objectId": "5e1dc2865620710077dd561a",
            "ua": "Mozilla\/5.0 (Macintosh; Intel Mac OS X 10_15_2) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/79.0.3945.117 Safari\/537.36 Edg\/79.0.309.60",
            "insertedAt": {
                "__type": "Date",
                "iso": "2020-01-14T13:30:46.162Z"
            },
            "createdAt": "2020-01-14T13:30:46.284Z",
            "pid": "5e1dc1a5dd3c13006ae0d11e",
            "link": "",
            "comment": "<p><a class=\"at\" href=\"#5e1dc1a5dd3c13006ae0d11e\">@zc <\/a> , 666\u554a\ud83d\udc4d<\/p>\n",
            "url": "\/my-new-blog\/",
            "rid": "5e1dbf4f7796d9006a31b183",
            "isNotified": true
        },
    ],
    "className": "Comment"
}
```