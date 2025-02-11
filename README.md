# Projeto Start

# Versionamento de Código - Git GitHub

Módulo que busca nos mostrar conceito, função, comandos, integração e forma de uso das plataformas conectadas.

Aqui teremos um resumo das aulas afim de organizar o conhecimento e facilitar o aprendizado.

## Objetivos

- Conhecer as plataformas
- Instalar, Configurar e Autenticar a conexão
- Primeiros passos com Git e GitHub
- Dicas e Materiais de Apoio
- Conclusão

## Pré-Requisitos

- Computador com acesso à Internet
- Vontade de Aprender
- Fechar outras Abas

## 1 - O que é Versionamento de Código?

Versionamento de código é o registro do histórico de atualizações de um arquivo. 

Ele oferece:

- organização 
- controle
- segurança 

Gerenciando as alterações, datas, autores, e controlando as versões ao longo do tempo.

O **versionamento de código** é realizado através de Sistemas de Controle de Versão (VCS), vamos agora conhecê-los.

**Existem dois tipos principais de VCS**:

- VCS Centralizado (CVCS): Exemplo: CVS, Subversion.

O Sistema de controle de versionamento Centralizado é mais restrito, limitado, pois não permite que duas ou mais pessoas consigam trabalhar no mesmo projeto ao mesmo tempo.

- VCS Distribuído (DVCS): Exemplo: **Git**, Mercurial.

Um Sistema de Controle de Versão Distribuído (DVCS) oferece diversas vantagens, incluindo:

- Cada clone funciona como um backup.
- Possibilidade de trabalhar sem conexão à rede.
- Fluxo de trabalho flexível.

*Ao contrário dos Sistemas de Controle de Versão Centralizados (CVCS)*, o DVCS clona o repositório completo, incluindo o histórico de versões.

tornando-se assim a opção mais recomendada, a qual utilizaremos no curso.  #GIT e #GitHub.

