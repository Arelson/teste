## Inicializa o git na pasta
* git init 

## inicia as configuração do git
* git config:
### Niveis de atuação da configuração
    * --system = afeta todos os compuatdores
    * --global = afeta para mim e todos os meus projetos
    * --local = afeta apenas no projeto atuas e usuarios do projeto

    Configuração do usuario
    + user.name = registra ou altera o nome de usuario
    + user.email = registra o e-mail para associar a conta
    + -l = acessa todas as informaçoes padrao e as registradas
    + core.editor (nome do editor) = altera o editor de texto para o uso do git

## Adiciona o arquivo desejado na are de stage
- git add (nome do arquivo):

### Parametros
* . = Adiciona todos os arquivos e alterações na staged

## Consulta o estado dos arquivos
-git status

## Torna rastreavel para o git os arquivos
* git commit *:
    ### Parametros
    * -m 'texto' = adiciona uma mensagem no commit
    * -am 'texto' = faz o commit em arquivos que ja estao rastreaveis pulando o processo de add no stage (a = add e m = mensagem)
* git commit comando 'texto XXX'
    - #n = referencia a issues correspondente ao numero
    - closes #n° = fecha a issues referente ao numero
    - fixes #n° = fecha a issues referente ao numero dizenco que o erro apontado foi corigito

## Comando que consulta o historico de mudanças
* git log *
	flags:
	* --graph = mostra a linha do tempo dos commits do projeto
	* --oneline = simlifica o graph(pode usar varias flags no msm coamndo)

## Comando que acessa versoes anteriores do projeto
-git checkout (Codigo do commit)
-git checkout * (nome da ramificação) = troca a linha do tempo do projto em que se trabalha
	comandos:
	* -b = cria uma branch nova e automaticamente entra nela

## Comando que traz o projeto do github para a maquina
* git clone (link do repositorio)
    comando que lista os arquivos do projeto
    -ls

## Comando que envia arquivos para o github pois so o commit(so faz local) não adianta
* git push
* git push origin (nome da branch) = envia uma nova branch para o github

## comando que traz os arquivos de github para a maquina do usuario
* git pull

## comando que ramimifica a linha principla do projeto
* git branch * (nome da ramificação)
	comando:
	* -d = apaga a branch criada
    * -a = lista todas as branchs e as remotas
* git branch  = lista as ramificaçoes criadas

## Comando que adiciona a ramificação na linha principal do projeto
* (Pra juntar primeiramente é necessario esta na main(linha principal))
    * git merge (nome da ramificação)

## comando similar ao merge porem faz com que não aconteça o commit do merge recursivo e reescreve o commit 
* feito na branch, tornando o merge fast foward(necessario acessar branch nova pra realizar o comando)
* git rebase (main ou otra branch que ira receber)
* git rebase --continue". continua o rebase depois da resolução do conflito
* git rebase --skip". pula o rabase sem a resolução do conflito
* git rebase --abort". cancela o rebase feito

