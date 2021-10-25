# scale_tabbar

* 缓解tab切换文字抖动问题 
* 添加双击事件(不推荐使用) 
* 默认去除点击水波纹 
* 可自定义水波纹颜色和圆角 
* 与官方TabBar使用方法相同 

使用方法
```dart
//simple example

ScaleTabBar(
    tabs: _tabs,
    onTabChanged: (int? index) => print('change to $index'),

    ///TODO 添加双击事件会导致[onTap]响应延时,不推荐使用
    // onDoubleTap: (int index) {
    //   Scaffold.of(context).showSnackBar(
    //     SnackBar(content: Text('Double tap : $index')),
    //   );
    // },

    labelColor: Colors.black,
    labelStyle: const TextStyle(fontSize: 30),
    unselectedLabelStyle: const TextStyle(fontSize: 15),

    //波纹属性
    splashColor: Colors.blue,
    highlightColor: Colors.redAccent,
    borderRadius: BorderRadius.circular(10),
)

```


## 效果预览

预览网址:[https://scaletabbar.liugl.cn](https://scaletabbar.liugl.cn)

<img src="https://raw.githubusercontent.com/xSILENCEx/flutter_scale_tabbar/master/preview/preview.gif" height=400>
