# Design-a-luminous-intensity-meter-such-that-light-intensity-falling-on-LDR-is-sensed-and-displayed-
beee-evaluation
 AIM:- To Design a luminous intensity meter, such that light intensity falling on LDR is sensed and displayed on the serial monitor upon the press of a switch.
 
 
 Apparatus:-connecting wires,arduino,LDR sensor,resistor,led.
 
 
 CODE:- 
 
 int sensorPin=A0;
 
 
 int ledPin=3;
 
 int sensorValue=0;
 
 void setup()
 
 {
 
 Serial.begin(9600);
 
 pinMode(3,OUTPUT);
 
 }
 
 void loop()
 
 {
 
 
 sensorValue=analogRead(A0);
 
 
 Serial.println(sensorValue);
 
 
 delay(100);
 
 
 if(sensorValue>300)
 
 {
 
 digitalWrite(3,HIGH);
 
 }
 
 
 else
 
 
 {
 
 
 digitalWrite(3,LOW);
 
 
 }
 
 
 
 RESULT:Designed a luminous intensity meter, such that light intensity falling on LDR is sensed and displayed on the serial monitor upon the press of a switch.
 
 
 PRECAUTION:-
 
 1. Connection should be proper.
 
 2.Check whether led is working or not.
 
 
 SOURCES OF ERROR:- 1.LED is not working.
 
 2.power supply is not proper.
 
 3.LDR is not working.
 
 
 
 
