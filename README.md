import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: MarginContainerDemo(),
 );
 }
}
class MarginContainerDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Container with Margin')),
 body: Center(
 child: Container(
 margin: EdgeInsets.all(20), // ⬅️ Adds space around the 
container
 color: Colors.lightBlue,
 height: 100,
 width: 200,
 child: Center(child: Text('With Margin')),
 ),
 ),
 );
 }
}
