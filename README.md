# Algoritmo Genético para o Problema da Mochila

Este projeto implementa um algoritmo genético para resolver o clássico problema da mochila. Ele utiliza bibliotecas como `pygame` para exibição visual e `openpyxl` para salvar resultados em um arquivo Excel.

---

## Índice

- [Algoritmo Genético para o Problema da Mochila](#algoritmo-genético-para-o-problema-da-mochila)
  - [Índice](#índice)
  - [Descrição do Problema](#descrição-do-problema)
  - [Requisitos](#requisitos)
  - [Funcionalidades](#funcionalidades)
  - [Como Usar](#como-usar)
  - [Estrutura do Código](#estrutura-do-código)
    - [Principais Funções](#principais-funções)
  - [Resultados](#resultados)
    - [Exemplo de Resultado](#exemplo-de-resultado)

---

## Descrição do Problema

O problema da mochila consiste em determinar quais itens devem ser incluídos em uma mochila de capacidade limitada, de forma a maximizar o valor total dos itens selecionados. Cada item possui um peso e um valor.

Este projeto usa um algoritmo genético para encontrar a melhor solução possível dentro de uma quantidade limitada de gerações.

---

## Requisitos

Antes de executar o projeto, certifique-se de ter as seguintes bibliotecas instaladas:

- `pygame`
- `matplotlib`
- `openpyxl`

Instale todas as dependências usando o seguinte comando:

```bash
pip install pygame matplotlib openpyxl
```

---

## Funcionalidades

1. **Geração Aleatória de Itens e Capacidade**:

   - Itens são gerados aleatoriamente com pesos e valores.
   - A capacidade da mochila também é aleatória.

2. **Algoritmo Genético**:

   - Seleção por torneio.
   - Cruzamento com ponto único.
   - Mutação com taxa ajustável.

3. **Visualização**:

   - Exibição do progresso do algoritmo usando gráficos no `pygame`.

4. **Exportação de Resultados**:
   - Salva os resultados em um arquivo Excel formatado.

---

## Como Usar

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/genetic-algorithm-knapsack.git
   ```

2. Navegue para o diretório do projeto:

   ```bash
   cd genetic-algorithm-knapsack
   ```

3. Execute o script principal:
   ```bash
   python main.py
   ```

---

## Estrutura do Código

### Principais Funções

- **`randomize_items_and_capacity`**:
  Gera aleatoriamente os itens (peso e valor) e a capacidade da mochila.

- **`fitness`**:
  Calcula a aptidão de um indivíduo com base nos itens selecionados e na capacidade da mochila.

- **`initialize_population`**:
  Cria uma população inicial de indivíduos aleatórios.

- **`tournament_selection`**:
  Seleciona o melhor indivíduo de um grupo aleatório para reprodução.

- **`crossover`**:
  Realiza o cruzamento de dois pais para gerar um novo indivíduo.

- **`mutation`**:
  Introduz pequenas alterações em um indivíduo para manter a diversidade genética.

- **`save_to_excel`**:
  Salva os resultados do algoritmo genético em um arquivo Excel formatado.

- **`draw_plot`**:
  Exibe gráficos em tempo real com o progresso do algoritmo.

---

## Resultados

Ao final da execução do algoritmo genético:

- **Itens Selecionados**: Uma lista dos itens escolhidos, com seus respectivos pesos e valores.
- **Fitness Máxima**: O valor total dos itens selecionados.
- **Geração Ideal**: A geração onde a melhor solução foi encontrada.
- **Arquivo Excel**: Os resultados são exportados para um arquivo Excel chamado `genetic_algorithm_results.xlsx`.

### Exemplo de Resultado

- **Capacidade da Mochila**: 150
- **Itens Selecionados**:
  - Item 1 (Peso: 10, Valor: 15)
  - Item 2 (Peso: 5, Valor: 8)
- **Fitness Máxima**: 120
- **Geração Ideal**: 45

---

