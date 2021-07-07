# 绯月 hosts

## 一、介绍

解决绯月日常炸裂（dns污染）的问题

若为主机ip被墙，那么只能请大家富强上网了（笑
## 二、使用方法

### 2.1 复制下面的内容
```bash
# 绯月 Host Start
173.230.157.235               bbs.kforz.com
173.230.157.235               bbs.bakabbs.com
172.104.110.220               bbs.365gal.com
172.105.52.107                bbs.365galgame.com
# Star me GitHub url:https://github.com/Ecalose/fyhosts
# 绯月 Host End

```

上面内容会自动定时更新，保证最新有效。数据更新时间：2021-07-08T06:12:34+08:00（内容无变动不会更新）

### 2.1 手动方式
#### 2.1.1 修改 hosts 文件
hosts 文件在每个系统的位置不一，详情如下：
- Windows 系统：`C:\Windows\System32\drivers\etc\hosts`
- Linux 系统：`/etc/hosts`
- Mac（苹果电脑）系统：`/etc/hosts`
- Android（安卓）系统：`/system/etc/hosts`
- iPhone（iOS）系统：`/etc/hosts`

修改方法，把第一步的内容复制到文本末尾：

1. Windows 使用记事本。
2. Linux、Mac 使用 Root 权限：`sudo vi /etc/hosts`。
3. iPhone、iPad 须越狱、Android 必须要 root。

#### 2.1.2 激活生效
大部分情况下是直接生效，如未生效可尝试下面的办法，刷新 DNS：

1. Windows：在 CMD 窗口输入：`ipconfig /flushdns`

2. Linux 命令：`sudo rcnscd restart`

3. Mac 命令：`sudo killall -HUP mDNSResponder`

**Tips：** 上述方法无效可以尝试重启机器。

### 2.2 自动方式

**Tip**：推荐 [SwitchHosts](https://github.com/oldj/SwitchHosts) 工具管理 hosts

以 SwitchHosts 为例，看一下怎么使用的，配置参考下面：

- Title: 随意

- Type: `Remote`
- URL: `https://raw.fastgit.org/Ecalose/fyhosts/master/hosts`(fastgit加速)
       `https://gh.haval.gq/Ecalose/fyhosts/raw/master/hosts`(cloudflare加速)
        
        (二者任选其一即可）
- Auto Refresh: 最好选`1hour`

如图：

![](./img/switch-hosts.png)

这样每次 hosts 有更新都能及时进行更新，免去手动更新。

### 2.3 AdGuard Home 用户（自动方式）

在 **过滤器>DNS 封锁清单>添加阻止列表>添加一个自定义列表**，配置如下：

- 名称: 随意

- URL: `https://raw.fastgit.org/Ecalose/fyhosts/master/hosts`(fastgit加速)
       `https://gh.haval.gq/Ecalose/fyhosts/raw/master/hosts`(cloudflare加速)
       
       (二者任选其一即可）

如图：

![](./img/AdGuard-rules.png)

更新间隔在 **设置>常规设置>过滤器更新间隔（设置一小时一次即可）**，记得勾选上 **使用过滤器和 Hosts 文件以拦截指定域名**

![](./img/AdGuard-rules2.png)

**Tip**：不要添加在 **DNS 允许清单** 内，只能添加在 **DNS 封锁清单** 才管用。另外，AdGuard for Mac、AdGuard for Windows、AdGuard for Android、AdGuard for IOS 等等 **AdGuard 家族软件** 添加方法均类似。



## 声明
<a rel="license" href="https://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh"><img alt="知识共享许可协议" style="border-width: 0" src="https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png"></a><br>本作品采用 <a rel="license" href="https://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh">署名-非商业性使用-禁止演绎 4.0 国际</a> 进行许可。
