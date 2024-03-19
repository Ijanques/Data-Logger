# Data Logger Industrial

Este é um projeto de data logger industrial desenvolvido para monitorar e registrar níveis anormais de luminosidade, temperatura e umidade em uma planta industrial. O dispositivo é projetado para emitir sinais de alerta sonoros e visuais quando os valores detectados estiverem fora das faixas especificadas.

## Especificações Técnicas

### Componentes Utilizados:
- Arduino Uno R3
- Sensor de Temperatura
- Sensor de Luminosidade
- Sensor de Umidade
- Buzzer
- LED
- EEPROM
- RTC (Real Time Clock)
- Bateria de 9V (Backup de Alimentação)

### Faixas de Valores:
- Temperatura: 15 °C < t < 25 °C
- Luminosidade: 0% < l < 30%
- Umidade: 30% < u < 50%

## Funcionamento

O data logger industrial realiza as seguintes funções:

1. **Monitoramento de Sensores:** Os sensores de temperatura, luminosidade e umidade são continuamente monitorados pelo dispositivo.

2. **Detecção de Anormalidades:** Se os valores detectados estiverem fora das faixas especificadas, o dispositivo aciona um sinal de alerta sonoro e visual.

3. **Registro de Ocorrências:** As ocorrências anormais são registradas na EEPROM do Arduino, juntamente com a data e hora em que ocorreram.

4. **Backup de Alimentação:** Uma bateria de 9V é utilizada como backup de alimentação para garantir a integridade dos dados em caso de falha na alimentação principal.

5. **Registro de Data e Hora:** Um RTC (Real Time Clock) é utilizado para registrar a data e hora precisas de cada ocorrência.

6. **Visualização dos Dados:** Os dados registrados podem ser acessados posteriormente para análise.

## Diagrama Elétrico

a implementar

## Manual de Operação

Para montar e operar o data logger industrial, siga as instruções abaixo:

1. **Montagem:**
   - Conecte os sensores de temperatura, luminosidade e umidade aos pinos correspondentes do Arduino. Conforme indicado no projeto thinkercad em anexo
   - Conecte o buzzer e o LED aos pinos adequados do Arduino.Conforme indicado no projeto thinkercad em anexo
   - Certifique-se de alimentar o Arduino adequadamente.
   - Conecte o RTC de acordo com as especificações do fabricante.

2. **Configuração:**
   - Certifique-se de calibrar os sensores corretamente, se necessário.
   - Ajuste os limites de temperatura, luminosidade e umidade conforme necessário no código fonte.
   - Certifique-se de configurar corretamente o RTC para garantir a precisão do registro de data e hora.

3. **Operação:**
   - Ligue o dispositivo.
   - O data logger começará a monitorar os sensores.
   - Se valores anormais forem detectados, o buzzer emitirá um som e o LED acenderá.
   - As ocorrências serão registradas na EEPROM junto com a data e hora.

