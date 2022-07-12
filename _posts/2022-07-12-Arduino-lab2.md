# Lab 1
[Simple LED control on breadboard](https://www.tinkercad.com/things/7XpqwPmR0yH-neat-hillar/editel?tenant=circuits) this is a simple LED blinking display.


# Code

// C++ code
//
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  pinMode(3, OUTPUT);

  digitalWrite(LED_BUILTIN, LOW);
  analogWrite(3, 0);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  analogWrite(3, 1);
  delay(1000); // Wait for 1000 millisecond(s)
  analogWrite(3, 0);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
