# Euler angles
this script right here turns the sprite to the left when you press left arrow button \
```c
if(Input.GetKeyDown(KeyCode.LeftArrow)){
		 Time.deltaTime* 10);
			transform.eulerAngles=  new Vector3(
    			transform.eulerAngles.x,
    			transform.eulerAngles.y,
    			transform.eulerAngles.z+20
          );
        }
  ```
