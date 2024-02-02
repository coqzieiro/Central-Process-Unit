## 1. Introdução

A unidade central de processamento, é a parte de um sistema computacional, que realiza as instruções de um programa de computador, que executa a aritmética básica, orientado por um padrão binário 0 e 1, que possibilita a entrada, o processamento e saída de dados.  A CPU é implementada em um circuito integrado (CI) chamado microprocessador, que pode conter uma ou mais CPUs em um único chip. Um microprocessador com várias unidades é chamado de processador multi-core. Cada núcleo, pode também ser dividida em várias CPUs virtuais ou lógicas, usando uma técnica chamada multithreading.

A ideia do projeto é desenvolver um circuito no Quartus Prime Lite Edition para simular o comportamento de uma CPU.

## 2.Desenvolvimento

O projeto da CPU foi implementado na placa FPGA DE0-CV Cyclone V.

#### 2.1 ULA (Unidade Lógica e Aritmética)

A ULA é o componente da CPU que realiza as operações aritméticas (soma, subtração, multiplicação, divisão) e lógicas entre os dados armazenados nos registradores. Tal componente recebe dois operandos de entrada, um código de operação que indica qual operação deve ser realizada, e gera um resultado de saída e um sinal de status que indica se houve algum erro ou condição especial.

#### 2.2 Registradores
Registradores são pequenas memórias internas da CPU que armazenam dados temporariamente durante a execução de um programa. Eles são mais rápidos do que a memória principal, mas possuem uma capacidade limitada. Existem diferentes tipos de registradores, como registradores de dados, que armazenam os operandos e os resultados das operações da ULA, registradores de endereço, que armazenam os endereços de memória onde os dados estão localizados, e registradores de controle, que armazenam informações sobre o estado da CPU.

#### 2.3 Contadores
Contadores são circuitos sequenciais que contam o número de pulsos de um sinal de clock. Eles podem ser usados para gerar sequências de números binários ou para medir intervalos de tempo. Eles podem ser classificados em contadores síncronos ou assíncronos, dependendo se todos os flip-flops que os compõem são acionados pelo mesmo sinal de clock ou por sinais diferentes. No caso da CPU, usamos o contador assíncrono.

#### 2.4 Unidade de Controle (UC)
A unidade de controle é o componente da CPU que coordena as ações dos demais componentes, como a ULA, os registradores e a memória principal. Ela é responsável por buscar, decodificar e executar as instruções de um programa. A UC pode ser implementada por meio de circuitos combinacionais e sequenciais com lógica fixa ou por meio de um microprograma armazenado em uma memória interna com lógica programável.

#### 2.5 Display de 7 Segmentos

Um display de 7 segmentos é um dispositivo eletrônico que exibe dígitos decimais ou hexadecimais usando sete segmentos luminosos dispostos em forma de 8. Cada segmento pode ser acionado individualmente por meio de um sinal elétrico, podendo ser do tipo catodo ou anodo comum, dependendo se os segmentos são ligados ao polo negativo ou positivo da fonte de alimentação. Para acender um segmento, é preciso aplicar uma tensão inversa à do tipo do display. 

## 3. Simulações

#### 3.1 ULA (Unidade Lógica e Aritmética)

#### 3.2 Registradores

#### 3.3 Contadores

#### 3.4 Unidade de Controle (UC)

#### 3.5 Display de 7 Segmentos

#### 3.6 CPU Memória 1

#### 3.7 CPU Memória 2

## 4. Conclusão

Neste relatório, apresentamos os conceitos básicos sobre a CPU e os componentes que fazem parte dessa estrutura.  Concluímos que CPU é um extremamente importante no funcionamento do computador, pois é ela que executa as instruções de um programa e realiza as operações aritméticas e lógicas entre os dados. A CPU é formada por circuitos integrados que implementam a lógica digital por meio de portas lógicas, flip-flops e outros elementos. A CPU interage com a memória principal e com os dispositivos de entrada e saída por meio de barramentos de dados, endereços e controle.

A compreensão do funcionamento da CPU é fundamental para o estudo da arquitetura e da organização de computadores, bem como para o desenvolvimento de programas eficientes e otimizados.

## 5. Referências

TOCCI, R. J.; WIDMER, N. S.; MOSS, G. L. Sistemas digitais: princípios e aplicações. 11. ed. São Paulo: Pearson Prentice Hall, 2011.

STALLINGS, W. Arquitetura e organização de computadores. 8. ed. São Paulo: Pearson Prentice Hall, 2010.

FERREIRA, A.; PEREIRA, F.; SILVA, J.; SILVA, M.; SOUSA, P. Circuitos sequenciais: contadores. Universidade do Minho, 2009.

MONTEIRO, M. A. Introdução à organização de computadores. 5. ed. Rio de Janeiro: LTC, 2007.

FRANCHI, E.; IAROSSI, R.; MARQUES FILHO, O.; MEDINA, N.; ZUFFO, M. Display de 7 segmentos: conceitos básicos e aplicações práticas. Universidade de São Paulo, 2003. 

COMPUTER HOPE - "CPU (Central Processing Unit)." Computer Hope. Disponível em: https://www.computerhope.com/jargon/c/cpu.htm.

BRITANNICA - "Central processing unit (CPU)." Encyclopaedia Britannica. Disponível em: https://www.britannica.com/technology/central-processing-unit.

