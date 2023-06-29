# Welcome to the Tutorial
***In this tutorial, we will learn to make a simple counter app which has an increment button***
<br>
Given below is the code for the app. You can copy this code for testing or you can clone this [repo](SampleCode)
```
import 'package:flutter/material.dart';
void main() {
runApp(CounterApp());
}

class CounterApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Counter App',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: CounterPage(),
    );
  }
}

class CounterPage extends StatefulWidget {
  @override
  _CounterPageState createState() => _CounterPageState();
}

class _CounterPageState extends State<CounterPage> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Counter App'),
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Text(
              'Counter Value:',
              style: TextStyle(fontSize: 20),
            ),
            Text(
              '$_counter',
              style: TextStyle(fontSize: 40, fontWeight: FontWeight.bold),
            ),
          ],
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: _incrementCounter,
        tooltip: 'Increment',
        child: Icon(Icons.add),
      ),
    );
  }
}
```

**The app when run in chrome browser looks something like this.**
<br>
![App](https://github.com/aastha51551/TSS-2023/assets/134774307/8f27ac2a-91e3-4b31-b70e-8fedf409a984)

## Explanation

* `import 'package:flutter/material.dart';` imports the flutter material package.This contains all the widgets we can use in Flutter. Widgets are different components like appbars, buttons etc. that we can add to our app. We will learn more about widgets in the upcoming weeks.

*
```
class CounterApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Counter App',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: CounterPage(),
    );
  }
}
```
This Section gives a `title:` Counter App through title parameter and a blue coloured theme through `theme:` parameter.

*
```
 void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }
```
In this section we define a function(method) named `_incrementCounter` and inside that we call a `setState()` function which is used to update the internal state of the widget and trigger a rebuild of the widget's user interface.In simple words, this segment of code is responsible for incrementing the counter value `_counter++;` and updating the user interface accordingly.

*
```
return Scaffold(
      appBar: AppBar(
        title: Text('Counter App'),
```
In Flutter, `Scaffold` is a pre-built widget provided by the Flutter framework that serves as a basic structural layout for an application screen.Here, we create an appbar which is titled as Counter App.

*
```
 body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Text(
              'Counter Value:',
              style: TextStyle(fontSize: 20),
            ),
            Text(
              '$_counter',
              style: TextStyle(fontSize: 40, fontWeight: FontWeight.bold),
            
```
Here , We define the body of the app. We create a widget which is aligned to the center of the screen and has the text **Counter Value:**.In the same widget, we update the text according to our counter value using `'$_counter'`.

*
```
floatingActionButton: FloatingActionButton(
        onPressed: _incrementCounter,
        child: Icon(Icons.add),
```
The `floatingActionButton` is a named parameter of the Scaffold widget.Within the `floatingActionButton` parameter, a `FloatingActionButton` widget is created. The `FloatingActionButton` is a pre-defined widget in the Flutter framework that represents a circular material design button.` onPressed:` tells us that when the button is pressed the previously defined function `_incrementCounter()` is called.
<br>
`child` parameter specifies the child widget to be displayed inside the FloatingActionButton. Here, an `Icon` widget with the `Icons.add` icon is used . This displays a "+" symbol inside the floating action button.
> Note: This is just a basic tutorial to help you with your assignment.Concepts related to OOPs and widgets will be covered in detail later in the course.If you don't understand any particular segment of code that hasn't been covered in this tutorial, stay assured it will be covered later. 
