# webView
- 자바스크립트를 실행하기위해서는 반듯시
```
javascriptMode: JavascriptMode.unrestricted
```
이 값을 주어야 실행이 된다.

- 전체 코드 예시
```
import 'package:flutter/material.dart';
import 'package:webview_flutter/webview_flutter.dart';

class HomeScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
        body: WebView(
      initialUrl: 'https://blog.codefactory.ai',
      javascriptMode: JavascriptMode.unrestricted,
    ));
  }
}


```