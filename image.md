```dart
import 'package:flutter/material.dart';

void main(List<String> args) {
  // runApp flutter 入口方法
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    // MaterialApp 一般作为根组件
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("小爱同学"),
          centerTitle: true,
        ),
        body: HomeContent(),
      ),
    );
  }
}

class HomeContent extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return Center(
        child: Container(
      child: Container(
        width: 300.0,
        height: 300.0,
        decoration: BoxDecoration(
            color: Colors.yellow,
            borderRadius: BorderRadius.circular(150.0),
            // image: DecorationImage(
            //     image: NetworkImage(
            //         'https://www.baidu.com/img/baidu_jgylogo3.gif'),
            //     fit: BoxFit.cover)
            ),
        // 加载远程图片
        // child: Image.network('https://www.baidu.com/img/baidu_jgylogo3.gif',
        //   fit: BoxFit.fitWidth,
        //   repeat: ImageRepeat.repeatY,
        //   // alignment: Alignment.topRight,
        //   color: Colors.blue,
        //   colorBlendMode: BlendMode.screen,
        // )

        // 圆角
      ),
    ));
  }
}

```

```dart
import 'package:flutter/material.dart';

void main(List<String> args) {
  // runApp flutter 入口方法
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    // MaterialApp 一般作为根组件
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("小爱同学"),
          centerTitle: true,
        ),
        body: HomeContent(),
      ),
    );
  }
}

class HomeContent extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return Center(
        child: Container(
      child: ClipOval(
        child: Image.network(
            "https://dss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=516794689,2676638222&fm=179&app=42&f=JPEG?w=67&h=75&s=162265A0DA5325FF9E90FD030300F0D1"),
      ),
    ));
  }
}

```

```dart
Image.asset("images/a.jpeg");
```