#Lógica Matemática: Construção da Tabela Verdade em Python

#Estrutura da Tabela Verdade:
1.**( P\ ) Proposição de entrada 1**
2.**(Q\ ) Proposição de entrada 2**
3.**(R \ ) Proposição de entrada 3**
4.**(P_and_q) Conjunção de operador 'and'**
5.**(not_P_and_q) Negação de operador 'not'**
6.**(P_and_Q → R) Implicação**

#Funcionalidade: 
**Automoção por meio da utilização do módulo nativo python 'itertools' para mapear todas possibilidades para as variáveis P, Q, R.**
**Formatação limpa da interface do terminal: Usando tratamento (':<4' ... ':<6') para espaçamento das colunas e** 
**conversão booleana para caracteres tradicionais ('V' ... 'F')**

#Aplicação Prática:
**Na engenharia de software, tabelas verdade atuam no mapeamento de validação de dados**
import itertools
def exibir_tabela_verdade_completa():
    print("===TABELA VERDADE 100% COMPLETA===")
    print(f"{'P':<4} | {'Q':<4} | {'R':<4} | {'P ^ Q':<6} | {'¬(P ^ Q)'} | {'(P ^ Q) → R'}")
    print("-" * 55)

    valores = [True, False]


    for p, q, r in itertools.product(valores, repeat=3):
        p_and_q = p and q
        not_p_and_q = not p_and_q
        implicacao = not p_and_q or r
    
    #Formatando TRUE/FALSE para V/F
        f_p = 'V' if p else 'F'
        f_q = 'V' if q else 'F'
        f_r = 'V' if r else 'F'
        f_and = 'V' if p_and_q else 'F'
        f_not = 'V' if not_p_and_q else 'F'
        f_imp = 'V' if implicacao else 'F'

        print(f"{f_p:<4} | {f_q:<4} | {f_r:<4} | {f_and:<6} | {f_not:<6} | {f_imp}")

if __name__ == "__main__":
    exibir_tabela_verdade_completa() 