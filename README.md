# lfr502-slide
一个用原生JS实现的轮播图简易插件

## 快速开始

- npm

  git clone https://github.com/lvfangren/lfr502-slide.git
  cd  lfr502-slide
  npm run release //项目编译,具体见package.json文件
  npm run example //运行项目测试用例

- CDN http://unpkg.com/lfr502-slide/release/bundle.js

## 参数说明
调用方式
```
<script>
new LfrSlide({
  picwrap:'picwrap',
  prev:'prev',
  next:'next',
  number:5
})
</script>
```
test.html文件结构
```
<div id='wrap'>
  <div id='picwrap' style="left:0;">
    <img src='./assert/1.jpg'>
    <img src='./assert/2.jpg'>
    <img src='./assert/3.jpg'>
    <img src='./assert/4.jpg'>
    <img src='./assert/5.jpg'>
  </div>
  <span id='prev'>&lt;</span><span id='next'>&gt;</span>
  <div id='controls'>
    <span class='on' data-index='0'></span>
    <span data-index='1'></span>
    <span data-index='2'></span>
    <span data-index='3'></span>
    <span data-index='4'></span>
  </div>
</div>

```
### 必传参数：
  picwrap //图片父盒子ID
  prev  //上翻按钮ID
  next  //下翻按钮ID

### 选传参数：
  number  //轮播图片数量（轮播变换次数）
  clickSpan //鼠标点击图片下方小圆点能否发生图片切换,默认为true
  touchStop //鼠标移入图片时轮播是否发生暂停，默认为true
  moveTime //图片切换时间,默认为3000ms


## 问题交流

https://github.com/lvfangren/lfr502-slide/issues


## 关于作者
- [博客地址]
    https://blog.csdn.net/qq_36458054
