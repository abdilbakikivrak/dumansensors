int kirmizi=10; 
int yesil=9; 
int buzzer=8; 
int sensor=A0;
int referans=400; 

void setup (){
  pinMode(kirmizi,OUTPUT); 
  pinMode(yesil,OUTPUT); 
  pinMode(buzzer,OUTPUT); 
  pinMode(sensor,INPUT); 
  Serial.begin(9600); 
}

void loop (){
  int deger=analogRead(sensor); 
  Serial.print("MQ-2 okunan analog değer");
  Serial.println(deger); 

  if(deger>referans){ 
    digitalWrite (kirmizi,HIGH); 
    digitalWrite (yesil,LOW);
    digitalWrite (buzzer,800); 
  }

  else{
    digitalWrite (kirmizi,LOW); 
    digitalWrite (yesil,HIGH); 
    noTone(buzzer); 
  }

  delay(1000); 
}
