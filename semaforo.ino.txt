// Define os pinos dos LED
int Verde = 8;
int Amarelo = 9;
int Vermelho = 10;

void setup() {
  // Configura os pinos como saídas
  pinMode(Verde, OUTPUT);
  pinMode(Amarelo, OUTPUT);
  pinMode(Vermelho, OUTPUT);
}

void loop() {
  // LED Verde ligado (Carros passam)
  digitalWrite(Verde, HIGH);
  digitalWrite(Amarelo, LOW);
  digitalWrite(Vermelho, LOW);
  delay(2000); // Espera 2 segundos

  // LED Amarelo ligado (Atenção)
  digitalWrite(Verde, LOW);
  digitalWrite(Amarelo, HIGH);
  digitalWrite(Vermelho, LOW);
  delay(1000); // Espera 1 segundo

  // LED Vermelho ligado (Carros param)
  digitalWrite(Verde, LOW);
  digitalWrite(Amarelo, LOW);
  digitalWrite(Vermelho, HIGH);
  delay(2000); // Espera 2 segundos
}
