# 围脖是个好图床



> 围脖是个好图床 用于解决互联网图片传播存储的问题。图片文件存储在渣浪围脖中。

> 因为之前 web 版本的因为种种限制，变成了浏览器插件版，现在想想浏览器插件还是有诸多不便（其实是自己不想维护了），于是开了这个新坑（我肯定可以坚持维护下去的...大雾）。

> 当前版本仅 macOS 系统可使用（因为朱一自己主要在 macOS 上干活）。之后也许大概可能会出一个叫做 weibotuchuang-lite 之类的平台通用版本。

![app@2x.png](http://wx3.sinaimg.cn/large/6e9ad2bdly1fczpngdr4yj20sg0sgwqc.jpg)

## 使用方式
![屏幕快照 2017-02-21 下午7.53.17.png](http://wx4.sinaimg.cn/large/6e9ad2bdly1fcyc5bztafj216c0kqhdt.jpg)

1. 通过将图片文件拖拽到 menubar 图标上。
2. 通过点击 menubar 图标，在菜单中选择 上传图片。
3. 如果图片文件在被复制到剪贴板中，可以通过点击 menubar 图标，在菜单中选择 从剪贴板上传。

## F&Q

__Q:__ 这个需要通过登录围脖才能使用，围脖账号会有被盗的危险么？

__A:__ 围脖是个好图床 会在登陆之后记录下登陆凭证 (cookie), 并且加密（虽然是加密，但是项目上 electron 的情况下，防君子不防小人 2333）保存在 `~/.weibotuchuang` 文件下。不会上传服务器。所以如果保证您的设备是安全的情况下，不会有被盗危险。如果你要把电脑转借他人请在 围脖是个好图床 中登出围脖，或者执行在 __终端__ 中执行 `rm ~/.weibotuchuang`。

__Q:__ 我上传的图片的列表我可以取到吗？

__A:__ 我会在用户本地保存最近10组上传记录。如果想获取更多的话，目前是没有其他手段可以获取到的。总结说，如果上传之后返回的地址如果丢了，没有其他手段可以找回图片地址。（如果你是围脖内部人士可以试试。）

__Q:__ 我的电脑是 windows，什么时候可以出 windows 版本。

__A:__ 也许大概可能下个月吧... > _ <

__Q:__ 为什么我打开应用时提示 __打开来自身份不明开发者的应用__, 并且不能启动

__A:__ 因为朱一没有给 apple 的开发者账号充钱..., 你可以在 __系统偏好设置 > 安全性与隐私 > 通用__ 下允许打开即可。(下次就不会弹出了)


## 反馈

有意见反馈可以在 [https://github.com/zythum/weibotuchuang-electron/issues](https://github.com/zythum/weibotuchuang-electron/issues) 提交。