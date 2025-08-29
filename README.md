-----

<img alt="pucminas" src="https://joaopauloaramuni.github.io/image/fundo_teams_icei_capa_svg_3.svg?raw=true"/>

-----

# Repo Laboratorio de Iniciação à Programação

![GitHub repo size](https://img.shields.io/github/repo-size/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge) ![GitHub stars](https://img.shields.io/github/stars/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge) ![GitHub forks](https://img.shields.io/github/forks/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge) ![GitHub language count](https://img.shields.io/github/languages/count/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge) ![GitHub license](https://img.shields.io/github/license/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge&color=007ec6) ![GitHub last commit](https://img.shields.io/github/last-commit/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao?style=for-the-badge) ![Views Counter](https://views-counter.vercel.app/badge?pageId=https%3A%2F%2Fgithub%2Ecom%2Fjoaopauloaramuni%2Flaboratorio-de-iniciacao-a-programacao&leftColor=555555&rightColor=007ec6&type=total&label=Repo%20Views&style=upper)  

Disciplina do curso de Ciência da Computação da PUC Minas 

- 1°Sem 2024

-----

### Sumário:
- [Aulas em PDF](https://github.com/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao/tree/main/PDF)
- [Atividades com SCRATCH](https://github.com/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao/tree/main/SCRATCH)
- [Atividades com TINKERCAD](https://github.com/joaopauloaramuni/laboratorio-de-iniciacao-a-programacao/tree/main/TINKERCAD)

#### Links úteis:

##### 🧪 TINKERCAD

- 🎵 [Exemplo Piezo - Música Do Re Mi Fa no Buzzer](https://www.tinkercad.com/things/aM5CrCyPsk3-musica-do-re-mi-fa-no-buzzer?sharecode=b1cv6yhNJ4K3S4Nizf7RTXKxM89S2m4DKHRL6VDUUjM)
- 🎶 [Exemplo Arduino Songs - Repositório no GitHub](https://github.com/robsoncouto/arduino-songs)

##### 💡 Dicas para o trabalho do GENIUS

- 🖨️ [Função Serial.println()](https://www.arduino.cc/reference/pt/language/functions/communication/serial/println/)
- 🎼 [Função tone()](https://www.arduino.cc/reference/pt/language/functions/advanced-io/tone/)
- 🎲 [Função randomseed()](https://www.arduino.cc/reference/pt/language/functions/random-numbers/randomseed/)
- 🎚️ [Função analogRead()](https://www.arduino.cc/reference/pt/language/functions/analog-io/analogread/)

##### 🛠️ Projetos

- 🧰 [Link do primeiro projeto no TINKERCAD](https://www.tinkercad.com/things/8eiV2qBfo7p-primeiroprj?sharecode=RDpDAr_wetgqmD450qSU3mOcuxu7ifrfz_gJ4tp3uXc)
- 🔧 [Link do segundo projeto no TINKERCAD](https://www.tinkercad.com/things/caJB5BoGqT5-segundoprj?sharecode=QOZkeGFn7rutd8pNzPoW4TDYIsgxIswnG3CQIYtr9-Q)

##### 🧑‍🏫 Turma - TINKERCAD

- 👨‍💻 [Link da turma no TINKERCAD](https://www.tinkercad.com/joinclass/JWLN7XVLG)

-----

##### 🧩 SCRATCH

- 🚀 [Exemplo Jogo Espacial 1](https://scratch.mit.edu/projects/976796355/editor/)
- 🛸 [Exemplo Jogo Espacial 2](https://scratch.mit.edu/projects/979046219/editor/)
- 🧭 [Exemplo Labirinto](https://scratch.mit.edu/projects/1005948595/editor/)
- 👾 [Exemplo PACMAN](https://scratch.mit.edu/projects/13701368/editor/)
- 📦 [Recursos PACMAN](https://tinyurl.com/pac-man-recursos)
- 🏁 [Exemplo MARIOKART](https://scratch.mit.edu/projects/46578586/editor/)

-----

#### ⌨️ Comandos úteis:

```cpp
// Gerar uma semente aleatória com base em ruído analógico
randomSeed(analogRead(0)); // Garante que os números aleatórios sejam diferentes a cada execução

// Sortear um número de 1 a 4 (por exemplo, para representar cores: verde, azul, vermelho, amarelo)
sequencia[n] = random(1, 5); // Gera um número inteiro aleatório de 1 a 4 (intervalo: [1, 4])

// Definir pinos como entrada ou saída
pinMode(ledPin, OUTPUT);     // Define o pino como saída (para LEDs, por exemplo)
pinMode(botaoPin, INPUT);    // Define o pino como entrada (para botões)
pinMode(sensorPin, INPUT);   // Entrada analógica ou digital de sensor

// Acionar ou desligar um pino digital
digitalWrite(ledPin, HIGH);  // Liga o LED ou envia sinal alto (5V)
digitalWrite(ledPin, LOW);   // Desliga o LED ou envia sinal baixo (0V)

// Ler estado de botão ou sensor digital
int estado = digitalRead(botaoPin); // Lê se o botão está pressionado (HIGH) ou não (LOW)

// Ler valor de sensor analógico
int valor = analogRead(A0); // Lê valor de 0 a 1023 de um sensor conectado à entrada analógica A0

// Esperar um tempo (em milissegundos)
delay(1000); // Espera 1 segundo (1000 ms)

// Imprimir mensagens no monitor serial (útil para depuração)
Serial.begin(9600);             // Inicia comunicação serial a 9600 bauds
Serial.print("Valor: ");        // Imprime sem pular linha
Serial.println(valor);          // Imprime com quebra de linha

// Funções auxiliares para tornar o código mais legível
void acenderLed(int pino) {
  digitalWrite(pino, HIGH);     // Liga o LED conectado ao pino especificado
}

void apagarLed(int pino) {
  digitalWrite(pino, LOW);      // Desliga o LED conectado ao pino especificado
}

// Extras úteis
// Inverter estado de um LED (toggle)
digitalWrite(ledPin, !digitalRead(ledPin)); // Lê o estado atual e escreve o oposto

// Controle PWM (dimerização de LEDs, motores, etc.)
analogWrite(ledPin, 128); // Escreve valor de 0 a 255 (50% da intensidade máxima)

// Debounce simples para botões
if (digitalRead(botaoPin) == HIGH) {
  delay(50); // Espera para evitar falso acionamento
  if (digitalRead(botaoPin) == HIGH) {
    // botão foi pressionado de verdade
  }
}
```

-----

#### 📑 Exemplo de um relatório para o trabalho final de Scratch:

##### 📘 Relatório do Projeto: *Floppy Fish Adventures*

###### 🧾 Introdução:
O jogo *"Floppy Fish Adventures"* foi desenvolvido como parte do projeto final em Scratch, com o objetivo de demonstrar competências em programação, design de jogos e lógica computacional. Este relatório detalha o processo de desenvolvimento, as ferramentas utilizadas, a motivação por trás do jogo e como ele funciona. O projeto reflete a aplicação prática de conceitos fundamentais em desenvolvimento de jogos e design interativo.

-----

###### 🎮 1. Descrição do Jogo:
*"Floppy Fish Adventures"* é um jogo de ação e habilidade em que os jogadores controlam um peixe navegando por um rio cheio de obstáculos. A principal mecânica é desviar de troncos e pedras que aparecem de forma contínua, enquanto tenta sobreviver o máximo possível. O jogo oferece uma experiência desafiadora e divertida, com pontuações baseadas na distância percorrida.

-----

###### 🧱 2. Elementos Utilizados:

- **🔼 Movimentos:**  
  Usei blocos de movimento para controlar a movimentação do peixe (cima e baixo).

- **🎨 Aparências:**  
  Criação de sprites personalizados para o peixe, troncos, pedras e o cenário do rio.

- **🔊 Sons:**  
  Adicionados efeitos sonoros de água e colisões para aumentar a imersão.

- **📡 Eventos:**  
  Utilização de eventos para detectar colisões entre o peixe e os obstáculos.

- **🎮 Controle:**  
  Controles simples; o jogador clica ou pressiona uma tecla para fazer o peixe nadar para cima.

- **📊 Variáveis:**  
  Implementação de variáveis para gerenciar a pontuação e o estado do jogo (ativo ou game over).

- **➗ Operadores:**  
  Operadores usados para calcular a pontuação com base na distância percorrida pelo peixe.

-----

###### 💭 3. Motivação:

Minha principal motivação para criar *"Floppy Fish Adventures"* foi desenvolver um jogo que fosse:  
- 🎯 Divertido e desafiador.  
- 💻 Capaz de demonstrar minhas habilidades em programação e design.  
- 🎨 Um exercício criativo para explorar mecânicas simples mas envolventes.  

O desafio esteve em equilibrar a dificuldade para manter o jogador engajado.

-----

###### ⚙️ 4. Funcionamento do Jogo:

1. 🐟 O jogo inicia com o peixe posicionado no centro do rio.  
2. 🖱️ O jogador clica ou pressiona uma tecla para fazer o peixe nadar para cima.  
3. 🌲 Obstáculos como troncos e pedras se aproximam continuamente.  
4. 💥 Se o peixe colidir com um obstáculo, o jogo termina, e a pontuação final é exibida.  
5. 🔁 Após o término, o jogador pode optar por reiniciar o jogo para tentar alcançar uma pontuação maior.

-----

###### 🏁 5. Conclusão:

*"Floppy Fish Adventures"* foi um projeto desafiador e gratificante, que me permitiu aplicar e consolidar conceitos de programação, lógica e design de jogos.  
O processo de desenvolvimento envolveu desde a criação de sprites personalizados até a implementação de mecânicas simples mas eficazes para garantir a jogabilidade.  
Como aprendizado principal, destaco a importância do equilíbrio na dificuldade do jogo para manter o interesse do jogador. Estou satisfeito com o resultado e considero que o jogo cumpre seu objetivo de oferecer uma experiência divertida e desafiadora.

-----

<div align="center">
  <img width="70%" alt="pucminas" src="https://joaopauloaramuni.github.io/image/engsoft2.svg?raw=true"/>
</div>

-----
