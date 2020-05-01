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

A primeira ação é criar um branch onde será desenvolvida a primeira feature:

```
git checkout -b feature/pagina-basica
```

Como feature inicial criaremos a página básica, composta da estrutura básica do html e todos os elementos definidos na parte 1 do curso. Esses elementos são:

- A estrutura obrigatória do html.
- As configurações do head.
- Um cabeçalho composto por um header e um banner.
- Logo abaixo do cabeçalho algumas informações sobre serviços.
- Um arquivo .css aplicando um estilo a essa estrutura inicial.

Além disso, o projeto deverá atender ao requisitos e utilização dos seguintes recursos/elementos:
- Utilizar tags h1 e p; :heavy_check_mark:
- Utilizar negrito e tag strong; :heavy_check_mark:
- Ênfase em textos com itálico e tag em; :heavy_check_mark:
- Informar ao navegador a versão do html utilizado, com a tag adequada; :heavy_check_mark:
- Informar ao navegador o idioma utilizado; :heavy_check_mark:
- Informar ao navegador o charset utilizado; :heavy_check_mark:
- Definir um título principal para a página; :heavy_check_mark:
- Aplicar estilos à página utilizando recursos de:
	- alinhamento; :heavy_check_mark:
	- tamanho de fonte; :heavy_check_mark:
	- cores e textos; :heavy_check_mark:
	- cores de fundo; :heavy_check_mark:
- Ajustar tamanho dos elementos utilizando tags; :heavy_check_mark:
- Configurar espaçamento e externo dos elementos; :heavy_check_mark:
- Criar listas; :heavy_check_mark:
- Aplicar o conceito de classes aos elementos; :heavy_check_mark:
- Dividir seções no arquivo de forma básica; :heavy_check_mark:
- Alterar o comportamento dos elementos; :heavy_check_mark:

## 1.1 Enviando as alterações para o Github

Atendido a todos os casos de uso anteriores, os próximos passo são:

- Merge do branch `development` com a feature; :heavy_check_mark:
- Efetua alguns testes; :heavy_check_mark:
- Checkout na `master` e merge com a `dev`; :heavy_check_mark:
- Gera a versão; :heavy_check_mark:
- Realiza o push; :heavy_check_mark: