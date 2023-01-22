# Módulo 4 - Sistema Resilia
<h2>Projeto Individual do Módulo 4 (Banco de Dados) dos Projeto Programadores Cariocas.</h2>

A proposta do projeto consiste em modelar um banco de dados que armazene as entidades CURSOS, TURMAS E ALUNOS.
Além disso, é necessário para a realização a resposta a três perguntas:
<blockquote>Existem outras entidades além dessas três?</blockquote>
<blockquote>Quais são os principais campos e tipos?</blockquote>
<blockquote>Como essas entidades estão relacionadas?</blockquote>

<h2>Respostas:</h2>

<h3>Existem outras entidades além dessas três?</h3>
Para a criação do modelo foi necessário criar as entidades Facilitador e Disciplinas além das pré determinadas.

<h3>Quais são os principais campos e tipos?</h3>
Aluno_ID, Facilitador_ID, Turma-ID, Curso_ID e Disciplina_ID são do tipo PK INT;
Mensalidade é do tipo float;
Data_de_Nascimento e Data_Inicio são do tipo date e datetime, respectivamente;
Os outros campos são do tipo varchar.

<h3>Como essas entidades estão relacionadas?</h3>
ALUNO está relacionada a TURMA no tipo (1,1), sendo adicionada a chave estrangeira FK_Curso_ID int;<br>
TURMA está relacionada a ALUNO no tipo (1,N);<br>
A relação de TURMA e FACILITADOR é (N,N), portanto foi criada uma entidade TURMA_FACILITADOR entre elas;<br>
A relação entre TURMA e CURSO é de (1,1) e (1,N), respectivamente, sendo adicionada a chave estrangeira CURSO_ID na entidade TURMA;<br>
A relação entre FACILITADOR e DISCIPLINA é de (1,1) e (1,N), respectivamente, sendo adicionada a chave estrangeira DISCIPLINA_ID na entidade FACILITADOR;<br>
A relação de CURSO e DISCIPLINA é (N,N), portanto foi criada uma entidade CURSO_DISCIPLINA entre elas.<br>

<h2>Requisitos Extras:</h2>
Preparar os scripts que vão criar o banco de dados proposto e adicionar uma pasta chamada SQL com os arquivos.

<h2>Print do Modelo</h2>

![Projeto Individual - Módulo 4](https://user-images.githubusercontent.com/112409835/213898359-cfbf899f-f9b4-4f83-a6b0-b73d077737f3.jpg)

