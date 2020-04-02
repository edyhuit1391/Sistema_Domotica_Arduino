#include <Servo.h> //Esta librería nos facilita el control de servomotores

//Creando objeto tipo Servomotor:
Servo ServoGarage;

//Declaración de variables
int Valor_LDR_Garage; //Valor de estado de la fotoresistencia del garage

//Entradas/Salidas Analógicas de Arduino
int LDR_Garage = A3; //Indicando que la fotoresistencia del garage estará en la salida A3 de Arduino


void setup() {
  
  //Enviando como parametro el número del pin al objeto servomotor del garage:
  ServoGarage.attach(12);
  
}

void loop() {
     
  //Servomotor en 0 grados si el valor de la fotoresistencia es inferior a 400:
  if(Valor_LDR_Garage < 400) {
      ServoGarage.write(0);
    }

  //Servomotor en 90 grados si el valor de la fotoresistencia es superior a 500:
  if(Valor_LDR_Garage > 500) {
      ServoGarage.write(90);
    }
   
}
