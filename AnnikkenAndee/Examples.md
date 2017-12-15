# Examples

This section provides examples for your Andee shield. You can jump to the example that best suits your needs.

## Creating Widgets {#creating-widgets}

To create a new widget, you will need to instantiate a new instance of the AndeeHelper class as follows. The ideal place to place this would be just below your #includes declaration in your Arduino sketch.

```cpp
AndeeHelper widget1;
```

When creating a new widget, the most important properties that you need to set are:

1. **Unique ID**
2. **Screen location**
3. **Type**
4. **Colors**
5. **Display data**
 
Lets go through each of these properties.

1. **Unique ID**
To set the id:
```cpp
widget1.setId(0);
widget2.setId(1);
```
**Note:** The integer id for each widget should be unique and different. Declaring a widget as the same id as another will cause the latest widget to override the other.

2. **Screen Location**
You can set the location of your widget by one of two methods:
  * A row and column based system.
  The mobile devices is divided into 4 rows and 4 columns.
    ```cpp
    widget1.setLocation(1, 2, ONE_THIRD);
    ```
    For an in depth explanation on setLocation(), refer to this [documentation](/AnnikkenAndee/methods.md#setlocat)
  
  * Cartesian based system.
  This system is based on x and y coordinate with its origin at the top left corner, along with its height and width. 
  ```cpp
  widget1.setCoord(25, 25, 50, 25);
  ```
  For an in depth explanation on setCoord() refer to this [documentation](/AnnikkenAndee/methods.md#setcoord)

3. **Type**
The Andee library provides a few different types of UI. To see how the widgets look like, refer to [Andee U/iOS](https://annikkenconnect.com/andee-u) or [Andee Android](https://annikkenconnect.com/andee-android).
```cpp
widget1.setType(DATA_OUT);
```
For an in depth explanation on setType() and options for type, refer to this [documentation](/AnnikkenAndee/methods.md#settype)

4. **Colors**
Every component of the widget can be customised by color.
To set the color of the titles.
```cpp
widget1.setTitleTextColor("FFAEDE94");
```
To set the background color for title region.
```cpp
widget1.setTitleColor("FFFFDAAA");
```
To set body text color.
```cpp
widget1.setTextColor("FFFFDAAA");
```
To set body background color.
```cpp
widget1.setColor("FF6D92A0");
```

For an in depth explanation to set colours and predefined colors, refer to this [documentation](/AnnikkenAndee/methods.md#setcolor)







## Sending Data {#sending-data}




## Receiving Data {#receiving-data}



## Responding to Events {#responding-to-events}