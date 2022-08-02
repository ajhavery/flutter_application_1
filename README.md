# flutter_application_1

## Main project folder - lib/main.dart

1. main.dart - has main() function which runs runApp() method
2. Demo screen of intro to Scaffold, Theme and Container

## Material App

1. **title**: one-line description of the app for the device.
2. **theme**: property takes in ThemeData class as the object to describe the theme for the MaterialApp.
3. **darkTheme**: theme data for the dark theme for the application.
4. **color**: controls the primary color used in the application.
5. **supportedLocales**: keeps hold of the locals used in the app by taking in Iterable<E> class as the object.
6. **debugShowCheckedModeBanner**: boolean as the object to decide whether to show the debug banner or not.
7. **home**: property takes in widget as the object to show on the default route of the app.

```dart
class GFGapp extends StatelessWidget {
  const GFGapp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'MyApp',
      theme: ThemeData(primarySwatch: Colors.blue),
      darkTheme: ThemeData(primarySwatch: Colors.grey),
      color: Colors.amberAccent,
      supportedLocales: {const Locale('en', ' ')},
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(title: const Text('GeeksforGeeks')),
      ),
    );
  }
}
```

## Functions:

1. **main() function**: statements written inside main function are executed when the app starts. The return type of main function is ‘void’.
2. **runApp(Widget widget) function**: It takes a widget and sets it as the root widget of the app and other widgets as the child of it. It gives the constraints to the widget to fit into the screen.

![demo screen](https://github.com/ajhavery/flutter_application_1/blob/dev%23ch1/demo/sim_screen_1.png?raw=true)
