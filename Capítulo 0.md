# 0. Introdução

## Bla bla bla inicial

C é uma linguagem de programação de uso geral. É usada há mais de 50 anos para produzir programas que necessitam maior proximidade de recursos de baixo nível, como o processador, a memória e outros dispositivos. Assim, C é largamente utilizado no desenvolvimento do núcleo (kernel) de sistemas operacionais, drivers e é suportado por arquiteturas que vão de microcontroladores a supercomputadores.

A linguagem C é
* imperativa, ou seja, executa comandos que instruem a alteração do estado do programa;
* procedural, ou seja, executa passos em sequência que podem ser reaproveitados; e
* estruturada, ou seja, utiliza blocos de controle de fluxo condicionais e de repetição, além de permitir a estruturação de dados em blocos.

A classificação do nível de C é controversa. C pode ser considerada de alto nível pois utiliza mnemônicos da linguagem natural, mas muitos a consideram de médio nível por causa do seu poder no manejo de tarefas de baixo nível, incluindo o manejo de memória.

Um programa escrito na linguagem C deve ser compilado para o sistema em que se deseja executá-lo. Em linhas gerais, um compilador de C transforma o código-fonte do programa em um arquivo executável do sistema operacional (o compilador faz muito mais do que isso, mas deixo isso para outra hora =)).

## Configurando o ambiente

Para este tutorial, não utilizarei nenhuma IDE (exemplos: Visual Studio, Code::Blocks, Dev-C++) pois o foco deste tutorial é ensinar a linguagem, é desenvolver o código.

Basta possuir um PC com os sistemas Windows ou Linux, alé, de um compilador e um editor de texto.

O compilador que utilizarei será o GCC.

Não tenho preferências por editores de texto, mas recomendo que se use um que possua realçador de sintaxe. As opções para Linux são várias, já que o próprio Linux é, ele próprio, um grande IDE. Para Windows, boas opções são o Notepad++ e o Visual Studio Code (não confunda com o Visual Studio - sem o Code!).

### Instalando o GCC no Windows

Se você está no Linux, pode pular essa seção.

### Instalando o GCC no Linux

Se você está no Windows, pode pular essa seção.

O GCC normalmente já vem instalado por padrão nas distribuições Linux mais populares. Caso ele esteja instalado, ao tentar executar o comando `gcc` no terminal, o sistema responderá que nenhum arquivo foi fornecido ao compilador, ou ainda, a saída do compilador será `gcc: no input files`. Caso ele não esteja instalado, o sistema acusará que o comando não foi encontrado, e, para instalá-lo, as instruções dependerão do tipo de gerenciador de pacotes é usado no sistema. Detalharei, aqui, como proceder à instalação do GCC com o DNF e com o APT, apesar deles não serem os únicos gerenciadores de pacotes que existem por aí.

#### Instalando os pacotes do GCC via YUM-DNF

Rode, inicialmente, o comando `dnf upgrade` para atualizar os pacotes do seu sistema. Em seguida, para instalar o GCC, rode o comando
```
dnf install gcc-g++
```
Note que esses comandos podem exigir privilégios de super-usuário. Considere usar esses comandos com a diretriz `sudo`.

#### Instalando os pacotes do GCC via APT

Rode, inicialmente, o comando `apt update` para atualizar a lista de pacotes disponíveis. Em seguida, execute o comando `apt upgrade` para atualizar os pacotes do sistema. Finalmente, instale o GCC com o comando
```
apt install gcc
```
Note que esses comandos podem exigir privilégios de super-usuário. Considere usar esses comandos com a diretriz `sudo`.

