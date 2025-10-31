# US-001 Cadastro de Curso

| **PO Responsável** | Ana Sousa |
| **Sprint** | 2 |
| **Prioridade de Negócio** | Alta |
| **Pontos Estimados** | 5 |

## Desejo

Eu, como **usuário administrador** do módulo de curso, <br>
Quero **cadastrar novos cursos por meio de um formulário**, <br>
Para que **fiquem disponíveis na listagem e possam ser visualizados por outros usuários.**

---

## Regras de Negócio

1.  O sistema deve permitir o cadastro de um novo curso preenchendo os campos obrigatórios.
2.  **Campos obrigatórios:** Nome do Curso, Descrição, Carga Horária.
3.  **Campo Nome do Curso:** Deve conter no mínimo 3 caracteres.
4.  **Campo Carga Horária:** Deve aceitar apenas números positivos.
5.  **Campo Descrição:** Deve conter no mínimo 10 caracteres.
6.  **Campo Data de Fim:** Não pode ser anterior à Data de Início.
7.  O **botão "Salvar"** deve permanecer inativo até que todos os campos obrigatórios sejam preenchidos corretamente.
8.  Caso algum campo seja preenchido incorretamente, o sistema deve exibir uma mensagem de erro específica abaixo do campo.
9.  O curso cadastrado deve aparecer na listagem de cursos imediatamente após o salvamento.
10. O sistema deve impedir o cadastro de cursos com nomes duplicados.

---

## Critérios de Aceitação (Gherkin)

### Cenário 1: Cadastrar curso com sucesso

```gherkin
Dado que o usuário está na página "Cadastrar Curso"
E preenche o campo "Nome do Curso" com "Introdução ao Teste de Software"
E preenche o campo "Descrição" com "Aprenda fundamentos e técnicas de QA"
E preenche o campo "Carga Horária" com "20"
E preenche o campo "Data de Início" com "01/10/2025"
E preenche o campo "Data de Fim" com "30/10/2025"
Quando o usuário clica em "Salvar"
Então o sistema exibe a mensagem "Curso cadastrado com sucesso"
E o curso "Introdução ao Teste de Software" aparece na listagem principal
