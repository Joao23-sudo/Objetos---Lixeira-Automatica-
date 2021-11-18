# Projeto - Lixeira Automática 

# Membros do Projeto
    João Vitor Freire Dias - TIA: 31919537
    Adriano Lopes Martins - TIA: 31857647
    
# Descrição de uso e Funcionamento 

Como primeiro projeto de IoT estávamos visando o que utilizamos no dia-a-dia que poderíamos automatizar. A ideia inicial, era automatizar uma cortina de janela, porém em vista da complexidade e tempo, optamos por automatizar uma lixeira, é utilizada diariamente pelas pessoas e para não ficar abrindo e fechando, faremos este trabalho de forma sútil.

O produto-ﬁnal do projeto foi a criação de uma lixeira automática. Assim que ligado, o sensor do protótipo detectava a presença de uma pessoa com a intenção abrir a lixeira, que automaticamente manda um sinal para o microcontrolador NodeMCU, que transmitia para o computador via cabo micro USB. O software Arduino IDE então passava a sua programação de volta para o microcontrolador, que transmitia a informação de abrir a lixeira, ou exibir uma mensagem no MQTT Dash.

[Clique aqui](https://www.youtube.com/watch?v=jzSzF4YRMc4) Para assistir o vídeo

# Hardware Utilizados

  1 - 1x NodeMCU ESP8266
  2 - 1x Cabo Micro USB
  3 - 2x Sensores de Distância - HC-SR04
  4 - 1x Micro Servo SG-90.
  5 - 1x Lixeira de porte médio.
  6 - 1x Pistola de Cola Quente.
  7 - 8x Cabo Wire Jumper Fêmea x Fêmea 20Cm
  8 - Arduino IDE
  9 - MQTT Dash
 
 
 # Modo de Montagem
 
Agora que temos todos os Materias, vamos montar nosso protótipo.

Posicione o NodeMCU da melhor onde voce pode fazer a conexão com os sensores e 

Ligamos os cabos no NodeMCU com o sensor HC-SR04.

Podemos acompanhar melhor o que foi dito acima atráves do [diagrama do circuito eletroeletrônico](https://github.com/Joao23-sudo/Objetos---Lixeira-Automatica-/blob/main/Circuito%20eletronico.png).

Para melhor compreender como fica o resultado final do projeto montado, segue imagem abaixo:

![Lixeira Automática](https://user-images.githubusercontent.com/65844927/142509526-c6e6840d-5f54-4205-b65a-2f024328073d.png)

# Software Desenvolvido

Para programar o que vamos desenvolver devemos primeiramente baixar o Arduino IDE e caso não tenha esse Software você pode fazer o download [Clique Aqui](https://www.arduino.cc/en/software/)

Após a instalação do Arduino IDE, vamos instalar dentro dele as bibliotecas necessárias: O esp8266 by ESP8266 Community, que permite que o microcontrolador NodeMcu seja reconhecido, o PubSubClient e os tópicos publishers e subscribers, para a comunicação com o MQTT, tornando possível a utilização do mqtt.

