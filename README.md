# Task1-Electronics

## Turn LED ON and OFF With Push Button

 ### Idea:
  Power on the LED when the button is pressed, and power off the LED when the button is not pressed.

 ### Hardware Required:
  - Arduino UNO.
  - Breadboard.
  - LED.
  - Push button.
  - 220 Ohm resistors.
  - male to male wires.

  ### Circuit:

  - When the button is not pressed:
 
      ![image](Circuit-1.png)
 
  - When the button is pressed:
    
      ![image](Circuit-1.1.png)


  ### Code:

```
int led=2;
int PushButton=5;
int button;

void setup()
{
  
  pinMode(led, OUTPUT);
  pinMode(PushButton, INPUT);
  Serial.begin(9600);
}

void loop()
{
  
  button=digitalRead(5);
  
  if(button==HIGH)
  {
    digitalWrite(led,HIGH);
    delay(3000);
  }
  else
  {
     digitalWrite(led,LOW);
  }
  
}
```
  ### Tinkercad link:

      https://www.tinkercad.com/things/dksbH09xmc7?sharecode=gaO8uukPS-zQfJDkhBOqCBr6Dx06qi3JcHrlQG23NlI




## 5x5 LED Matrix


