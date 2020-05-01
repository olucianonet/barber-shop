# Barber SHOP

Uma landing page criada para testar os conhecimentos obtidos nos cursos de HTML5 /CSS3:
- HTML5 e CSS3 parte 1: A primeira página da Web
- HTML5 e CSS3 parte 2: Posicionamento, listas e navegação
- HTML5 e CSS3 parte 3: Trabalhando com formulários e tabelas
- HTML5 e CSS3 parte 4: Avançando no CSS

Versionamento realizado utilizando os conhecimentos obtidos nos cursos de git:
- Git e Github: Controle e compartilhe seu código
- Git e Github: Estratégias de ramificação, Conflitos e Pull Requests

## Objetivo:

O objetivo é criar uma landing page a partir do conteúdo estudado nos cursos de
html/css. 

O projeto será composto de várias fases, cada uma representando o conteúdo 
estudado em cada curso. Desta forma, o projeto estará em constante evolução.

Inicialmente teremos as seguintes etapas:

0. Criação do repositório
1. Página básica: Criando a estrutura e preenchendo o conteúdo básico.
2. Posicionamento, listas e navegação.
3. Trabalhando com formulário e tabelas.
4. Melhorando o CSS.

## 0. Criação do repositório

Como primeiro passo, é necessário criar o projeto no Github, já que esse 
projeto ficará hospeado lá. 

Após a criação do repositório no Github, é necessário realizar o pull dos dados para o ambiente local. 

Assim, crie a pasta que irá conter o projeto, e execute os seguintes comandos:

```
git init
git remote add origin ulr-do-projeto-no-github
touch README.md
git add . 
git commit -m 'Commit inicial'
git push origin master
git tag -a v0.1.0 -m 'Commit inicial'
git push origin v0.1.0
```

Neste momento, temos uma versão inicial, contendo apenas um README com algumas
instruções do projeto.

### 0.1 Git Flow

A forma de organização de desenvolvimento do projeto será baseada no Git Flow.
Desta forma, a partir do repositório `master` já existente, daremos início em
mais um branch chamado `development`. 

No branch `development` ficará o conteúdo principal durante o desenvolvimento,
composto pelo arquivo README.md, contendo a descrição das atividades do projeto e as features implementas.

Além do branch development, para cada nova feature implementada será criado um
novo branch, que ao final da implementação, sofrerá um merge com o development.

A cada implementação, será lançada uma nova release/tag e enviada para o origin.

Hotfixes serão tratados em branch específicos. 

Caso aconteça na master o merge deverá ocorrer diretamente nela e posteriormente o development irá receber o merge do hotifx. 

Caso o hotfix ocorrá na release, a correção poderá ser implementada diretamente
nela, sem a necessidade de criar um branch específico.

Assim, vamos criar o novo branch `development`:

```
git checkout -b development
```

A partir de agora, determinadas as implementações, para cada feature será criado um novo branch.

## 1. Página Básica

Como feature inicial criaremos a página básica, composta da estrutura básica do html e todos os elementos definidos na parte 1 do curso.

```