
# LM35
--------------------
In this repo we want to work with a temperature sensor with `lm35 code`
I hope these imformation help you ;)
## Components
* bread board
* wire
* LM35 sensor
### Circuit 
![Circut ](https://roboeq.ir/blog/wp-content/uploads/2022/01/wiring-lm35-to-ardoino-1.png)
## Prerequisite
* Arduino IDE or Editor 
* Arduino board `nano or uno`
* upload cable
## Run locally
1. make the circuit
2. open Arduino Ide or editor
3. paste this code in it:
  ```
  // Define the analog pin, the LM35's Vout pin is connected to
  #define sensorPin A0
 
  void setup() {
  // Begin serial communication at 9600 baud rate
  Serial.begin(9600);
  }
 
  void loop() {
  // Get the voltage reading from the LM35
  int reading = analogRead(sensorPin);
 
  // Convert that reading into voltage
  float voltage = reading * (5.0 / 1024.0);
 
  // Convert the voltage into the temperature in Celsius
  float temperatureC = voltage * 100;
 
  // Print the temperature in Celsius
  Serial.print("Temperature: ");
  Serial.print(temperatureC);
  Serial.print("\xC2\xB0"); // shows degree symbol
  Serial.print("C  |  ");
   
  // Print the temperature in Fahrenheit
  float temperatureF = (temperatureC * 9.0 / 5.0) + 32.0;
  Serial.print(temperatureF);
  Serial.print("\xC2\xB0"); // shows degree symbol
  Serial.println("F");
 
  delay(1000); // wait a second between readings
  }
  ```
4. And done, now run it.
## About author 
this program was written by nime mirvahabi, you can contact me by:
mirvahabinima@gmail.com
# license 
this project is under [this](https://roboeq.ir/blog/%d8%a2%d9%85%d9%88%d8%b2%d8%b4-%d8%b1%d8%a7%d9%87-%d8%a7%d9%86%d8%af%d8%a7%d8%b2%db%8c-%d8%b3%d9%86%d8%b3%d9%88%d8%b1-%d8%af%d9%85%d8%a7-lm35-%d8%a8%d8%a7-%d8%a2%d8%b1%d8%af%d9%88%db%8c%d9%86%d9%88/) link 
