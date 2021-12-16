void setup(){
Serial.begin(9600);
pinMode(5,OUTPUT);
 }
 void loop(){
  int a= analogRead(A0);
  Serial.println(a);
  if(a>30)
  {
    digitalWrite(5,HIGH);
  }
  else
  {
     digitalWrite(5,LOW);
  }
  }
