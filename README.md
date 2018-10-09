# Vue-Cli 初始化目录
> 移动端 Vue 项目基于 Cli 脚手架工具的初始化目录。

## 步骤
### 添加 viewport
在 `index.html` 中添加 `viewport` 。
```HTML
<meta name="viewport" content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no">
```

### 添加 reset.css
将 `reset.css` 文件放置到项目目录的 `assets` 下的 `styles` 中。并在 `main.js` 入口文件中引入。
```JavaScript
import './assets/styles/reset.css'
```

[`reset.css` 下载地址](https://evenyao-1257191344.cos.ap-chengdu.myqcloud.com/reset.css)


### 添加 border.css
解决移动端 `1px` 边框的问题。将 `border.css` 文件放置到项目目录的 `assets` 下的 `styles` 中。并在 `main.js` 入口文件中引入。
```JavaScript
import './assets/styles/border.css'
```

[`border.css` 下载地址](https://evenyao-1257191344.cos.ap-chengdu.myqcloud.com/border.css)


### fastclick
使用 `fastclick` 解决移动端 `click` 事件 `300ms` 延迟。重启服务后，在 `main.js` 入口文件中引入 `fastclick`。
```
npm install fastclick --save
```
![](https://upload-images.jianshu.io/upload_images/12904618-c224dee3d1b5c39c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

重启服务后，在 `main.js` 入口文件中引入 `fastclick`，并在 `document.body` 之上使用 `fastClick.attach`。这样就使用了 `fastclick`。

![](https://upload-images.jianshu.io/upload_images/12904618-a7aca00b31b7b290.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
