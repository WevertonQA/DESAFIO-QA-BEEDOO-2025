#Users Story

## US-001 Cadastro de Curso

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

### Desejo

Eu, como administrador do módulo de curso <br>
Quero visualizar todos os cursos cadastrados em uma lista organizada <br>
Para consultar rapidamente as informações de cada curso (nome, descrição, instrutor, vagas, Tipo de Curso).

### Regras de Negócio:

1. A lista deve exibir todos os cursos cadastrados.
2. Cada curso deve ser mostrado em formato de card com as informações principais.
3. Se não houver cursos cadastrados, deve ser exibida mensagem informativa.
4. O administrador deverá ter a opção de excluir curso

---

## Evidências

**[Link evidências](https://drive.google.com/drive/folders/1rbYi7miKIfaSbp3tF1sEkUbtEtWdU5u0?usp=sharing)**  
**[Link para planilha de Casos de Teste (Google Sheets)](https://docs.google.com/spreadsheets/d/1V3RQUQzOYD9jRXwoGJ6UT6IduTA_2P_UNolllkhnPoE/edit?usp=drive_link)**  
**[Link para planilha de Relatório de Testes)](https://docs.google.com/spreadsheets/d/1AQGmC9ZMNhMidSW97ihXg7Qucfez20pELPL78ohKepA/edit?usp=drive_link)**  
**[Relatório de Bugs](https://docs.google.com/spreadsheets/d/1EXpasn3eziw9Jg-70PvdNyHjh_uGNsMmtVyYNtblpu4/edit?usp=drive_link)**  

---

## Passo a Passo de Execução

1. Acesse o link da aplicação.  
2. Crie um curso de teste preenchendo todos os campos obrigatórios.  
3. Verifique se o curso aparece na listagem após salvar.  
4. Teste a exclusão de um curso e observe se ele é realmente removido.  
5. Registre evidências visuais e resultados obtidos.  

---


**Weverton Hnrique Ramalho dos Santos**  
QA Júnior – Desafio Beedoo 2025  
wevertonsantos.qa@gmail.com
