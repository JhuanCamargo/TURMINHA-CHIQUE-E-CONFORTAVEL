// # TURMINHA-CHIQUE-E-CONFORTAVEL
// PROGRAMAÇÃO BOTÃO + LED


//DECLARAR AS CONSTANTES
const int led = 7; //constante led pino dig. 7
const int botao =2; // "        botão	" 2


//VARIÁVEL QUE CONTERÁ SE O BOTÃO ESTÁ 0 = LOW OU 1 = HIGH

int estadoBotao =0;//estado desligado por isso = 0


//MÉTODO Setup >>>

void setup(){
pinMode(led, OUTPUT);
pinMode(botao,INPUT);


}
//METODO LOOP
void loop() {
 //LENDO O ESTADO DO PINO 2, CONSTANTE BOTÃO E
 //ATRIBUINDO O RESULTADO A VARIÁVEL estadoBotao
 
 estadoBotao = digitalRead(botao);
 
 
 //VERIFICANDO O ESTADO DO BOTAO CONDIÇÃO
 
 if (estadoBotao == HIGH) {
	digitalWrite(led, HIGH); // led ON
	}
	
	
	else {
	digitalWrite(led, LOW);
	}
  
}
