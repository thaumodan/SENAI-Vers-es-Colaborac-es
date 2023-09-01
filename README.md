```
# SENAI-Versoes-Colaboracoes

readme de exemplo
```



# Passos para Configurar o GitHub e Iniciar um Projeto

Para começar o processo de desenvolvimento vamos criar a estrutura inicial do Código-Fonte, mas primeiro é necessário identificar o _usuário_ e seu _e-mail_, então após já instalado o programa na maquina:

1º.  Crie uma _pasta_* em sua maquina para armazenar o projeto. Esta pasta será o seu "_Repositório Local_**";

2º. Abra a pasta criada (que neste momento estará vazia) então clique na área em branco com o botão direito do mouse, assim um menu deve abrir, nele será possível encontrar a opção: “_Git Bash Here_“;

3º. Ao clicar em “_Git Bash Here_“ um terminal (Prompt de Comando) abrirá;

4º. Após aberto o terminal (Prompt de Comando), na sua maquina, digite **git config** e informe um _nome de usuário_ e _e-mail_



**COMANDO: git config**



Exemplo:

git config --global user.name “Fulano de Tal“                      Para usuário

git config --global user.email “fulanodetal@email.com“             Para e-mail



5º. Em seguida, vamos inicializar o _Repositório Local_ digitando **git init**



**COMANDO: git init**



Exemplo:
git init         
(Após digitado no terminal, pressione “Enter“ para executar o comando)

Uma vez executado, será criada uma pasta*** chamada **_.git_* com subdiretórios, desse modo transformando o diretório atual em um _repositório do Git_. Agora, dentro do _Repositório Local_ haverá uma subpasta do Git (.git).

.

.

\* Neste momento esta pasta é apenas um _arquivo comum da maquina do desenvolvedor_

\** O repositório local é a pasta/diretório da sua máquina com o seu projeto, mas **ATENÇÃO**, $para$ $efeito$ $didático$, a pasta só deve ser considerada na qualidade de _Repositório Local_ quando a(s) alteração(ões) for(em) efetivamente registrada(s) e salva(s) por meio do comando **git commit** que veremos melhor mais adiante.

*** Esta pasta pode estar oculta no sistema, então é interessante torná-la visível. Dentro da pasta criada (_repositório local_), vá na aba “Exibir” e marque a caixinha de seleção “Itens ocultos”. Dica: Marque também a caixinha “Extensões de Nomes de Arquivos“




# Incluindo e Rastreando um Arquivo no Repositório Local


#### Incluindo Arquivo:

Para incluir um arquivo dentro do _Repositório Local_ abra a pasta do _Repositório_; na área em branco, com o botão direito do mouse, clique em “Novo” e, em seguida, em “Documento de Texto” para criar um arquivo com extensão _.txt_ dentro da pasta.


OBS: Caso já tenha algum arquivo pronto, basta arrastá-lo para dentro do _Repositório Local_.


NOTA: Ao adicionar este arquivo na pasta significa que houve uma _alteração_, mas o arquivo que foi criado ou colocado dentro do _Repositório Local_ ainda não está sendo rastreado pelo Git

#### Rastreando Arquivo no Repositório Local:



`Etapa 1 de 2`

Para Rastrear um arquivo, inicialmente faremos uso do comando **git status** que serve para acompanharmos as alterações que foram realizadas.


**COMANDO: git status**  
(Após digitado no terminal, pressione “Enter“ para executar o comando)


Uma vez executado, o terminal (Prompt de Comando) informará que nenhum arquivo foi _registrado/salvo_ (_committed_) ainda. Também informará que foi detectado um arquivo no _Repositório Local_, mas que este arquivo ainda não está sendo rastreado pelo Git


Então, agora vamos fazer com que o Git passe a rastrear o arquivo _.txt_ que foi criado (ou o arquivo que foi arrastado/colado na pasta), e cuja pasta estará sendo usada como _Repositório Local_. Para isso usaremos o comando **git add**.


**COMANDO: git add**

Exemplo:
git add \[nome-do-arquivo.txt]

Esta ação transporta o arquivo para um ponto intermediário e seguro entre a maquina do desenvolvedor e o _Repositório Local_, esta área e chamada de **STAGING**\*



**DICA:** É sempre interessante, após se fazer alguma alteração, que se verifique, atraves do comando **git status**, a situação atual até para confirmar (e se localizar em relação ao ponto em que se pretende estar e o ponto em que realmente se está)

**DICA 2:** Faça uso do comando **git log** para acompanhar as alterações que já foram salvas/registradas no _Repositório Local_

**DICA 3:** Caso queira visualizar alguma alteração basta fazer uso do comando **git show [numero-do-commit**]** 

.

.

\* É nesta área que se pode fazer uma revisão na(s) alterção(ões) antes de gravá-la(s)/salvá-la(s) no _histórico de alterações_

\** Sempre que um arquivo é registrado (após o uso do comando **git commit**) é gerado um numero de registro que serve como identificador


`Etapa 2 de 2`

Após adicionar a(s) alteração(ões) na _staging_ e revisá-la(as), agora é a hora de concluir o procedimento de registro/salvamento da(s) alteração(ões) no hitórico, para isso usaremos o comando **git commit**.


**COMANDO: git commit -m**

É sempre interessante que após o comando **git commit** seja inserido um breve comentário explicativo com o intuito de facilitar e agilizar o acompanhamento das alterações realizadas

Exemplo:

git commit -m "[comentário-explicativo]"


Por fim, depois que uma ou mais alterações estão na área _staging_, é só executar este comando e, a alteração será salva/registrada no hitórico do projeto.
