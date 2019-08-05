# Game-code-snippets
## User input
#### Mouse input
`Input.GetMouseButtonDown(int param)`

The get GetMouseButtonDown checks if in this frame the mouse button has changed state from not-clicked to clicked
it takes integer values as parameters
0-left mouse button
2-right mouse button


`Input.GetMouseButton(int param)`
The get GetMouseButton checks if in this frame the mouse button in the clicked state
it takes integer values as parameters
0-left mouse button
2-right mouse button

`Input.GetMouseButtonUp(int param)`
The get GetMouseButtonUp checks if in this frame the mouse button has changed state from clicked to not-clicked\
**it takes integer values as parameters** \
0-left mouse button\
2-right mouse button\

Note:touches on android work as left mouse events

## Keyboard input

`Input.GetKeyDown(int param)`
The get GetKeyDown checks if in this frame the supplied key has changed state from not-clicked to clicked \
**It takes integer value as parameter**
key code of the given key is supplied in the class [KeyCode](https://docs.unity3d.com/ScriptReference/KeyCode.html)

`Input.GetKey(int param)`
The get GetKey checks if in this frame the supplied key is clicked
**It takes integer value as parameter**
key code of the given key is supplied in the class [KeyCode](https://docs.unity3d.com/ScriptReference/KeyCode.html)

`Input.GetKeyUp(int param)`
The get GetKeyUp checks if in this frame the supplied key has changed state from clicked to not-clicked \
**It takes integer value as parameter** \
key code of the given key is supplied in the class [KeyCode](https://docs.unity3d.com/ScriptReference/KeyCode.html)


##Player movement \
**Translate** \
[check out documentation](https://docs.unity3d.com/ScriptReference/Transform.Translate.html)

**Rotate**
Well you can use Quaternion for this but I personally find that method very messy.\
So I use euler-Angles instead \
[check example](./euler-angle-example.md)

**Triggers**
we can use triggers for many things. We used it to know what we are colliding with if it is a powerup or an enemy
