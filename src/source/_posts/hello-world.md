---
title: Hello World
id: hello-world
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

# 标题

## Quick Start

### Test

```cpp
#include <iostream>
using namespace std;

const int mod = 10008;
const int maxn = 1e5 + 5;
int a[maxn];
long long dp[maxn][10];

int main(int argc, char const *argv[])
{
    int T;
    cin >> T;
    while (T--)
    {
        string s;
        cin >> s;
        int len = s.length();
        memset(dp, 0, sizeof(dp));
        for (size_t i = 0; i < len; i++)
        {
            a[i] = s[i] - '0';
            if (a[i] % 2 == 1)
            {
                dp[i + 1][2] += 1;
            }
            if (a[i] % 4 == 0)
            {
                dp[i + 1][0] += 1;
            }
        }
        long long sum = 0;
        for (size_t i = 0; i < len; i++)
        {
            if(a[i]==4||a[i]==8)
            {
                sum+=i+1;
            }
            else if(a[i]==2)
            {
                if(dp[i][2]==1)
                {
                    sum+=i;
                }
            }
            else if(a[i]==0)
            {
                if(dp[i][0]==1)
                {
                    sum+=i;
                }
                sum+=1;
            }
            sum%=mod;
        }
        cout<<sum<<endl;
    }
    return 0;
}

```

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
