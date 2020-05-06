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
        body: Center(
          child: Text("你好"),
        ),
      ),
    );
  }
}
```