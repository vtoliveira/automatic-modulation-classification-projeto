# automatic-modulation-classification-projeto
Projeto da disciplina Comunicação Digital do Curso de Engenharia de Informação da Universidade Federal do ABC.

Estes notebooks são para o projeto da disciplina Comunicação Digital da Universidade Federal do ABC.
Iremos utilizar o dataset Communication-Digital-Signals criado pelo Professor Dr. Baochang Zhang e utilizado no paper Automatic Modulation Classification Based on Deep Learning for Unmanned Aerial Vehicles (https://pdfs.semanticscholar.org/7376/187ab51f95cf07f913bd98fab9a6fa7823c3.pdf)

### Problema

Nestes notebooks iremos classificar qual tipo de modulação pertence um certo sinal. Com grandes aplicações em área militares, de compliance e identificação de usuários que fazem uso indevido do sinal de comunicação, é de extrema importância o desenvolvimento de algoritmos capazes de identificar de forma confiável qual tipo de modulação trata-se um sinal, a fim de determinar seu conteúdo do método mais apropriado.

Os dados foram gerados pelo Dr. Baochang Zhang e podem ser encontrados em seu repositório no github (https://github.com/bczhangbczhang/Communication-Signal-Dataset). O dataset foi criado a partir de um simulador de dados geográficos do Visual Studio e simuladores de canais e modulações no Matlab. Basicamente, temos um sinal recebido da seguinte forma:
![image.png](attachment:image.png)

Onde y(t) é o sinal recebido, x(t) o sinal modulado, n(t) ruído AWGN e c(t) representa as especificações do canal (fading, etc). Assim, temos ao total 22000 dados com 963 amostras e o label de modulação que ele representa, sendo de 0-10 representando 2ASK, 2FSK, 2PSK, 4ASK, 4FSK, 4PSK, 8ASK, 8FSK, 8PSK, 16QAM e 64QAM, respectivamente. Para a mesma situação, foram gerados também dados variando-se a SNR, com valores de 0, 4, 8, 12, 16 e 20 dB.