
# Projeto ESP32 - Servidor Web

Este projeto contém dois programas que configuram um servidor web para controlar um dispositivo ESP32. Dependendo de sua aplicação, você pode optar por uma das seguintes configurações de rede:
![Dispositivo](https://github.com/pedronetto12/Microfone-com-WebServer/blob/main/dispositivo.jpg)

## Conexão Direta com o ESP32 (Modo Access Point - AP)
Nesse modo, o ESP32 funciona como um ponto de acesso (AP), permitindo que dispositivos, como seu smartphone ou computador, se conectem diretamente a ele. Após a conexão, você pode acessar a interface web hospedada pelo ESP32 para realizar o controle ou visualização de dados.

## Conexão Via Roteador (Modo Station - STA)
Neste modo, o ESP32 se conecta à rede local de um roteador. Você poderá acessar a interface web hospedada pelo ESP32 a partir de qualquer dispositivo conectado à mesma rede Wi-Fi, utilizando o endereço IP atribuído ao ESP32 pelo roteador.

## Ligações

```
  Módulo SD                       ESP32                      Mic INMP441
   ________                   _____________                   _________
  |     CS |-----------------|(5)      (15)|-----------------| I2S_WS  |
  |   MOSI |-----------------|(23)      (2)|-----------------| I2S_SCK |
  |   MISO |-----------------|(19)     (13)|-----------------| I2S_SD  | 
  |    GND |-----------------|(GND)   (GND)|-----------------| GND     |
  |    Vcc |-----------------|(Vcc)   (Vcc)|-----------------| Vcc     |
  |________|                 |_____________|                 |_________|
```

### Observações
- **CS**: Chip Select do módulo SD
- **MOSI**: Master Out Slave In do módulo SD
- **MISO**: Master In Slave Out do módulo SD
- **GND**: Terra
- **Vcc**: Alimentação
- **I2S_WS**: Word Select
- **I2S_SCK**: Serial Clock
- **I2S_SD**: Serial Data

## Como Usar
1. Escolha a configuração de rede desejada (AP ou STA).
2. Faça as conexões conforme descrito acima.
3. Carregue o programa no ESP32.
4. Acesse a interface web conforme necessário.

Se tiver dúvidas ou sugestões, sinta-se à vontade para contribuir!
