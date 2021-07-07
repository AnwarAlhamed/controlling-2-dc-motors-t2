# controlling-2-dc-motors-t2
## Designing and Programing 2 dc motors circuit.
### The circuit design 
The circuit contains:

- Arduino UNO.
- Breadboard.
- 2 DC motors.
- 9V battery.
- Wires ( red= power , black= ground , yellow and green = signal).
 
and the circuit was designed using tinkercad website as below:
#### Diagram preview:
![controlling 2 DC motors (1)](https://user-images.githubusercontent.com/86317095/124780496-52d27e80-df4b-11eb-8e88-96e9d51cd091.png)
### Programing 2 dc motors to move clockwise and counterclockwise:
 The circuit was programmed using the C++ language via the Tinkercad website as shown in ino file in this repository.
  #### Code Explanation:
  ```
  //controlling 2 DC-motors
int pot=A0 ;
int value ;

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
  digitalWrite(7, LOW);
  digitalWrite(6, HIGH);
  digitalWrite(5, LOW);
  digitalWrite(4, HIGH);
  delay(3000); // Wait for 3 seconds
 
  //moving counterclockwise
  digitalWrite(7, HIGH);
  digitalWrite(6, LOW);
  digitalWrite(5, HIGH);
  digitalWrite(4, LOW);
  delay(3000); // Wait for 3 seconds
  
}
```
 ### For simulation:
 - [Press here ](https://www.tinkercad.com/things/fcfQ0BxayjX-controlling-2-dc-motors)
