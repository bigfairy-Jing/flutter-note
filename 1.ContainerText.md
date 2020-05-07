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
        child: Text(
          "我是一个文本我是一个文本我是一个文本我是一个文本我是一个文本",
          // textAlign: TextAlign.center,
          textAlign: TextAlign.left,
          // overflow: TextOverflow.ellipsis,
          // overflow: TextOverflow.fade,
          // overflow: TextOverflow.clip,
          style: TextStyle(
              fontSize: 30.0,
              color: Colors.yellow,
              fontWeight: FontWeight.w800,
              fontStyle: FontStyle.italic,
              decoration: TextDecoration.lineThrough,
              decorationColor: Colors.white,
              decorationStyle: TextDecorationStyle.wavy,
              letterSpacing: 8.0),
        ),
        height: 300.0,
        width: 300.0,
        decoration: BoxDecoration(
            color: Colors.blue,
            border: Border.all(color: Colors.green, width: 2.0),
            borderRadius: BorderRadius.all(Radius.circular(8.0))),
        // padding: EdgeInsets.all(20.0),
        padding: EdgeInsets.fromLTRB(20.0,0,10.0,1.0),
        // transform: Matrix4.translationValues(50.0,0,0),
        transform: Matrix4.rotationZ(0.3),
        alignment: Alignment.bottomCenter,
      ),
    );
  }
}

```