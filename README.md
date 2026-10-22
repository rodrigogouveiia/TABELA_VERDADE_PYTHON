# Gerador de Tabela Verdade Completa em Python
Este projeto apresenta a construção automatizada de uma **Tabela Verdade Completa** com 3 proposições (\(P\), \(Q\) e \(R\)) utilizando a linguagem Python. O objetivo é demonstrar a aplicação da **Lógica Matemática** na estruturação de circuitos de validação de dados.
## Funcionalidades
* **Geração Binária Exaustiva:** Mapeamento de todas as combinações possíveis (8 cenários para 3 variáveis).* **Formatação Limpa:** Interface de terminal otimizada usando máscaras de alinhamento (`:<4`, `:<6`).
## Código Implementado
```pythonimport itertools
def exibir_tabela_verdade_completa():    print("=== TABELA VERDADE 100% COMPLETA ===")    print(f"{'P':<4} | {'Q':<4} | {'R':<4} | {'P ∧ Q':<6} | {'¬(P∧Q)':<6} | {'(P ∧ Q) → R'}")    print("-" * 55)        valores = [True, False]        for p, q, r in itertools.product(valores, repeat=3):        p_and_q = p and q        not_p_and_q = not p_and_q        implicacao = not_p_and_q or r                f_p = 'V' if p else 'F'        f_q = 'V' if q else 'F'        f_r = 'V' if r else 'F'        f_and = 'V' if p_and_q else 'F'        f_not = 'V' if not_p_and_q else 'F'        f_imp = 'V' if implicacao else 'F'                print(f"{f_p:<4} | {f_q:<4} | {f_r:<4} | {f_and:<6} | {f_not:<6} | {f_imp}")
if __name__ == "__main__":    exibir_tabela_verdade_completa()```
## Demonstração do Terminal
    ![Uploading Screenshot_1.png…]()
