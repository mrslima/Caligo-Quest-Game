# **Caligo Quest - Manual de Regras**

## **1. Visão Geral**
**Caligo Quest** é um jogo de exploração, estratégia e combate onde jogadores devem descobrir caminhos, enfrentar armadilhas e outros jogadores, além de coletar itens e a Chave do Portão para alcançar a vitória. O jogo se desenrola em um tabuleiro modular, criado dinamicamente conforme os jogadores avançam.

## **2. Componentes do Jogo**
- **Dados:**
  - **Dado Amarelo**: Define a movimentação do jogador.
  - **Dado Vermelho**: Determina o dano de um ataque.
  - **Dado Azul**: Utilizado para defesa contra ataques.
- **Tabuleiro Modular:** Criado dinamicamente com **tiles** de terreno.
- **Cartas de Tiles:** Representam os terrenos exploráveis.
- **Cartas de Itens:** Concedem vantagens e efeitos especiais.
- **Totens:** Permitem teletransporte entre locais específicos.
- **Chave do Portão:** Item essencial para desbloquear a vitória.

## **3. Visão Geral da Jogabilidade**
Os jogadores exploram um tabuleiro modular enquanto enfrentam desafios, coletam itens e competem entre si. O objetivo principal é encontrar a **Chave do Portão** e utilizá-la para vencer o jogo.

## **4. Configuração Inicial**
1. **Distribuição do Tabuleiro**: Todos os tiles começam desconhecidos.
2. **Ordem de Jogadores**: Determinada por rolagem de dados (desempates requerem nova rolagem).
3. **Distribuição de Vida**: Cada jogador inicia com **6 pontos de vida (6 HP).**
4. **Itens e Totens**: Embaralhe os baralhos de itens e tiles.

## **5. Detalhamento da Jogabilidade**
### **5.1 Movimentação**
- Os jogadores movem-se com base na rolagem do **Dado Amarelo**.
- No primeiro movimento, o jogador escolhe uma direção e adiciona um tile ao tabuleiro.
- Caso o jogador encontre um **tile desconhecido** durante seu movimento, deve interromper sua movimentação e revelar um novo tile.

### **5.2 Combate (PvP e Armadilhas)**
- **Antes da Chave do Portão ser descoberta**, jogadores não podem batalhar entre si.
- Após a chave ser descoberta, sempre que dois ou mais jogadores estiverem no mesmo tile, inicia-se uma batalha.
- **Resolução de Combate:**
  - O jogador atacante lança o **Dado Vermelho** (ataque).
  - O jogador defensor lança o **Dado Azul** (defesa).
  - Se o valor da defesa for maior ou igual ao ataque, o defensor não recebe dano.
  - Se o ataque for maior que a defesa, o defensor perde pontos de vida equivalentes à diferença.

**Consequências do Combate:**
- Se o atacante perder a batalha sem morrer, ele pode seguir seu caminho.
- Se um jogador for derrotado (0 HP), retorna ao ponto inicial e perde todos os seus itens.
- Se o jogador derrotado possuía a **Chave do Portão**, ela retorna ao seu tile de origem (caso tenha morrido para uma armadilha) ou passa para o jogador vencedor (caso tenha morrido para outro jogador).

### **5.3 Totens e Teletransporte**
- Totens permitem teletransporte entre si caso mais de um tenha sido revelado.
- Para usar um totem, o jogador deve gastar uma **Pedra Mágica**.
- O teletransporte encerra a movimentação do turno.

### **5.4 Tiles com Baús**
- Ao passar por um **tile com baú**, o jogador pode pegar uma carta de item.
- Um mesmo jogador **não pode pegar itens do mesmo baú em dois turnos consecutivos**.
- Para pegar um novo item do mesmo baú, o jogador deve sair do tile e retornar em um turno posterior.

## **6. Exemplo de Rodadas**
### **Exemplo 1 - Movimentação e Exploração**
1. O jogador A rola **5** no **Dado Amarelo**.
2. Move-se **4 espaços** em um caminho já descoberto.
3. No **5º espaço**, encontra um **tile desconhecido** e deve interromper sua movimentação.
4. Revela um novo tile e encerra seu turno.

### **Exemplo 2 - Combate entre Jogadores**
1. O jogador A e o jogador B encontram-se no mesmo tile.
2. O jogador A (atacante) lança o **Dado Vermelho** e tira **6**.
3. O jogador B (defensor) lança o **Dado Azul** e tira **4**.
4. Como o ataque foi maior, o defensor perde **2 HP**.
5. O combate termina e o jogador atacante pode seguir seu caminho.

## **7. Condições de Vitória**
- O jogador que encontrar a **Chave do Portão** e levá-la até o local da saída vence o jogo.
- Se um jogador for derrotado enquanto carrega a chave, ela pode ser recuperada por outro jogador.

## **8. Itens e Seus Efeitos**
- **Ímã**: Retira a chave de um jogador e a devolve ao tile de origem.
- **Botas Estilosas**: Permite ignorar o dano de um **tile de armadilha**.
- **Capa da Invisibilidade**: Evita batalhas ao passar por outro jogador.
- **Energético**: Adiciona **+3 movimentos extras** no turno.
- **Frango Cru**: Rola-se um dado:
  - Se o valor for **maior** que a vida atual, o jogador **se cura** até esse valor.
  - Se for **menor**, o jogador perde vida equivalente ao valor do dado.
  - Este item **não pode matar um jogador**.
- **Dinamite**: Inflige **-2 HP** a um jogador-alvo.

## **9. Referência Rápida**
- **Movimentação**: Rola-se o **Dado Amarelo**.
- **Combate**:
  - Atacante rola **Dado Vermelho**.
  - Defensor rola **Dado Azul**.
  - Dano = Ataque - Defesa (se ataque for maior que defesa).
- **Exploração**: Novos **tiles** são revelados conforme os jogadores se movem.
- **Totens**: Permitem **teletransporte** ao custo de **Pedra Mágica**.
- **Chave do Portão**: Essencial para vencer o jogo.

---

Este manual foi desenvolvido para proporcionar clareza e acessibilidade às regras do **Caligo Quest**. Para mais informações ou sugestões, entre em contato com os desenvolvedores.
