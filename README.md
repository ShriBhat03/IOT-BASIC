# 1)=>3 Bulb</br>
https://wokwi.com/projects/333796932630610515</br>


# 2)=>RGB LED</br>
https://wokwi.com/projects/333801500788654674</br>

# 3)=>hello world</br>
https://wokwi.com/projects/333806219693130324</br>

# 4)=>UltraSonic SENSOR</br>
https://wokwi.com/projects/334344881532043858</br>

# 5)=>PIR SENSOR</br>
https://wokwi.com/projects/334346049182237266</br>

# 6)=>IR SENSOR</br>
https://wokwi.com/projects/334346772804534867</br>

# 7)=>TEMP SENSOR</br>
https://wokwi.com/projects/334346714953548371</br>

# 8)=>Button LED</br>
https://wokwi.com/projects/334430962204017236</br>

# 9)=> Button Fade</br>
https://wokwi.com/projects/334431341587202643</br>

# 10)=>  Motion Sensor</br>
 https://wokwi.com/projects/334431854492910163</br>

# 11)=>Motion Sensor Buzzer </br>
https://wokwi.com/projects/334433831716127314</br>

# 12)=>Ultra Sonic sensor LED</br>
https://wokwi.com/projects/334434440478458452 </br>

# 13=>Servo motor</br>
https://wokwi.com/projects/334975025852449363</br>

# 14=>Servo motor controlled by potentiometer</br>
https://wokwi.com/projects/334978058200023635</br>

# 15=>Servo motor controlled by button</br>
https://wokwi.com/projects/334977135889351250</br>

# 16=>Ultra sonic sensor with both LED and Buzzer</br>
https://wokwi.com/projects/335610620425536082</br>

# 17=> NodeMCU ultrasonic</br>
const int trigPin = 12;</br>
const int echoPin = 14;</br>

//define sound velocity in cm/uS</br>
#define SOUND_VELOCITY 0.034</br>
#define CM_TO_INCH 0.393701</br>
</br>
long duration;</br>
float distanceCm;</br>
float distanceInch;</br>
</br>
void setup() {</br>
  Serial.begin(115200); // Starts the serial communication</br>
  pinMode(trigPin, OUTPUT); // Sets the trigPin as an Output</br>
  pinMode(echoPin, INPUT); // Sets the echoPin as an Input</br>
}</br>
</br>
void loop() {</br>
  // Clears the trigPin</br>
  digitalWrite(trigPin, LOW);</br>
  delayMicroseconds(2);</br>
  // Sets the trigPin on HIGH state for 10 micro seconds</br>
  digitalWrite(trigPin, HIGH);</br>
  delayMicroseconds(10);</br>
  digitalWrite(trigPin, LOW);</br>
  </br>
  // Reads the echoPin, returns the sound wave travel time in microseconds</br>
  duration = pulseIn(echoPin, HIGH);</br>
  </br>
  // Calculate the distance</br>
  distanceCm = duration * SOUND_VELOCITY/2;</br>
  </br>
  // Convert to inches</br>
  distanceInch = distanceCm * CM_TO_INCH;</br>
  </br>
  // Prints the distance on the Serial Monitor
  Serial.print("Distance (cm): ");</br>
  Serial.println(distanceCm);</br>
  Serial.print("Distance (inch): ");</br>
  Serial.println(distanceInch);</br>
  </br>
  delay(1000);</br>
}</br>
___+_______+_____________+______________+___________________</br>

