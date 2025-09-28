# bAttle - Jogo de RPG Textual 

Um simples jogo de RPG por turnos, totalmente em uma única página HTML, onde você derrota monstros, coleta ouro, equipa itens e fica mais forte.

---

Powered by AI

---

#### Site do jogo: https://battlev102.netlify.app/splash.html​ (onde joga)

---

### **Sumário**
1.  [Visão Geral](#visão-geral)
2.  [Como Jogar](#como-jogar)
3.  [Mecânicas do Jogo](#mecânicas-do-jogo)
4.  [Itens e Equipamentos](#itens-e-equipamentos)
5.  [Créditos e Desenvolvimento](#créditos-e-desenvolvimento)
6.  [Código Completo](#código-completo)

---

### **Visão Geral**

`bAttle` é um jogo de RPG minimalista, construído com HTML, CSS e JavaScript. Ele opera inteiramente no seu navegador, sem a necessidade de um servidor. O jogo se concentra em combates simples e progressão do personagem através de um sistema de itens e níveis.

### **Como Jogar**

1.  **Encontrar Inimigo:** Clique no botão para iniciar um combate contra um monstro aleatório.
2.  **Atacar:** Clique no botão "Atacar" para causar dano ao inimigo. O combate é por turnos: você ataca, e depois o inimigo ataca.
3.  **Ganhar Recompensas:** Ao derrotar um inimigo, você ganha **Ouro** e **XP**.
4.  **Loja:** Use seu ouro para comprar itens poderosos na Loja e melhorar seus status.
5.  **Limpar Dados:** Se precisar começar do zero, use o botão "Limpar Dados" para apagar seu progresso salvo.

---

### **Mecânicas do Jogo**

#### **Combate**
O dano é calculado de forma simples:
* **Dano do Jogador:** `ATK do Herói` - `DEF do Inimigo`
* **Dano do Inimigo:** `ATK do Inimigo` - `DEF do Herói`
Ambos os ataques podem causar dano crítico com base no status **CRIT** do atacante.

#### **Nivelamento (Level Up)**
Você ganha **XP** ao derrotar inimigos. A quantidade de XP necessária para subir de nível é:
* `XP Necessária = Nível do Herói * 50`

Ao subir de nível, seus status base aumentam:
* `+10` para **HP Máximo**
* `+5` para **MP Máximo**

#### **Ouro e Loja**
O ouro é ganho ao derrotar inimigos. A loja oferece 1000 itens gerados aleatoriamente, com um sistema de raridade baseado em preço e poder.

---

### **Itens e Equipamentos**

O jogo possui um sistema de raridade **3:2:1**, que define os preços e o poder dos itens na loja.

* **Comuns (50%):** Preço de **1 a 100** de ouro. Adicionam um pequeno aumento nos status.
* **Raros (33%):** Preço de **101 a 5.000** de ouro. Oferecem um aumento moderado.
* **Épicos (17%):** Preço de **5.001 a 5.000.000** de ouro. Itens mais caros e poderosos do jogo.

#### **Tipos de Equipamento**
* **Arma:** Aumenta seu **ATQ** (Ataque) e **CRIT** (Chance de Crítico).
* **Off-hand:** Aumenta sua **DEF** (Defesa).
* **Amuleto:** Pode aumentar seu **HP**, **MP**, **ATK** e/ou **CRIT**.
* **Poção de Cura:** Item consumível que restaura todo o seu HP.

Os bônus de todos os itens equipados são somados aos seus status base para determinar seu poder total.

---

### **Créditos e Desenvolvimento**

Este projeto foi desenvolvido em colaboração, com o objetivo de criar um jogo simples e divertido em um único arquivo de código.

* **Designer:** O jogo foi projetado com base em contribuições diretas, incluindo o sistema de preços dos itens, a distribuição de raridade e os conceitos de jogo.
* **Desenvolvimento:** O código é escrito em **HTML**, **CSS** e **JavaScript** puro.

---

### **Código Completo**

Para rodar o jogo, basta copiar e colar o código abaixo em um arquivo `index.html`
