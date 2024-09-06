

O que é SO? 

  

Um sistema que abstrai a informação complexa que o hardware utiliza para se comunicar.

Ela é apresentada ao usuário como um máquina estendida ou uma máquina virtual, que é mais fácil de interagir e programar.

* Um SO atua como intermediário entre hardware e usuário
* SO - Um gerenciador de recursos: processadores, memórias, discos, dispositivos de E/S
* SOs mainframe(computador de alto desempenho) são projetados para otimizar a utilização do hardware
*  Divisão de um Sistema de computação:

-Hardware

-SO

-Programas aplicativos

-Usuários
- Sistema de computadores: é composto por hardware, software e dados. O SO fornece os meios para utilização apropriada desses recursos durante a operação do sistema de computação.
CPU ->Unidade Central de Processamento (Processador)

##Funcionamento dos SOs
- Processos: Um programa que está em execução 

* Todo e qualquer processo, compete por recursos (da CPU) e interage com outros processos (está sempre solicitação recursos da máquina )
  
- Estados de um Processo
    ![[Pasted image 20240905200727.png]]

Executando (usando a CPU para executar instruções do programa);

Bloqueado/ Em espera (aguardando pela ocorrência de algum evento externo);

Ativo/Pronto (aguardando apenas CPU para executar ).

  

O SO GERENCIA OS PROCESSOS ATRAVÉS DE SYSTEM CALLS (CHAMA DE SISTEMAS ) é a ocorrência de uma tarefa que deseja ser realizada

* Shell e System Calls


Shell -> Interpretador de comandos: Um processo que faz uma interface do usuário com o Sistema Operacional, pode ser tanto através de linhas de comando GLI (Terminal), quanto por uma interface gráfica(GUI) [Ele é um programa, nao um aplicativo]

(GUI) - Graphical User interface - interface gráfica de usuário
(GLI) - Command line interface  - Interface de linha de comando


* System Calls -> (Chamada de Sistemas) Oferece uma interface de comunicação entre o SO e os programas e aplicativos

![[Pasted image 20240905201517.png]]


Duvida, entao se eu digitar linhas de comando em um terminal, para abrir o fire fox, eu estou fazendo uma System call ? 

R; Sim, o shell faz uma System Call, requisitando do Kernel que inicie o FireFox


Resumindo: Uma system call é uma interface que o SO fornece para que programas de interface de usuário (com o shell) possa fazer requisições ao hardware e a outros processos


* Sistemas multusuário e multarefa 

-> multiusuário: Um SO multiusuário permite acessos simultâneo ao computador, onde cada usuário tem seu ambiente de trabalho isolado (cada conta tem seu ambiente próprio)

-> multitarefa - O SO alterna entre cada tarefa (ou processo), dando a impressão que todas estão sendo feitas ao mesmo tempo. Ele tem apenas uma CPU, que deve dar conta de todos esse processos. [possui apenas uma CPU => multiprogramação != Multiprocessamento ]


-> Multiprogramação: Permite a utilização de vários programas, porem o atendimento deles é feita por apenas uma CPU. E tudo isso é feito de maneira alternada, dando a impressão que tudo está funcionando simultaneamente.

	*Systemas monoprogramaveis: Como era feito antigamente, apenas um programa executando por vez. Execução funcionando instrução-a-instrução, menos eficiente.

-> Multiprocessamento: Projetada para aproveitar a presença de multprocessadores (CPUs)
em apenas um computador. Ele permite a execução concorrente de vários processos em diferentes CPUs
