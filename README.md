# EA076-Projeto3
# Barco de Controle Remoto com BitDogLab

Este projeto apresenta um barco de controle remoto desenvolvido com a placa **BitDogLab**, explorando conceitos de sistemas embarcados, automação e programação. A proposta combina controle remoto via Bluetooth, propulsão, direção, iluminação e sinalização sonora de forma interativa e funcional.

## Funcionalidades do Projeto

- **Controle Direcional**: Ajuste da direção do leme via servo motor com comandos (`left`, `right`, `front`).
- **Propulsão**: Controle de motores DC para movimentação com comandos (`START`, `PAUSE`).
- **Iluminação**: LEDs Neopixel para sinalização com comandos (`Luz`, `On Light`, `Off Light`).
- **Buzina**: Ativação de som e piscas com o comando (`Buzina`).
- **Feedback Interativo**: Display OLED exibe o status em tempo real.

## Como Usar

### Requisitos

#### Hardware Necessário:
- Placa BitDogLab
- Servo Motor
- Motores DC (3V ou superiores)
- Transistor BC548
- Módulo Bluetooth HC-05
- Display OLED SSD1306
- Neopixel Matriz de LEDs 5x5
- Buzzer

#### Software:
- Editor de código compatível (ex.: Thonny, VS Code)
- Firmware MicroPython instalado na BitDogLab
- Aplicativo ou dispositivo que envie comandos Bluetooth (ex.: Serial Bluetooth Terminal)

### Configuração

1. Conecte os componentes conforme o diagrama de conexões:
   - **Servo Motor**: GPIO 18
   - **Motores DC**: GPIO 8 (via transistor BC548)
   - **Módulo Bluetooth**: GPIO 16 (TX), GPIO 17 (RX)
   - **Buzzer**: GPIO 21
   - **LEDs Neopixel**: GPIO 7
   - **Display OLED**: GPIO 14 (SDA), GPIO 15 (SCL)

2. Carregue o código-fonte para a BitDogLab usando o firmware MicroPython.

3. Certifique-se de que o módulo Bluetooth está pareado com o dispositivo de controle.

### Envio de Comandos

- **Propulsão**: `START` (iniciar motores) ou `PAUSE` (pausar motores).
- **Direção**: `left`, `right`, `front` (controle do leme).
- **Iluminação**: `Luz`, `On Light`, `Off Light` (controle dos LEDs).
- **Buzina**: `Buzina` (ativa o som e LEDs piscantes).

### Teste do Sistema

1. Conecte o sistema e verifique as conexões físicas.
2. Ligue a BitDogLab e o dispositivo de controle remoto.
3. Envie comandos via Bluetooth e observe a resposta do barco.

## Melhorias Futuras

- Adição de sensores para navegação autônoma.
- Controle PWM para ajuste de velocidade dos motores.
- Integração de uma câmera para monitoramento remoto.

---

Sinta-se à vontade para ajustar esse formato diretamente no GitHub, incluindo imagens, diagramas ou links adicionais, conforme necessário!

