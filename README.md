CP2 - Edge Computing 🍷💡
Projeto: Vinheria Agnello – Monitoramento de Luminosidade, Temperatura e Umidade com Arduino

Este repositório contém o projeto desenvolvido para o Checkpoint 02 da disciplina Edge Computing & Computer Systems (FIAP - 2025). Trata-se de um sistema físico e funcional montado com Arduino, focado no monitoramento da luminosidade, Temperatura e Umidade do ambiente de armazenamento da Vinheria Agnello, com o objetivo de preservar a qualidade dos vinhos.

🧩 Descrição do Desafio
A Vinheria Agnello tem a intenção de ampliar suas atividades para o meio digital, mantendo a excelência no atendimento e no zelo pelos produtos. O nosso objetivo foi sugerir um sistema integrado que pudesse identificar condições ambientais inapropriadas da estufa dos vinhos— no caso, excesso de luz, temperaturas muito elevadas ou muito baixas, e umidade inadequada mostrando em uma tela do LCD os resultados. Porém, fazendo o circuito percebemos que o simulador TinkerCAD não possui o sensor DHT 11 que iremos usar no projeto físico... então usamos um sensor do próprio simulador.

Funcionalidades implementadas:
Leitura do nível de luminosidade com sensor LDR;
LEDs sinalizadores:
✅ Verde: ambiente adequado;
⚠️ Amarelo: luminosidade em alerta;
❌ Vermelho: luminosidade inaceitável;
Acionamento de buzzer quando houver alerta;

Leitura do nível de temperatura e Umidade com o DHT11:
✅Temperatura OK: Temperatura entre 10°C e 15°C;
❌Temperatura Fria: Temperatura abaixo de 10°C;
❌ Temperatura Quente: Temoeratura a cima de 15°C;
✅Umidade ok: Umidade entre 50% e 70%;
❌Umidade Baixa: Umidade abaixo de 50%;
❌Umidade Alta: Umidade a cima de 70%;

💡 Solução Técnica
O sistema foi montado fisicamente e também simulado no Tinkercad.

🔗 Simulação no Tinkercad
https://www.tinkercad.com/things/fe9vuVPYnbp-cp2-edge-computing?sharecode=wGM_nSf_tSDv2zDrcT62B0VDeKhKQqVPBCKxfacoClU

🖼️ Imagem da simulação no Tinkercad
![image](https://github.com/user-attachments/assets/5d3ce3f0-99af-46ea-912e-9e4190adde08)


🔧 Componentes Utilizados
1 × Arduino Uno R3 (U1)
1 × Fotorresistor (LDR) (Rluz)
4 × Resistor de 220 Ω (R4) (conectados nos LEDs e no LDR)
3 × LEDs:
1 × Vermelho
1 × Verde
1 × Amarelo
1 × Buzzer Piezoelétrico 
Cabos Jumpers
1 × Protoboard


🛠️ Montagem do Circuito (Resumo)
LDR + resistor de 220Ω: leitura feita no pino analógico A1 (formando um divisor de tensão);
LEDs: conectados aos pinos digitais:
Verde → pino 13
Amarelo → pino 12
Vermelho → pino 11
Buzzer: conectado ao pino digital 10;
Resistores de 220 Ω conectados em série com cada LED e no LDR;
GND e 5V do Arduino distribuídos nos trilhos laterais da protoboard.

💾 Execução do Projeto
Monte o circuito conforme o esquema elétrico;
Faça o upload do código na placa usando a IDE do Arduino;
Ajuste a luminosidade manualmente (ou use o controle do Tinkercad) para testar os diferentes comportamentos do sistema;
Observe os sinais visuais (LEDs, LDR, LCD e sensor de temperatura DHT 11) e sonoros (buzzer) em tempo real.
👥 Integrantes do Grupo
Julia Pompeu – 561955
Laura Tigre Amaral – 565281
Áurea Sardinha Carminato – 563837
Giovana Parreira – 562275
Ben-Hur Iung de Lima Ferreira – 561564
