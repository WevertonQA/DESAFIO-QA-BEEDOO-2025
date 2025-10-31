

## US-001 Cadastro de Curso

 **PO Responsável:**  Ana Sousa <br>
 **Sprint:** 2 <br>
 **Prioridade de Negócio:**  Alta | <br>
 **Pontos Estimados:**  5 

### Desejo

Eu, como **usuário administrador** do módulo de curso, <br>
Quero **cadastrar novos cursos por meio de um formulário**, <br>
Para que **fiquem disponíveis na listagem e possam ser visualizados por outros usuários.**

---

### Regras de Negócio

1.  O sistema deve permitir o cadastro de um novo curso preenchendo os campos obrigatórios.
2.  **Campos obrigatórios:** Nome do Curso, Descrição do Curso, Instrutor, Datas Incício e Fim, Número de Vagas e Tipo de Curso (Endereço ou Online dependendo do tipo de curso).
3.  **Campo Nome do Curso:** Deve conter no mínimo 3 caracteres.
4.  **Campo Instrutor:** Deve conter no mínimo 3 caracteres, excluindo caracteres númericos e especiais.
5.  **Campo Número de Vagas:** Deve aceitar apenas números positivos.
6.  **Campo Descrição do Curso:** Deve conter no mínimo 10 caracteres.
7.  **Campo Data de Fim:** Não pode ser anterior à Data de Início.
8.  Ao selecionar um tipo de curso, o administrador deverá obrigatóriamente escolher o modelo de ensino (Online ou Presencial)
9.  Adicionar capa para o curso é opcional, mas se preenchido deverá conter dados formato de link
10.  O **botão "Salvar"** deve permanecer inativo até que todos os campos obrigatórios sejam preenchidos corretamente.
11. Caso algum campo seja preenchido incorretamente, o sistema deve exibir uma mensagem de erro específica abaixo do campo.
12. O curso cadastrado deve aparecer na listagem de cursos imediatamente após o salvamento.
13. O sistema deve impedir o cadastro de cursos com nomes duplicados.

---

### Critérios de Aceitação (Gherkin)

#### Cenário 1: Cadastrar curso com sucesso

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
