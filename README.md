# flutter_application_1

## Chapter 2: Container, Scaffold and Text Widgets

1. Container is a like a box which can be customized
2. Cannot provide both a color and a decoration
   1. To provide both, use "decoration: BoxDecoration(color: color)".)

### Properties of Container Object

1. **Child**: Container can have only 1 child
2. **Color**: Sets background color of the entire container
3. **Height and Width**: By default a container takes the height and width required by the child. We can also set it in units.

```dart
height: 200,
width: double.infinity,
```

4. **Margin**: EdgeInsets.geometry is used to set the margin (empty space around the container)
5. **Padding**: EdgeInsets.geometry is used to set the padding (space between the border of the container and its child)
6. **Alignment**: To position the child within the container. Alignment.location is used to place the child inside the container
7. **Decoration**: decoration paints behind the child.
8. **foregroundDecoration** paints in front of a child

```dart
decoration: BoxDecoration(
            border: Border.all(color: Colors.black, width: 3),
          ),
```

9. **Transform** : helps us to rotate the container in any axis

```dart
transform: Matrix4.rotationZ(0.1),
```

10. **Other Options**: constraints and clipBehavior

### Properties of Scaffold Object

**Items provided by Scaffold class:**

- AppBar, Body, Drawer, SnackBar, BottomNavigationBar, BottomSheet, FloatingActionButton, etc.
- Scaffold will expand or occupy the whole device screen

1.  **AppBar**: Horizontal bar which mainly placed at the top of the Scaffold.
2.  **Body**: It will display the main or primary content in the Scaffold. It is below the appBar and under the floatingActionButton.

```dart
return Scaffold(
     appBar: AppBar(title: const Text('GeeksforGeeks')),
     body: const Center(
       child: Text(
         "Welcome to GeeksforGeeks!!!",
         style: TextStyle(
           color: Colors.black,
           fontSize: 40.0,
         ),
       ),
     ),
   );
```

3. **floatingActionButton**: FloatingActionButton is an icon button that floats over the content of the screen at a fixed place.

```dart
floatingActionButton: FloatingActionButton(
      elevation: 10.0,
      child: const Icon(Icons.add),
      onPressed: () {
        // action on button press
      },
    ),
```

4. **drawer**: drawer is sidebar opened by swipe or hamburger menu
5. **bottomNavigationBar**: bottomNavigationBar menu bar at the bottom of the Scaffold.
   1. _fixedColor_: color of active icon
   2. _BottomNavigationBarItems_: To add items in the bar
   3. _onTap(int indexOfItem)_: on tap action based on index of item

```dart
bottomNavigationBar: BottomNavigationBar(
        currentIndex: 0,
        fixedColor: Colors.green,
        items: const [
          BottomNavigationBarItem(
            label: "Home",
            icon: Icon(Icons.home),
          ),
          BottomNavigationBarItem(
            label: "Search",
            icon: Icon(Icons.search),
          ),
          BottomNavigationBarItem(
            label: "Profile",
            icon: Icon(Icons.account_circle),
          ),
        ],
        onTap: (int indexOfItem) {}),
```

6. **backgroundColor**: to set the color of the whole Scaffold widget.
7. **bottomSheet**: It takes in a widget as the object to display it at the bottom of the screen.

## Demo screen:

<img src="https://res.cloudinary.com/dhamikauser/image/upload/v1659354525/flutter-tut-demo/sim-screen-2_shifsl.png" alt="demo screen" width="200" />
