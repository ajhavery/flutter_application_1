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

## Demo screen:

<img src="https://res.cloudinary.com/dhamikauser/image/upload/v1659354525/flutter-tut-demo/sim-screen-2_shifsl.png" alt="demo screen" width="200" />
