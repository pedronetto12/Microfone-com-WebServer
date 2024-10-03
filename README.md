Este projeto contém dois programas que configuram um servidor web para controlar um dispositivo ESP32. Dependendo de sua aplicação, você pode optar por uma das seguintes configurações de rede:

Conexão Direta com o ESP32 (Modo Access Point - AP):
Nesse modo, o ESP32 funciona como um ponto de acesso (AP), permitindo que dispositivos, como seu smartphone ou computador, se conectem diretamente a ele. Após a conexão, você pode acessar a interface web hospedada pelo ESP32 para realizar o controle ou visualização de dados.

Conexão Via Roteador (Modo Station - STA):
Neste modo, o ESP32 se conecta à rede local de um roteador. Você poderá acessar a interface web hospedada pelo ESP32 a partir de qualquer dispositivo conectado à mesma rede Wi-Fi, utilizando o endereço IP atribuído ao ESP32 pelo roteador.
