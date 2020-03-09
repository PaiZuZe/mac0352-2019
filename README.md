# Redes de Computadores e Sistemas Distribuídos

Esse repositório guarda os 4 exercícios programas (EPs) relazidos no curso de graduação MAC0352 Redes de Computadores e Sistemas Distribuídos do IME-USP. Todos os projetos forem feitos por [Victor Gramgulia](https://github.com/PaiZuZe) e [Luiz Girotto](https://github.com/LuizGyro).

## EP1

Nesse projeto foi nescessário implementar algumas caractériscas de um servidor FTP seguindo a [RFC 959](https://tools.ietf.org/html/rfc959).

Era necssário escrever o servidor em C/C++, que funcionasse em GNU/Linux e deveria ser possível se conecetar com o servidor através do cliente ftp presente no GNU/Linux.


## EP2

Nesse projeto criamos um programa que ordena um arquivo com vários números usando todos os computadores disponiveis da rede local.

Para realizar essa tarefa dividimos os clientes/processos em 3 classes, o Imortal, o lider e os trabalhadores. Uma das caractêristicas do projeto é que seu protocolo deveria ser capas de lidar com clientes entrando e saindo da rede. O Imortal representa o cliente que começou o trabalho e que sempre ira se encontrar na rede (por isso o nome), seu trabalho é receber partes do arquivo já ordenados e os juntalos. O Lider ira distribuir o trabalho restante para os trabalhadores. E os trabalhadores devem ordenar pedaços do arquivo e envialos para o Imortal. Só existe um processos Imortal e um processo Lider.

Foi usado uma mistura de processos do Linux e POSIX threads para realizar a distinção de Imortal, Lider e Trabalhador, além dos encarreagados de enviar e receber dados.

## EP3

Essa tarefa se resumio em seguir um tutorial de [Open Flow](https://github.com/mininet/openflow-tutorial/wiki) para que os alunos entrarem em contato com Redes Definidas por Software (SDN) e o protocolo Open Flow.

## EP4

Nesta tarefa os alunos deveriam procurar alguma vulnerabilidade de rede descoberta após 2016 e que já tenha sido consertada. Os alunos então deveriam aprentar a vulnerabilidade escolhida, explicando o ponto de falha e o conserto feito, e também demontrar a falha sendo usada assim como mostrar que o patch consertava a falha.

Para essa apresentação exploramos o CVE-2018-1000224 que é uma falha na engine de jogos open source Godot.