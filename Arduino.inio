#define BUTTON_PIN_NUM	8
#define LED_PIN_NUM		7

bool g_isRun = false;
bool g_isPressedButton = false;

void setup()
{
  pinMode(BUTTON_PIN_NUM, INPUT);
  pinMode(LED_PIN_NUM, OUTPUT);
}

void loop()
{
  if (g_isRun && digitalRead(BUTTON_PIN_NUM) && !g_isPressedButton){
  	g_isRun = false;
    digitalWrite(LED_PIN_NUM, LOW);
    g_isPressedButton = true;
  }
  else if (!g_isRun && digitalRead(BUTTON_PIN_NUM) && !g_isPressedButton){
  	g_isRun = true;
    digitalWrite(LED_PIN_NUM, HIGH);
    g_isPressedButton = true;
  }
  
  if (!digitalRead(BUTTON_PIN_NUM)){
    g_isPressedButton = false;
  }
}
