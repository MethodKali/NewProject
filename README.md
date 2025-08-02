# NewProject
Study
# GitHub


### Comando para gerar uma chave SSH:
ssh-keygen -t ed25519 -C "email@email.com"

### Comando para copiar a chave SSH gerada:
eval "$(ssh-agent -s)"

1. SSH nada mais é do que um protocolo de segurança que consiste na criptografia de informações. 

2. Usando a chave SSH gerada como pass phrase do GitHub podemos fazer a conexão entre o computador e o Git e todos os projetos que forem adicionados ao repositório que estejam na máquina podem ser atualizados a medidas que haja alterações feitas

3. Após criarmos nosso primeiro repositório no Git podemos trazer esses arquivos anexados no repositório através do link gerado para conexão SSH.

4. Com esse link podemos trazer os arquivos armazenados no Git através do comando:

### Comando para trazer arquivos armazenados no GitHub:
git clone git@github.com:Usuario/Projeto.git

1. Após isso podemos perceber que uma pasta foi criada, e navegarmos por ela observamos que os mesmos arquivos armazenados noo git se encontra lá

2. O arquivo README.md armazena o texto de instruções anexadas no git com finalidade de orientações relacionadas ao código. Podemos abrir esse arquivo no visual code e fazer algumas alterações que futuramente será carregada para o git.

3. Após adicionar os textos dentro do arquivo README.md podemos verificar no GitBash que o arquivo foi modificado, usando o comando:

### Comando para verificar o status do GitHub:
git status

1. A informação em vermelho do arquivo README.md modificado indica que houve modificação porém o arquivo não está pronto para ser commitado. Para preparar nosso arquivo para um futuro commit podemos escrever o comando:

### Comando para preparar o arquivo que será comittado:
git add .

1. Ao verificar o status do git podemos observar que o arquivo README.md está desrtacado com a cor verde. Isso indicar que nosso arquivo está pronto para ser commitado.


2. Para fazer o commit local do nosso arquivo codamos:

### Comando para commitar o arquivo local:
git commit -m "NomeCommit"

1. Para verficar os processos de comunicação entre o Git e o PC podemos escrever o seguinte comando:

### Comando para verificar processos de modificações realizadas de arquivos:
git log

1. Nosso commit local está feito. Agora vamos fazer o commit usando a comunicação ssh. Para isso escrevemos:

### Comando para enviar alterações ao GitHub
git push origin HEAD

1. Prontinho as alterações feitas no arquivo README.md foram carregadas para o Git.

# Branches e Tags


## Branches

Agora que aprendemos sobre como fazer alterações em arquivos usando o comando commit vamos entender como funciona a lógica por trás das branches.

Antes de tudo devemos entender nosso repositório no Git como uma linha do tempo, a branch principal ou a main branch. Essa linha do tempo possui alguns marcos históricos que vamos chamá-los de commits, ou seja toda a alteração que ocorreu na main branch é marcada por um commit. 

Existem casos que queremos apenas fazer alguns teste no nosso repositório principal sem que as alterações não interfira no funcionamento do nosso código. Dessa forma criamos uma nova linha do do tempo paralela a linha do tempo principal e todas as alterações feitas nessa nova linha do tempo não irá interferir na main branch.

Para criar uma nova branch escrevemos no git bash:

### Criar Branches
git branch NomeBranch

Para verificar as branchs já existentes escrevemos:
### Verificar branchs existentes
git branch

Para selecionar uma branch existente escrevemos:
### Selecionar branch existente
git checkout NomeBranch

#### Nota: Para cada branch selecionada a criação de commits seguem a mesma lógica.

## Tags
O processo de criação de branchs para testes do projetos, adição de commits e após tudo estar ok é realizado o merge para que a branch teste passa a fazer parte da main branch. Esse processo é destacado como uma atualização da main branch em um numero de versão. Essa versão criada é o que chamamos de Tags para situar as atualizações realizadas na main branch

# Pull Requests

A comunidade Git Hub é formada por desenvolvedores que trabalham em grupos com o objetivo de lançar projetos sendo eles rentaveis ou open source.

Na aba Pull Requests os desenvolvedores comentam, avaliam as atualizações realizadas, indicam possiveis bugs em resumo, é um espaço para coleta, manutenção, avaliação e feedbacks




