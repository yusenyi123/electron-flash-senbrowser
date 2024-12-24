# 介绍
因为flash的安全性等问题，很多浏览器都不再支持flash。比如chrome，自 2021 年起，Adobe 已停止为 Flash Player 插件提供支持。[在任何版本的 Chrome 中，Flash 内容（包括音频和视频）都将无法再正常播放](https://www.blog.google/products/chrome/saying-goodbye-flash-chrome/)。

因此，在 Electron 里，使用 Pepper Flash 插件加载钟爱的flash小游戏，以供随时娱乐^ ^。
而electron的跨平台属性,可以让我们在多个平台都能畅玩flash游戏,安卓手机使用proot的方式装上一个linux的gui容器就可以运行该应用玩flash游戏
注意：
 - 版本：chromium从v88后，彻底地禁止使用flash。项目中的`electron`版本为`^11.4.7`，chromium版本为`87.0.4280.141`。
 - 自定义：可以在`plugins`下替换你本机的pepeflashplayer插件，也可以替换你想播放的flash！
 - 测试：在win10, macOS Catalina 10.15.5加载成功。macOS Big Sur版本11.3.1加载插件失败,proot容器下的armhf和arm64的系统均可运行



# 命令
安装依赖
``` bash
npm install
```

开发模式
``` bash
npm start
```

使用 Forge 的 `make` 命令来创建可分发的应用程序。运行结果在`out`目录下
``` bash
npm run make
```
