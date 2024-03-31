source code for this project is 


/* made by Asish Samal*/
int but1=2;
int but2=3;
int but3=4;
int but4=5;
int but5=6;
int but6=7;
int but7=8;
int but8=9;

int buzzer =13;
void setup()
{
  // lets declare the button pins as input
  pinMode(but1,INPUT);
  pinMode(but2,INPUT);
  pinMode(but3,INPUT);
  pinMode(but4,INPUT);
  pinMode(but5,INPUT);
  pinMode(but6,INPUT);
  pinMode(but7,INPUT);
  pinMode(but8,INPUT);
  // buzzer pin as output
  pinMode(buzzer,OUTPUT);
}
void loop()
{
 //read the values from the button
  int button1=digitalRead(but1);
  int button2=digitalRead(but2);
  int button3=digitalRead(but3);
  int button4=digitalRead(but4);
  int button5=digitalRead(but5);
  int button6=digitalRead(but6);
  int button7=digitalRead(but7);
  int button8=digitalRead(but8);
  
  if(button1==1){
    tone(buzzer,220,100);
  }
   if(button2==1){
    tone(buzzer,246.9,100);
   }
  if(button3==1){
    tone(buzzer,261.3,100);
  }
  if(button4==1){
    tone(buzzer,293.3,100);
  }
  if(button5==1){
    tone(buzzer,329.3,100);
  }
  if(button6==1){
    tone(buzzer,349.5,100);
  }
  if(button7==1){
    tone(buzzer,392,100);
  }
  if(button8==1){
    tone(buzzer,440,100);
  }
  
  
 // lets put a short delay 
  delay(10);
  
}
