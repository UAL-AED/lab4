# [Algoritmos e Estruturas de Dados 2020 2021](https://elearning.ual.pt/course/view.php?id=1787) - [UAL](https://autonoma.pt/)

## Laboratório 4

O objetivo deste laboratório é produzir uma implementação do tipo abstrato de dados Dicionário, através de uma tabela de dispersão aberta.

Este enunciado é acompanhado por um conjunto de ADTs, implementações de items (`aed_ds/dictionaries/item.py`), e um conjunto de exceções (`aed_ds/exceptions.py`).

Vai ser necessário criar o seguinte módulo:

- **`aed_ds/dictionaries/open_hash_table.py`**, que vai ter a classe `OpenHashTable`, com a implementação da tabela de dispersão aberta, de acordo com o ADT `Dictionary`, em `aed_ds/dictionaries/adt_dictionary.py`

A acompanhar o código segue também uma bateria de testes:

- `tests/dictionaries/test_open_hash_table.py` que testa a classe `OpenHashTable`

O laboratório é considerado completo quando todos os testes estiverem passados.

Os testes não são necessariamente exaustivos, pelo que o grupo de trabalho pode *acrescentar* testes, mas não pode alterar os que foram distribuídos.

Os testes pode ser executados de várias formas:

- Todos os testes do módulo
  - E.g., `python -m unittest tests.dictionaries.test_open_hash_table`
- Apenas um teste de uma classe
  - E.g., `python -m unittest tests.dictionaries.test_open_hash_table.TestOpenHashTable.test_size`
- Todos os ficheiros de teste
  - `python -m unittest discover tests`

## Datas

| Evento                        | Data                 |
| ----------------------------- | -------------------- |
| Disponibilização de enunciado | 15/05/2021           |
| Entrega                       | 30/05/2021, 23:59:59 |

## Regras

- O trabalho deve ser realizado em grupo, previamente registado no *e-learning*.
- O código produzido deverá estar disponível no repositório GitHub gerado pelo GitHub Classroom.
  - Podem ser criados vários *branches*, de acordo com o organização que o grupo de trabalho considerar mais conveniente.
  - Deve sempre existir um *branch* `main`, onde a versão final deverá ficar disponível.

## Entrega
A versão final do trabalho deve estar disponível na *branch* `main` do repositório até à hora limite de entrega. <span style="color: red">Não serão considerados *commits* com data posterior à data limite.</span>

A entrega deve também ser feita no *e-learning*, num ficheiro `zip` com todo o projeto.

## Atualização de enunciado

Repositório: <https://github.com/UAL-AED/lab3>

Para efetuar a atualização de enunciado:

1. Registar o repositório como `upstream` (só deve acontecer uma vez)
  
        git remote add upstream https://github.com/UAL-AED/lab4

2. Atualizar o `upstream` (sempre que existirem atualizações)

        git fetch upstream

3. Obter as alterações (e.g., ficheiro `README.md`)

        git checkout upstream/main README.md

### 2021/05/17 - Adiciona o módulo com o item de dicionário

    git fetch upstream
    git checkout upstream/main README.md
    git checkout upstream/main aed_ds/dictionaries/item.py

### 2021/05/21 - Adiciona `__init__.py` aos módulos de teste e remove exceção de `is_full` no ADT Dicionário

    git fetch upstream
    git checkout upstream/main README.md
    git checkout tests/__init__.py
    git checkout tests/dictionaries/__init__.py
    git checkout aed_ds/dictionaries/adt_dictionary.py

