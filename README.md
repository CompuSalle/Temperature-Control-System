# Temperature Control System Between Two Offices Using Cisco Packet Tracer 


### Before Using Please Refer To [LICENSE](https://github.com/WassemAdil/Network-System-Simulation/blob/main/LICENSE)

-----------------------
Use the original Cisco Packet Tracer Program From [Cisco](https://www.netacad.com/courses/packet-tracer)

You can find a go-through video step-by-step on my youtube channel in [here](https://www.youtube.com/watch?v=qICKNQ1g1wg)

------------------------------------------------------

>Programe Screenshot

![Screenshot](https://github.com/WassemAdil/Temperature-Control-System/blob/main/Program_Screenshot.png)

----------------------------------------------

> The used python script

**Inside MCU |main.py**

```
from gpio import *
from time import *

def inputHandler():
 
    value = (((analogRead(A0) - 0 ) * (100 - -100)) / (1023 - 0)) +  -100
    customWrite(0,value)
    
def main():
    add_event_detect(A0, inputHandler)

    while True:
        delay(1)

if _name_ == "__main__":
    main()
  on work
  
```


