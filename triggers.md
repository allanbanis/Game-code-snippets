# Triggers
for these functions to be called the object that you add this code to needs to have rigidbody2D.
### onTriggerEnter2D(Collider2D col)

this function is called if in this frame we have just entered another collider with the collider that we entered as a parameter\
[documentation](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerEnter2D.html)
##### Example:
```c
private void OnTriggerEnter2D(Collider2D other) {
		if(other.gameObject.tag=="Enemy"){
          //destroy ourselves
          Destroy(gameObject);
          gameOver=true;

		}
		if(other.gameObject.tag=="powerup"){
          //destroy the object that collided with us
		   Destroy(other.gameObject);
		}
	}
```
### onTriggerStay2D(Collider2D col)
This function is called if in the current frame we are intersecting another collider with that collider as a parameter\
[documentation](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerStay2D.html)

#### onTriggerExit2D(Collider2D col)
this function is called if this frame we have just exited another collider with that collider as the parameter\
[documentation](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerExit2D.html)
