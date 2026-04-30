# Simulação de Irrigação por Aspersão com Base em Lançamento Oblíquo

## Objetivo

Este projeto visa a simulação do comportamento de um sistema de irrigação por aspersão, utilizando princípios de cinemática do lançamento oblíquo para determinar o alcance das gotas de água e otimizar a distribuição de aspersores em uma área retangular.

---

## Conceitos Teóricos

O modelo físico adotado considera o lançamento de partículas sob ação da gravidade, sendo descrito pelas equações do movimento:

* Movimento horizontal:

  x(t) = v₀ · cos(θ) · t

* Movimento vertical:

  y(t) = h + v₀ · sin(θ) · t - (1/2) · g · t²

Onde:

* v₀ = velocidade inicial
* θ = ângulo de lançamento
* h = altura inicial
* g = aceleração da gravidade

O tempo de voo é obtido resolvendo a equação quadrática associada ao movimento vertical.

---

## Funcionamento

O código segue as seguintes etapas:

1. Entrada de dados da área:

   * Comprimento (C)
   * Largura (L)

2. Definição dos parâmetros:

   * Tipos de bombas (A, B, C)
   * Velocidades associadas
   * Ângulos de lançamento

3. Cálculo do tempo de voo e alcance para cada combinação:

   * Resolução da equação do movimento vertical
   * Determinação do alcance horizontal

4. Seleção da melhor configuração:

   * Maior alcance obtido

5. Dimensionamento do sistema:

   * Cálculo do número de aspersores necessários

6. Visualização:

   * Trajetória das gotas
   * Distribuição dos aspersores na área

---

## Visualização de Resultados

O programa fornece:

* Tempo de voo das partículas
* Alcance máximo para cada configuração
* Melhor combinação de bomba e ângulo
* Número total de aspersores necessários
* Visualização gráfica da trajetória e cobertura

---

## Como Executar?

1. Instale as bibliotecas necessárias:

```bash
pip install numpy matplotlib
```

2. Execute o código:

```bash
python main.py
```

3. Insira os valores solicitados no terminal.

---

## Exemplo de Uso

Entrada:

* Comprimento: 50 m
* Largura: 30 m

Saída:

* Melhor configuração de bomba e ângulo
* Alcance máximo
* Quantidade de aspersores
* Gráficos de trajetória e distribuição

---

## Limitações

* Não considera resistência do ar
* Assume lançamento ideal
* Não modela interação entre jatos de água
* Considera terreno plano e uniforme

---

## Possíveis Extensões Futuras

* Inclusão de resistência do ar
* Otimização automática via algoritmos
* Integração com dados reais de irrigação
* Aplicação de aprendizado de máquina para previsão de desempenho

---

## Contexto Acadêmico

Este projeto aplica conceitos de:

* Cinemática de partículas
* Lançamento oblíquo
* Modelagem matemática
* Simulação computacional

Sendo relevante para áreas como:

* Engenharia mecânica
* Engenharia agrícola
* Engenharia ambiental

---

## Tecnologias Utilizadas

* Python
* NumPy
* Matplotlib

---
