int led1 = 2;
int led2 = 4;
int led3 = 5;
int led4 = 7;
void setup()
{
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
  pinMode(led4, OUTPUT);
}
void loop()
{
  if (led2 == HIGH){
    digitalWrite (led1, LOW);
  }else {
    digitalWrite (led4, HIGH);
    digitalWrite (led2, HIGH);
    delay (2000);
    if (led2 == LOW){
    digitalWrite (led1, HIGH);
  }else {
    digitalWrite (led4, LOW);
    digitalWrite (led2, LOW);
    delay (2000);
    }
  }
  if (led1 == HIGH){
    digitalWrite (led2, LOW);
  }else {
    digitalWrite (led3, HIGH);
    digitalWrite (led1, HIGH);
    delay (2000);
    
    if (led1 == LOW){
    digitalWrite (led2, HIGH);
  }else {
    digitalWrite (led3, LOW);
    digitalWrite (led1, LOW);
    delay (2000);
    }
  }
}
