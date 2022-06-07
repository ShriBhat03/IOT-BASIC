=>3 Bulb</br>
https://wokwi.com/projects/333796932630610515</br>
void setup() {</br>
  pinMode(13,OUTPUT);</br>
  pinMode(12, OUTPUT);</br>
  pinMode(11, OUTPUT);</br>
}</br>

void loop() {</br>
  digitalWrite(13, HIGH);</br>
  delay(1000);</br>
  digitalWrite(13, LOW);</br>
  delay(50);</br>
digitalWrite(12, HIGH);</br>
  delay(1000);</br>
  digitalWrite(12, LOW);</br>
  delay(50);</br>
digitalWrite(11, HIGH);</br>
  delay(1000);</br>
  digitalWrite(11, LOW);</br>
  delay(50);</br>
}</br>

=>RGB LED</br>
https://wokwi.com/projects/333801500788654674

int red_light_pin= A5;
int green_light_pin = A4;
int blue_light_pin = A3;
void setup() {
  pinMode(red_light_pin, OUTPUT);
  pinMode(green_light_pin, OUTPUT);
  pinMode(blue_light_pin, OUTPUT);
}
void loop() {

  
  RGB_color(0, 255, 255); // Red
  delay(200);
  
 // RGB_color(0, 0, 255); //yellow
 // delay(100);
  RGB_color(255,255, 0); // Green
 delay(200);
 //RGB_color(255, 255, 255); // Red
 // delay(100);
 
}
void RGB_color(int red_light_value, int green_light_value, int blue_light_value)
 {
  analogWrite(red_light_pin, red_light_value);
  analogWrite(green_light_pin, green_light_value);
  analogWrite(blue_light_pin, blue_light_value);
}
