
### E o que é o GitHub?

Se você vai utilizar Git, é necessário armazenar seu repositório em algum lugar. Existem duas formas de se fazer isso, **offline**, no seu próprio computador, ou online, em alguma plataforma como [GitHub] ou [BitBucket].

#### Como funciona a comunicação entre o repositório local e remoto

Podemos separar o *workflow* do Git em quatro partes. 
1. Workspace: é referente ao seu espaço de trabalho onde você faz as mudanças necessárias no seu código.
2. Staging: essa parte refere ao momento onde você salva o seu trabalho realizado, porém, não cria um novo *commit* no seu projeto.
3. Repositório local: neste momento, temos a criação de um novo *commit* que ativa o gerenciamento de versões do repositório.
4. Repositório remoto: essa parte se refere ao repositório no qual o seu repositório local se espelha, envia e recebe mudanças. Geralmente está em um sistema em núvem como o GitHub ou o BitBucket.

A imagem abaixo representa a comunicação e alguns dos comandos mais utilizados no Git.

![GitWorkflow](https://blog.isquaredsoftware.com/images/2021-01-career-advice-git-usage/git-staging-workflow.png)

#### Primeiro uso: configurando o ambiente

Primeiramente, é necessário possuir o Git instalado no seu computador e uma conta no [GitHub]. Você pode baixar o Git no [site oficial], basta selecionar o seu sistema operacional e seguir o guia de instalação, caso não queira realizar a instalação do programa no seu computador, também é possível baixar uma versão portátil.

Depois de instalar o Git, é necessário configurar o seu nome e e-mail que serão exibidos em seus *commits*, para isso é só digitar no terminal, ou seja, no executável **Git bash**, os comandos abaixo:

```sh
$ git config --global user.name "[seu-nome]"
$ git config --global user.email "[seu-email@email.com]"
```

Caso queira verificar as configurações do seu Git local, execute o comando abaixo:

```sh
$ git config --list
```

### Fluxo de trabalho 1

Geralmente, no fluxo de trabalho com Git e GitHub é realizado um `clone` de um determinado repositório remoto compartilhado com vários desenvolvedores, ou seja, copiamos todo o repositório remoto escolhido no nosso repositório local onde podemos desenvolver com a última versão dos códigos e não atrapalhamos o desenvolvimento de nenhum outro desenvolvedor do projeto.

Após fazer o `clone` para a nossa máquina local, podemos realizar alterações, e por fim, podemos fazer o envio dessas mudanças de volta para o nosso repositório remoto.

#### Git Clone

Vamos clonar o repositório para a sua máquina local para que você possa realizar alterações. Na página do seu repositório no GitHub, existe um botão chamado **Code**, clique nele, selecione a opção HTTPS, e depois clique no botão de copiar.





[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [GIT]: <https://git-scm.com>
   [GitHub]:<https://github.com>
   [BitBucket]:<https://bitbucket.org> 
