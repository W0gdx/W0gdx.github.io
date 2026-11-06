# W0gdx.github.io

Chelsy 的个人网站。背景是一层实时渲染的雨落玻璃效果（WebGL），内容包括个人介绍、在做的 Android 应用 Silberth，以及过往参与宣发的电影项目。

网址：https://w0gdx.github.io

## 功能

- 雨落玻璃背景，右上角按钮可以调节雨量、速度、雾化、折射、亮度等参数
- 右上角面板里可以上传自己的图片或视频作为背景，只在本机浏览器里生效，不会上传到服务器
- 手机和电脑都能浏览

## 目录

```
index.html            页面内容、样式、SEO 信息
assets/
  index-*.js          雨落效果和设置面板（已编译的 React + three.js）
  posters/            电影海报
  shots/              Silberth 应用截图
```

## 本地预览

```sh
python3 -m http.server 8000
```

然后打开 http://localhost:8000 。直接双击 `index.html` 打不开雨落效果，需要通过本地服务器访问。

## 说明

- 页面依赖几个外部 CDN：Tailwind CSS、esm.sh（React、three.js）、Google Fonts。网络访问不到时，页面文字和图片仍会显示，雨落效果可能加载不出来。
- 电影海报版权归各片方所有，仅用于展示本人参与过宣发的项目。
- 雨落效果参考了 Shadertoy 上 BigWings 的作品 Heartfelt。
