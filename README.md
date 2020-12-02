/*
Cruzamento
Descrição: Simulação de cruzamento de ruas
Elaborado por: Renner Chirinotti 
Data: 01/09/2020

Semáforo 1		Semáforo 2
13-vermelho		7-vermelho
12-amarelo		6-amarelo
11-verde		5-verde
*/

void setup()// Cofiguraçãoes iniciais 
{
  pinMode(7, OUTPUT); 	// Defie o pino 13 como saída
  pinMode(10, OUTPUT);	// Defne o pino 10 como saída
  pinMode(11, OUTPUT);	// Define o pino 11 como saída
  pinMode(12, OUTPUT);	// Define o pino 12 como saída
  pinMode(5, OUTPUT);	// Define o pino 5 como saída
  pinMode(6, OUTPUT);	// Define o pino 6 como saída
}

void loop()// Roda de maneira cilica os comandos abaixo
{
  digitalWrite(7, HIGH); 	// Liga o pino 7
  digitalWrite(10, HIGH); 	// Liga o pino 10
  delay(3000); 				// Aguardar 3 segundos(s)
  digitalWrite(10, LOW); 	// Desliga o pino 10
  digitalWrite(11, HIGH); 	// Liga o pino 11
  delay(2000); 				// Aguardar 2 segundos(s)
  digitalWrite(11, LOW); 	// Desliga o pino 11
  digitalWrite(12, HIGH); 	// Liga o pino 12
  digitalWrite(7, LOW); 	// Desliga o pino 7
  digitalWrite(5, HIGH); 	// Liga o pino 5
  delay(3000); 				// Aguardar 3 segundos(s)
  digitalWrite(5, LOW);		// Desliga o pino 5
  digitalWrite(6, HIGH);	// Liga o pino 6
  delay(2000); 				// Aguardar 2 segundos(s)
  digitalWrite(6, LOW);		// Desliga o pino 6
  digitalWrite(12, LOW);	// Desliga o pino 12
}
