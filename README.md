# NewProject
Study
# GitHub


### Comando para gerar uma chave SSH:
ssh-keygen -t ed25519 -C "kerlesalves@gmail.com"

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