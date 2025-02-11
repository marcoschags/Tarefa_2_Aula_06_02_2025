# Instruções de Uso do Código para Controle de Servo e LED RGB
## Introdução

Este programa foi desenvolvido para controlar um servomotor utilizando o PWM de um Raspberry Pi Pico e acionar um LED RGB em uma GPIO específica. Ele permite movimentar o servomotor para diferentes posições e realizar um ciclo de movimentação suave. Além disso, o LED pisca em intervalos de 1 segundo.

# Requisitos
- Placa Raspberry Pi Pico (BitDogLab)
- Servomotor compatível com PWM
- LED RGB ou LED comum
- Software de desenvolvimento, como VSCode com Pico SDK instalado

# Conexão de Hardware
## Servomotor:

- Pino de Sinal (PWM): Conectar ao GPIO 22
- VCC: Conectar ao 3.3V ou 5V, dependendo do modelo do servo
- GND: Conectar ao GND

## LED RGB:
- Pino do LED: Conectar ao GPIO 12
- Resistor (se necessário): Entre 220 e 1kΩ
- GND: Conectar ao GND

## Compilação e Execução

- Abra o VSCode e carregue o código.
- Compile o programa utilizando o CMake e o Pico SDK.
- Coloque o Raspberry Pi Pico em modo BOOTSEL:
- Pressione e segure o botão BOOTSEL.
- Conecte via USB ao computador.
- Solte o botão BOOTSEL.

# Funcionamento do Programa
## Inicialização:

- Configura o PWM no GPIO 22 para controlar o servomotor.
- Configura o GPIO 12 para controle do LED.
- Movimenta o servomotor para as seguintes posições:

- 180° (pulso de 2400µs)
- 90° (pulso de 1470µs)
- 0° (pulso de 500µs)
- Executa movimentação suave entre 0° e 180°.
- Acende e apaga o LED em intervalos de 1 segundo.

# Vídeo - https://youtu.be/bo4hzWSQV8U
# Projeto no Wokwi.com - https://wokwi.com/projects/422260045451850753


