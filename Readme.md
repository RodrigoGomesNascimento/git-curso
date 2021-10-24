#Github

#Arquivo da aula de Git e Github

#modificar para aprender
#Este e o repositorio .
#saiba mais em [willianjusten.com.br](http://willianjusten.com.br)
#Gostou do curso quer mais ??
#estes e para testar.
#como configurar o git
gitconfig
gitconfig usuario
gitconfig do projeto(São onde guarda a informações.
git global.

comando para configurar o user global.

git config --global user.name "RodrigoGomesNascimento"

configurar o e-mail.

git config --global user.email "rgomes.nascimento@gmail.com"


configurar o editor de mensagens para o commit

git config --global core.editor code

Ver as configurações realizadas ou buscar qual foi a config feita

git config user.name {por exemplo, sem as chaves}

git config user.email 

Se for loko e quiser ver tudo o comando é 

git config --list


Agora tem que ser criar a pasta onde o projeto ira ficar e depois pelo terminal dentro da pasta 
digitar o comando abaixo para que o git enchergue as mudanças e atualize com o commit

git init

git status  para saber como estão meus arquivos untracked files git ainda não viu ou em portugues arquivos não monitorados

git add para monitorar arquivos.

Criar comitt que significa pegue todos os arquivos e crie uma imagem dele, uma versão

git commit-m "Add Readme.md" (importante mensagem para no log ver o que foi modificado)
apos dado esse comando o git ira criar o numero da versão do arquivo
qtas modificações ou inserções foram feitas


Log para ver quem fez as modificações

git log

git log --decorate

git log --author=”Rodrigo”

git shortlog (mostra os autores em ordem alfabética)

git shortlog -sn (mostra quem commitou e a quantidade)

git log --graph (mais detalhes)


para ver o que foi mudado dar um 
git show (e o numero da rash) ae4d09371d57e1830b929185a3c73e386f8a86d7

Para ver o que acrescentou usar o git diff(ele mosta as alterações como no print abaixo.;
Muito importante ver antes de comitar para ter certeza que não fez errado.
Tem que usar o git diff antes de add
git diff


git diff --name-only(ver so o nome do arquivo e não todos os log)



git commit -am “<file arquivo”
Esse git é para quando já exites o arquivo não é a primeira vez que se commita.




O git para desfazer a ultima inserção é o git checkout.

git checkout <file name>

*so funciona se ainda não add

quando vc já add antes de commitar tem que ser o 

git reset HEAD <file name> 

Ele vai tirar o último ponteiro por isso o HEAD, nÃO VAI APAGAR O QUE VC FEZ MAS VAI SAIR DA AREA DE COMITAR E VOLTAR PARA O MODIFIED ONDE VC PODE APAGAR 
COM CHECKOUT OU ENTRAR E APAGAR O QUE FEZ.



Se vc fez algo errado e quiser voltar o commit, pode-se usar o git reset que tem o soft apaga a ultima coisa e deixa no jeito de commitar de novo,
 o mixed que volta para o modified fora do stange e o hard vai ignorar tudo que foi feito no commit e apagar tudo é o mais bruto.
 TEM QUE ESCOLHER O COMITE ANTERIOR PARA CORRIGIR O QUE SE QUER.
Observação: usar o git reset --hard somente se ainda não subiu em um repositório remoto onde há mais pessoas trabalhando, pois pode gerar muita confusão.


git reset --soft
git reset --mixed
git reset --hard

