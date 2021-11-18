# Arduino-Projeto
Sensor de Temperatura com Arejamento

Alunas: Lethícia Marquezini 31740456 / Sthephany Chuber 31709311

Descrição do projeto realizado:

A princípio todos os materiais físicos serão juntados e montados (fios, resistores, jumpers, sensor de temperatura e air cooler). Após esse processo, a USB será conectada no computador e começaremos pelo carregamento do protocolo Firmata no microcontrolador para comunicar com o Arduino de forma adequada. Logo após, começa-se a aplicação Node-RED que irá trabalhar com o servidor e consequentemente iniciará o processo de medição da temperatura para ativar o ventilador.
A figura abaixo representa a conexão para este projeto:
![image](https://user-images.githubusercontent.com/50816053/121760274-3126d880-cb00-11eb-97e0-b58a61d68711.png)


Foi realizado a conexão de todos os componentes físicos em um computador para iniciarmos a execução. Iniciamos a comunicação do Arduino com o protocolo Firmata, sendo realizado com êxito através do sketch de exemplos (Firmata > StandardFirmata) no software IDE do Arduino. 
Logo após, abrimos o Node-Red com todos os componentes já conectados e com todas as devidas funções definidas. O MQTT é o responsável pela comunicação do dispostivo Arduino para com o dashboard, que recebe automaticamente, todas as informações da temperatura para assim acionar o Air Cooler.  
![image](https://user-images.githubusercontent.com/50816053/142439329-c9b80a74-1202-4b58-8771-507480945448.png)

Após o deploy, abrimos o dashboard para acompanharmos se a temperatura de 23º graus celsius (definido na função no Node-Red) é atingido para acionar o Air Cooler. Conforme a imagem a seguir, vemos que ao alcançar a temperatura, o switch é alterado para On e o Air Cooler é ativado:
![image](https://user-images.githubusercontent.com/50816053/142441169-f512f81b-2d0f-406b-bf92-9a791b59acb2.png)