## O que é Git? 
O Git é um sistema de controle de versão distribuído, gratuito e open source, podendo ser acessado por [aqui](https://git-scm.com/)


# O que é GitHub?
O GitHub é uma plataforma de hospedagem de código para controle de versão com Git e colaboração, e pode ser acessado por [aqui](https://github.com/)

## Breve Histórico sobre o Git

O Git foi criado como uma ferramenta de controle de versão após um conflito da comunidade com o BitKeeper.
Aqui está um breve histórico do Git:

**2002**: O projeto do núcleo (kernel) do Linux, que é open source, começou a utilizar o BitKeeper, um DVCS proprietário.

**2005**: Após conflitos com a comunidade, o BitKeeper rescindiu a licença gratuita, o que levou **Linus Torvalds** e sua equipe a desenvolverem o Git.

## Fluxo de Trabalho no Git

O fluxo de trabalho básico com Git envolve **clonar um repositório, gravar alterações e sincronizar entre os repositórios local e remoto**. 

Alguns comandos que fazem parte desse fluxo são:

- git clone, 
- git commit, 
- git pull e 
- git push
-  git init

# Resumindo o fluxo básico e comandos do GIT:

*   `git clone` tem a função de Clonar

Usa-se git clone para clonar um repositório Git existente para um diretório local.

*   `git commit` tem a função de gravar. 

Commit: O comando git commit grava as alterações no repositório local.

*   `git pull` tem a função de buscar e mescar as alterações 

Pull: O comando git pull busca e mescla as alterações do repositório remoto para o repositório local.

*   `git push` tem a função de enviar Alterações

Push: O comando git push envia as alterações do repositório local para o repositório remoto.

Além desses comandos, também temos:

Além dos comandos `git clone`, `git commit`, `git pull` e `git push` que já foram mencionados, o material de apoio cita outros comandos Git, juntamente com explicações sobre suas funcionalidades:

*   `git init`: Inicializa um repositório Git no diretório escolhido.
*   `git remote add origin`: Conecta o repositório local com o repositório remoto.
*   `git add`: Adiciona o conteúdo que deseja inserir no *commit*.
*   `git commit -m "message"`: Cria um *commit* e adiciona uma mensagem descritiva.
*   `git commit --amend`: Usado para desfazer alterações no repositório local.
    *   `git commit --amend –m"nova mensagem"`: Altera a mensagem do último *commit* sem abrir o editor.

*   `git reset`: Desfaz um *commit*.

    *   `git reset --mixed`:  você tem um desenho (seu código) e o mostrou para alguns amigos (salvou no Git). O --mixed é como se você voltasse para a versão anterior do desenho que mostrou aos amigos, mas ainda tivesse o desenho novo na mão, pronto para ser revisado.
    Você mostrou o desenho: Significa que você fez um commit, ou seja, salvou as alterações do seu código no Git. Voltou para a versão anterior:

    O --mixed faz com que o Git volte para o commit anterior, como se você estivesse desfazendo o último commit.

    Ainda tem o desenho novo na mão: As alterações que você fez no seu código continuam no seu computador, prontas para serem revisadas e commitadas novamente.
    *   `git reset --hard`: O --hard é como se você pegasse a borracha e apagasse completamente o desenho novo, voltando para a versão anterior que mostrou aos amigos.

    *   `git reset --soft`: O --soft é como se você voltasse para a versão anterior do desenho que mostrou aos amigos, mas ainda tivesse o desenho novo na mão, pronto para ser revisado e mostrado novamente. A diferença é que, com o --soft, seus amigos nem sabem que você mudou o desenho!
    Você fez alterações sem mostrar: Você fez modificações no seu código, mas não as commitou, ou seja, não as mostrou para o Git. 
    
    Voltou para a versão anterior: O --soft faz com que o Git volte para o commit anterior, mas como você não tinha mostrado as alterações, é como se nada tivesse mudado. 
    
    Seu amigo nem sabe que você mudou: Seu amigo, que está trabalhando no mesmo projeto, não verá as alterações que você fez até que você as commite e as envie para o repositório compartilhado.

*   `git branch`: Exibe as *branches*.
*   `git checkout -b nova-branch`: Troca de *branch* e cria uma nova.
*   `git branch –d nome-da-branch`: Deleta uma *branch*.
*   `git branch -v`: Apresenta o último *commit* de cada *branch*. 
-  `git config`, usado para configurar o Git, como, por exemplo, para configurar o nome de usuário e e-mail.


## Qual a Diferença entre Git e github

*Explicado para que até um leigo consiga entender (eu =D)*

### Git O que é?

Imagine o Git como um caderno de anotações inteligente que registra cada alteração feita em um documento (seu código). Ele permite que você:

**Volte no tempo**
e veja como o documento estava em qualquer momento anterior.

**Compare versões**
para identificar as mudanças feitas ao longo do tempo.

**Trabalhe em várias versões**
do documento simultaneamente, sem bagunçar a versão principal.

**Colabore com outras pessoas**
compartilhando as anotações e permitindo que cada um contribua com suas próprias anotações.

### GitHub O que é?

**O que é**
Pense no GitHub como uma plataforma online onde você pode guardar e compartilhar seus cadernos de anotações inteligentes (seus projetos com Git). Ele oferece:

**Um local centralizado**
para armazenar seus projetos e torná-los acessíveis de qualquer lugar.

**Ferramentas para colaborar**
com outras pessoas em projetos, como discussões,Pull Requests e gerenciamento de tarefas.

**Uma interface amigável**
para visualizar o histórico de alterações, comparar versões e gerenciar seus projetos.

**Integrações com outras ferramentas**
como editores de código e plataformas de desenvolvimento.

**Em resumo**

- Git
é o sistema que permite controlar as versões do seu código e colaborar com outras pessoas.

- GitHub
é a plataforma online que hospeda seus projetos com Git e oferece ferramentas para gerenciá-los e colaborar.
