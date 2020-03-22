# Flutter tutorial by the Net Ninja
Here you can find my documentation about what I have learned from the flutter tutorial.

>_To see the full tutorial playlist [click](https://www.youtube.com/watch?v=1ukSR1GRtMU&list=PL4cUxeGkcC9jLYyp2Aoh6hcWuxFDX6PBJ&index=1)_

## Everything is an Widged
When you hear that everything in flutter is an Widget, it litteraly means everything is an widged. Almost everything that you need is an widged. Even text and centering stuff is an widged on itself.

## Widged List
### MaterialApp
Allows us to use the Material design through out our application. This widged has the home property which defines what the user  sees when he/she opends the app. Aka home screen.
```dart
void main() => runApp(MaterialApp(
  home: Scaffold(),
));
```
### Scaffold
Scaffold is one the most commonly used widged. It is used to make your base layout for your app. The Scaffold widged gots a multiple of diffrent property's like appBar for the top navigation.
```dart
void main() => runApp(MaterialApp(
  home: Scaffold(
    appBar: AppBar(
      title: Text('Hello'),
      centerTitle: true,
    ),
  ),

));
```
