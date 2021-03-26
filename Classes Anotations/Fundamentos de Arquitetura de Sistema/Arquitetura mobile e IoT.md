# IoT

## Preocupções
* Privacidade e segurança
* Quantidade exponencial de dispositivos conectados na rede
* Ser capaz de processar e armazenar uma enorme quantidade de informações
* Gerar valor a partir dos dados coletados

## Protocolo de comunicação
** MQTT - protocolo mais conhecido e utilizado para IoT **
Consegue rodar em celular além dos tradicionais Raspberry Pi, Arduino, etc.
* M2M - Machine 2 Machine de forma assíncrona
* Base na pilha do TCP/IP
* Padrão OASIS suportado por várias linguaguens de programaçaõ
* Utiliza modelo Pub/Sub

### QoS
* nivel 0 - menor esforço, não existe garantia de que a mensagem será entregue e também o mais barato
* nivel 1 - Garante que a mensagem foi entregue no minio uma vez ao receber. Msg pode ser retransmitida 
* nivel 2 - Mesmas garantias do nível 1 + broker armazena que o client recebeu a resposta. Modelo mais caro.