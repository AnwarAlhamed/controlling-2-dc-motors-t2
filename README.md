# controlling-2-dc-motors-t2
## Designing and Programing 2 dc motors circuit.
### The circuit design 
The circuit contains:

- Arduino UNO.
- Breadboard.
- 2 DC motors.
- H-bridge (L293D).
- potentiometer.
- 9V battery.
- Wires ( red= power , black= ground , yellow and green = signal).
 
and the circuit was designed using tinkercad website as below:
#### Diagram preview:
![controlling 2 DC motors (4)](https://user-images.githubusercontent.com/86317095/124801421-7f909100-df5f-11eb-94e3-264953019960.png)

### Programing 2 dc motors to move clockwise and counterclockwise:
 The circuit was programmed using the C++ language via the Tinkercad website as shown in ino file in this repository.
  #### Code Explanation:
  ```
//controlling 2 DC-motors


void setup()
{
  pinMode(7, OUTPUT);
  pinMode(6, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(4, OUTPUT);
}

void loop()
{
 // moving clockwise
  if (analogRead(A0)>600)
  {
  digitalWrite(7, LOW);
  digitalWrite(6, HIGH);
  digitalWrite(5, LOW);
  digitalWrite(4, HIGH);
  }
  
 
  //moving counterclockwise
  if (analogRead(A0)<400)
  {
  digitalWrite(7, HIGH);
  digitalWrite(6, LOW);
  digitalWrite(5, HIGH);
  digitalWrite(4, LOW);
  }
  
  digitalWrite(7,LOW);
  digitalWrite(6, LOW);
  digitalWrite(5, LOW);
  digitalWrite(4, LOW);
}
```
 ### For simulation:
 - [Press here ](https://www.tinkercad.com/things/fcfQ0BxayjX-controlling-2-dc-motors)
