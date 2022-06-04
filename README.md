<!--- @VargasBarbeiro --->


<!---
VargasBarbeiro/VargasBarbeiro is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
// C++ code
//
byte cont = 0;
int const buzzer = 9;
void setup()
{
  Serial.begin(9600);
  pinMode(A0, INPUT);
  pinMode(A1, INPUT);
  pinMode(A2, INPUT);
  pinMode(A3, INPUT);
  pinMode(A4, INPUT);
  pinMode(A5, INPUT);
  pinMode(3, INPUT);
  pinMode(buzzer, OUTPUT);
}

void loop()
{ 
  Serial.println(cont);
  cont++;
  noTone(buzzer);
  if(digitalRead (A0) == HIGH) {
    tone(9, 264,10);
	}
  if(digitalRead (A1) == HIGH) {
    tone(9, 297,10);
	} 
  if(digitalRead (A2) == HIGH) {
    tone(9, 330);
	} 
  if(digitalRead (A3) == HIGH) {
    tone(9, 352);
	} 
  if(digitalRead (A4) == HIGH) {
    tone(9, 396);
	} 
  if(digitalRead (A5) == HIGH) {
    tone(9, 440, 100);
	} 
  if(digitalRead (3) == HIGH) {
    tone(9, 495, 100);
	}


    delay(10);
}
