# Resolução do Desafio: BFS vs DFS em Labirinto Complexo

Este repositório/notebook contém a implementação completa do desafio proposto, incluindo:

- Criação de **labirintos densos**
- Suporte a **movimentos diagonais**
- Uma proposta teórica e prática para análise de **complexidade Big-O**

---

## Parte A — Modificações no Labirinto e Algoritmos

Nesta etapa, foram realizadas as adaptações necessárias no ambiente e nos algoritmos para suportar:

- maior densidade de obstáculos no labirinto;
- movimentação em mais direções (incluindo diagonais, quando aplicável);
- comparação entre estratégias de busca (**BFS** e **DFS**) no contexto proposto.

---

## Parte B — Proposta de Análise Big-O

Para verificar na prática a complexidade esperada (como **O(V + E)**), propomos duas abordagens complementares:

### 1) Análise baseada em tempo de computação

**Método**
- Executar os algoritmos em labirintos de tamanho **N × N** (ex.: `10, 20, 40, 80, 160`).

**Análise**
- Como o número de estados **V** cresce aproximadamente com **N²**, o tempo deve ser analisado/plotado em função de **N²**.
- Se a curva **tempo × N²** for aproximadamente linear, isso sustenta a complexidade teórica.

### 2) Análise baseada em consumo de memória (cache)

**Conceito**
- O **DFS** tende a apresentar melhor **localidade espacial**, pois aprofunda a exploração em vizinhos próximos, mantendo dados “quentes” na cache (L1/L2) por mais tempo.

> Observação: essa análise pode ser complementada com medições via ferramentas de profiling (quando disponível), comparando padrões de acesso à memória entre BFS e DFS.

---

## Integrantes do Grupo

- **Pedro Henrique Teofilo Cunha** — **RA:** G9870F9  
- **Fernando Ariel da Silva Paulino** — **RA:** F358267  
- **Lucas Nascimento Pan** — **RA:** R062EC3  
- **Gabriel do Santos Marçal** — **RA:** G892AA4  
- **Rodrigo Froes Messias** — **RA:** G578CI8
