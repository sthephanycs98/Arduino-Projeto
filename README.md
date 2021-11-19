# Arduino-Projeto
Sensor de Temperatura com Arejamento

Alunas: Lethícia Marquezini 31740456 / Sthephany Chuber 31709311

Descrição do projeto realizado:

A princípio todos os materiais físicos serão juntados e montados (fios, resistores, jumpers, sensor de temperatura e air cooler). Após esse processo, a USB será conectada no computador e começaremos pelo carregamento do protocolo Firmata no microcontrolador para comunicar com o Arduino de forma adequada. Logo após, começa-se a aplicação Node-RED que irá trabalhar com o servidor e consequentemente iniciará o processo de medição da temperatura para ativar o ventilador.
A figura abaixo representa a conexão para este projeto:
![image](https://user-images.githubusercontent.com/50816053/121760274-3126d880-cb00-11eb-97e0-b58a61d68711.png)


Após a conclusão da conexão física dos componentes e a conexão via USB com um computador, partimos para a configuração e metodologia de execução do projeto, inicializando os componentes lógicos da aplicação. Primeiro, é necessário carregar o protocolo Firmata no nosso microcontrolador, para a comunicação com o Arduino ocorrer de forma efetiva, após isso iniciamos a aplicação Node-Red que vai trabalhar como servidor, na figura a seguir temos a montagem dos nodes da aplicação, começando pelo LM35 e terminando com o acionamento do cooler.    
![image](https://user-images.githubusercontent.com/50816053/142439329-c9b80a74-1202-4b58-8771-507480945448.png)

O dashboard para acompanharmos se a temperatura de 22º graus celsius (definido na função no Node-Red) é atingido para acionar o Air Cooler. Conforme a imagem a seguir, vemos que ao alcançar a temperatura, o switch é alterado para On e o Air Cooler é ativado:
![image](https://user-images.githubusercontent.com/50816053/142441169-f512f81b-2d0f-406b-bf92-9a791b59acb2.png)
