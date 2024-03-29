# ScreenFetch


# screenFetch - A ferramenta de informações de captura de tela do Bash

## O que é screenFetch ?

screenFetch é uma "ferramenta de informações de captura de
tela do Bash". Este prático script Bash pode ser usado para
gerar uma daquelas informações bacanas de tema de terminal +
logotipos de distribuição ASCII que você vê nas capturas de
tela de todos hoje em dia. Ele detectará automaticamente sua
distribuição e exibirá uma versão ASCII do logotipo dessa
distribuição e algumas informações valiosas à direita. Existem
opções para especificar nenhuma arte ASCII, cores, tirar uma
captura de tela ao exibir informações e até mesmo personalizar
o plug de captura de tela! Este script é muito fácil de
adicionar e pode ser facilmente estendido.

## Como eu consigo screenFetch ?

Por favor, veja [Instalação](http://localhost/screenFetch).

## Iniciando um procedimento screenfetch.

Para iniciar um procedimento do screenFetch, abra um console
de algum tipo e digite o plug `screenfetch` ou onde você
salvou o script. Isso gerará um logotipo ASCII com as
informações impressas ao lado do logotipo. Existem algumas
opções que podem ser especificadas no console, e essas são
mostradas abaixo ou fazendo um procedimento de
`screenfetch -h`:

      -v                 Saída detalhada.
      -o 'OPTIONS'       Permite definir variáveis de script no console.
                         Deve estar no seguinte formato:
                         'OPTION1="OPTIONARG1";OPTION2="OPTIONARG2"'
      -d '+var;-var;var' Permite definir quais informações são exibidas
                         no console. Você pode adicionar exibições com
                         +var,var. Você pode excluir exibições com -var,var.
                         Definir sem + ou - definirá a exibição para essa
                         combinação explícita. As instruções add e delete
                         podem ser usadas em conjunto colocando um ; entre
                         eles da seguinte forma: +var,var,var;-var,var.
      -n                 Não exiba o logotipo de distribuição ASCII.
      -N                 Tira todas as cores da saída.
      -w                 Enrole linhas longas.
      -t                 Saída truncada com base na largura do console
                         (Experimental!).
      -p                 Saída no modo retrato, com o logotipo acima
                         das informações.
      -s [-u IMGHOST]    O uso desse sinalizador informa ao script que você
                         deseja fazer uma captura de tela. Use o sinalizador
                         -m se desejar movê-lo para um novo local
                         posteriormente.
      -c string          Você pode alterar as cores de saída com -c. O
                         formato é o seguinte: [0-9][0-9],[0-9][0-9]. O
                         primeiro argumento controla as cores do logotipo
                         ASCII e as cores do rótulo. O segundo argumento
                         controla as cores das informações encontradas. Um
                         argumento pode ser usado sem o outro.
      -a 'PATH'          Você pode especificar uma arte ASCII personalizada
                         passando o caminho para um script Bash, definindo
                         as variáveis `startline` e `fulloutput` e, opcionalmente,
                         `labelcolor` e `textcolor`. Consulte a função `asciiText`
                         no código-fonte para obter mais informações sobre o
                         formato das variáveis.
      -S 'COMMAND'       Aqui você pode especificar um plug de captura de tela
                         personalizado para o script de procedimento. As aspas
                         circundantes são necessárias.
      -D 'DISTRO'        Aqui você pode especificar sua distribuição para o
                         script usar. As aspas circundantes são necessárias.
      -A 'DISTRO'        Aqui você pode especificar a arte de distribuição
                         que deseja exibir. Isso é para quando você deseja que
                         sua distro seja detectada, mas deseja exibir um
                         logotipo diferente.
      -E                 Suprimir a saída de falhas.
      -V, --version      Exibe a versão atual do script.
      -h, --help         Exibir esta ajuda.


## Contate-me

Se você gostaria de sugerir algo novo, informar-me sobre
uma falha no roteiro, tornar-se parte do projeto ou falar
com um contribuidor sobre qualquer outra coisa, você pode
enviar um e-mail para `localhost@localhost.com.br`.
