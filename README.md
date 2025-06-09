# 🧬 Problema das 8 Rainhas com Algoritmo Genético #
Este repositório contém a implementação de um algoritmo genético para resolver o clássico problema das 8 rainhas, com variações e experimentações nos parâmetros do algoritmo para avaliar seu desempenho.

## 📌 Descrição do Problema 
O problema das 8 rainhas consiste em posicionar 8 rainhas em um tabuleiro de xadrez 8x8 de forma que nenhuma delas se ataque mutuamente (nem na mesma linha, coluna ou diagonal).

## ⚙️ Estratégia Utilizada 
O algoritmo genético segue os seguintes parâmetros iniciais:
- Representação (Genótipo): Permutação de string de bits
- Inicialização: População gerada aleatoriamente
- Tamanho da população: 100 indivíduos
- Seleção de pais: Ranking – melhor de 2 entre 5 escolhidos aleatoriamente
- Recombinação: Operador “cut-and-crossfill crossover”
- Probabilidade de recombinação: 90%
- Mutação: Troca de genes (swap)
- Probabilidade de mutação: 40%
- Seleção de sobreviventes: Substituição do pior indivíduo
- Número de filhos por geração: 2
- Condição de parada: Solução encontrada ou 10.000 avaliações de fitness

## 🧪 Segunda Parte – Variações e Melhorias
O projeto inclui uma segunda fase com modificações nos seguintes aspectos para avaliar impacto no desempenho:
- Representação alternativa do indivíduo
- Novos operadores de recombinação e mutação
- Seleção de pais por roleta
- Seleção de sobreviventes por geração ou pior
- Variações no tamanho da população (10, 30, 50, 70, 120, 200)
- Melhoria na função de fitness

## 📊 Avaliação e Métricas 
Para cada configuração:
- Realização de 30 execuções independentes

### Avaliação de: ###
- Número de execuções que convergiram
- Iteração média e desvio padrão de convergência
- Quantos indivíduos convergiram por execução
- Fitness médio da população por execução
- Gráficos de convergência (média e melhor indivíduo por iteração)
-Fitness médio final (média e desvio padrão)
-Iterações até toda a população convergir (análise adicional)

