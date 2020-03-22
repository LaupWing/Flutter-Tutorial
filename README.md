# Flutter tutorial by the Net Ninja
Here you can find my documentation about what I have learned from the flutter tutorial.

>_To see the full tutorial playlist [click](https://www.youtube.com/watch?v=1ukSR1GRtMU&list=PL4cUxeGkcC9jLYyp2Aoh6hcWuxFDX6PBJ&index=1)_

## Everything is an widget
When you hear that everything in flutter is an Widget, it litteraly means everything is an widget. Almost everything that you need is an widget. Even text and centering stuff is an widget on itself.

## Styling in Flutter
To style in flutter you need to add a new property to the Widget you want to update. 
Most of the styling properties in flutter are premade Objects. So if you want to update the colors of one widget you need to use the `Colors` object with an color extension.
```dart
body: Center(
    child: Text(
        'Hello World',
        style: TextStyle(
            color: Colors.grey[600],
        )  
    ),
    )
```
### Custom font size 
To add your custom font-size you need to go to your `pubspec.yaml` file. You need uncomment the font part on the bottom part of this file and fill in your own information (you already need an directory fonts with your custom font). **_NOTE: The spaces need to be exactly the same otherwist it will throw an error_** 
```dart
body: Center(
    child: Text(
        'Hello World',
        style: TextStyle(
            color: Colors.grey[600],
            fontFamily: 'IndieFlower', // This is the font name you have specified
        )  
    ),
)
```

## widget List
### MaterialApp
Allows us to use the Material design through out our application. This widget has the home property which defines what the user  sees when he/she opends the app. Aka home screen.
```dart
void main() => runApp(MaterialApp(
  home: Scaffold(),
));
```
### Scaffold
Scaffold is one the most commonly used widget. It is used to make your base layout for your app. The Scaffold widget gots a multiple of diffrent property's like appBar for the top navigation.
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
