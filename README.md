#Users Story

## US-001 Cadastro de Curso

 **PO Responsável:**  Ana Sousa <br>
 **Sprint:** 2 <br>
 **Prioridade de Negócio:**  Alta | <br>
 **Pontos Estimados:**  5 

### Desejo

Eu, como **administrador** do módulo de curso, <br>
Quero **cadastrar novos cursos por meio de um formulário**, <br>
Para que **fiquem disponíveis na listagem e possam ser visualizados por outros usuários.**

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

---

## US-002 Listar Curso

 **PO Responsável:**  Ana Souza <br>
 **Sprint:** 2 <br>
 **Prioridade de Negócio:**  Alta | <br>
 **Pontos Estimados:**  5 

### Desejo

Eu, como administrador do módulo de curso <br>
Quero visualizar todos os cursos cadastrados em uma lista organizada <br>
Para consultar rapidamente as informações de cada curso (nome, descrição, instrutor, vagas, Tipo de Curso).

Regra(s) de Negócio:

1. A lista deve exibir todos os cursos cadastrados.
2. Cada curso deve ser mostrado em formato de card com as informações principais.
3. Se não houver cursos cadastrados, deve ser exibida mensagem informativa.
4. O administrador deverá ter a opção de excluir curso
