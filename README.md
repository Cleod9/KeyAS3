# Key.as Util for AS3#

This Key class for AS3 enables AS2-styled keyboard event behavior through a single static class. Simply call Key.init() once to initialize the class, and from there you can use `Key.beginCapture()` and `Key.endCapture()` to start and end the keyboard event listeners respectively. Also included in this class are all of the Flash key code values so you don't have to look them up.

### Minimum required classes for using this utility: ###

- com.mcleodgaming.util.Key

## Instructions ##

Copy the included **com** folder to your project's root code directory, and add the import to the top of your classes that will be using it:

```as3
import com.mcleodgaming.util.Key;
```

Then initiate the class in your code (only needs to be done once)

```as3
Key.init();
```

Once initiated, you are then able to use the following functions:

`Key.beginCapture(targetObject:DisplayObject):void` - Begins capturing keyboard  input based on the focus of the provided target DisplayObject. Supply the SWF `stage` object for global capture.

`Key.endCapture():void` - Stops keyboard input capture.

`Key.isDown(keyCode:int):Boolean` - Returns `true` if the supplied key code is pressed, or `false` otherwise. All of the Key codes can be accessed as static constants directly through the `Key` class.

## Terms of Use ##

Free to use in any projects without notifying me, nor is credit needed (though it'd be much appreciated!). Just do not re-distribute it under anyone else's name and be sure to retain the copyright notice in the source!

 
----------

Copyrighted © 2013 by Greg McLeod

GitHub: [https://github.com/cleod9](https://github.com/cleod9)