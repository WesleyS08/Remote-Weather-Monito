
# 🌦️ Remote Weather Monito

Este projeto é uma estação meteorológica inteligente que utiliza um ESP32, um sensor DHT22 para medir temperatura e umidade, um display LCD para exibição local e conectividade MQTT para comunicação remota. O sistema monitora a temperatura e a umidade em tempo real e envia esses dados para um servidor MQTT. Além disso, ele também pode receber mensagens do servidor MQTT e exibi-las no display LCD.



## 🛠️ Ferrramentas usadas 

Para desenvolver este projeto, utilizamos algumas ferramentas online para emular o hardware do Arduino e conectar-se a um servidor MQTT. Aqui estão as principais 

- 🌐 MQTTHQ: Um servidor MQTT público utilizado para comunicação entre o ESP32 e outros serviços.

- 💻 Wokwi: Um emulador de hardware usado para simular o ambiente Arduino e testar o código antes da implementação no hardware real.  



## 📋 Funcionalidades
 
Este projeto oferece uma série de funcionalidades que incluem:

### 🌡️ Coleta de Dados Ambientais
| Funcionalidade  |     | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `Medir Temperatura e Umidade` |  | O projeto utiliza um sensor DHT22 para medir a temperatura e a umidade do ambiente.|
| `Exibição Local` |  | Um display LCD I2C é usado para exibir os valores medidos de temperatura e umidade em tempo real. |   



### 📡 Transmissão de Dados via MQTT
| Funcionalidade  |     | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `Publicação de Dados para um Servidor MQTT` |  |O projeto transmite os valores de temperatura e umidade para um servidor MQTT, permitindo monitoramento remoto e integração com outras aplicações IoT.|
| `Formato de Dados JSON` |  | Os dados são formatados como JSON antes de serem enviados para o servidor MQTT, facilitando a interoperabilidade e a análise de dados. |  

### 🔁 Interação com o Servidor MQTT
| Funcionalidade  |     | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `Recebimento de Mensagens MQTT` |  |O projeto pode receber mensagens do servidor MQTT e exibi-las no LCD. Isso permite interações bidirecionais, como comandos remotos ou notificações.|
| `Reconexão Automática ao MQTT` |  | Se a conexão com o servidor MQTT for interrompida, o projeto tenta reconectar automaticamente, garantindo a continuidade do serviço. |  

### 🛠️ Outras Funcionalidades
| Funcionalidade  |     | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `Conexão Wi-Fi` |  |O projeto se conecta a uma rede Wi-Fi para comunicação com o servidor MQTT.|
| `Indicadores Visuais` |  |  O LCD mostra mensagens para indicar o status da conexão Wi-Fi e do servidor MQTT, bem como para exibir mensagens recebidas.|  

## 🔧 Configurações Necessárias

Para rodar esse projeto, você vai precisar adicionar ou mudar as seguintes coisas 

🔗 `MQTT_BROKER`: Endereço do servidor MQTT.


🗣️ `MQTT_TOPIC`: Tópico MQTT para comunicação.

## Projeto

![Arduino](/img/arduino.png)


![server](/img/server.png)

## Licença

[MIT](https://choosealicense.com/licenses/mit/)


## Rodando os testes

esse é um exempro do projeto funcionadno 

![Arduino](/img/20240510_094155.gif)

