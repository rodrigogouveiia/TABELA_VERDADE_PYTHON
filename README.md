# Gerador de Tabela Verdade Completa em Python
Este projeto apresenta a construção automatizada de uma **Tabela Verdade Completa** com 3 proposições (`P` `Q` `R`) utilizando a linguagem Python. O objetivo é demonstrar a aplicação da **Lógica Proposicional** para mapeamento de validação de dados na engenharia de software.
## Funcionalidades
**Automação:** Utilização do módulo nativo python `itertools` para mapear todas possibilidades para as variáveis proposicionais `P, Q, R`.

Mapeamento de todas as 8 combinações possíveis das 3 variáveis ( `P` `Q` `R` ). Cada variável pode assumir dois estados lógicos ( `True` ou `False`), resultando no calculo matemático ($2^3$) = `8 combinações`. 

**Formatação Limpa:** Interface limpa do terminal usando tratamento de alinhamento (`:<4`, `:<6`) para espaçamento das colunas e conversão booleana para caracteres tradicionais True (`V`) False (`F`).
  
## Estrutura da Tabela Verdade:
1.**( P\ ) Proposição de entrada 1**

2.**(Q\ ) Proposição de entrada 2**

3.**(R\ ) Proposição de entrada 3**

4.**(P_and_Q) Conjunção de operador `and`**

5.**(not_P_and_Q) Negação de operador `not`**

6.**(P_and_Q → R) `Implicação`**

## Demonstração do Terminal
   <img width="405" height="189" alt="Screenshot_1" src="https://github.com/user-attachments/assets/84ec7918-b090-4758-87ec-d1fcaaef95a8" />

