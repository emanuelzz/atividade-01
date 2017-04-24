# atividade-01

# Multiprogramação 

Periodicamente o sistema operacional decide se a execução de um processo deve ser interrompida e a execução de um outro processo deve ser iniciada--pela razão do primeiro já ter tido mais do que a sua fatia de tempo de CPU. Em um sistema de multiprogramação a CPU fica se alternando entre a execução de vários processos, cada um por dezenas ou centenas de milisegundos.

Um processo pode estar em um dos seguintes estados:

- Running: usando a CPU naquele instante;
- Ready: pronto para ser executado, temporariamente parado para que outro processo possa ser executado; e
- Blocked: impossibilitado de ser executado até que algum evento externo ocorra.

Em um sistema de multiprogramação temos frequentemente a situação onde vários processos estão prontos para serem executados. Quando mais de um processo está ready, o sistema operacional deve decider qual processo deve ser executado primeiro. A parte do sistema operacional que toma esta decisão é chamada de scheduler, e o algoritmo que é usado é chamado de scheduler algorithm. A cada interrupçao do relógio o sistema operacional toma o controle e decide se o processo que está sendo executado deve continuar a ser executado ou deve ser suspenso para que outro processo passe a ser executado. A estratégia que permite que um processo que está sendo executado seja suspenso temporariamente é chamada de preemptive schedule.

Existem scheduling algoritms que assumem que todos os processos são iguais. Entretanto, existem muitas pessoas que possuem e administram centros de computação que discordam disto. Por exemplo, em um centro de computação de uma universidade pode ser dada a mais alta prioridade aos processos de diretores, depois aos de professores, depois aos de secretarias, depois aos de porteiros, ...e finalmente aos de alunos. Isto é chamado de um priority schedule (alguns podem chamar isto de injustiça).

Para evitar que processos que têm alta prioridade fiquem sendo executados indefinidamente o scheduler pode baixar a prioridade do processo que esta sendo executado a cada interrupção do relógio.

Através da execução “simultânea” de vários programas, a multiprogramação torna mais eficiente o aproveitamento dos recursos do computador, tais como: tempo do processador, espaço de memória, etc. Na realidade a execução é feita de forma concorrente (máquinas monoprocessadas). Em um sistema multiprogramado vários programas são mantidos na memória ao mesmo tempo. 

# Programação concorrente

 É um paradigma de programação para a construção de programas de computador que fazem uso da execução concorrente de várias tarefas computacionais interativas, que podem ser implementadas como programas separados ou como um conjunto de threads criadas por um único programa.
 
  A programação concorrente foi usada inicialmente na construção de sistemas operacionais. Atualmente, ela é usada para desenvolver aplicações em todas as áreas da computação. Este tipo de programação tornou-se ainda mais importante com o advento dos sistemas distribuídos e das máquinas com arquitetura paralela.
  
  Um programa concorrente pode ser visto como se tivesse vários fluxos de execução.Nele é definido o uso simultâneo de múltiplos recursos computacionais para resolver um problema. Para ser executado em diversas CPUs: O problema é quebrado em partes que podem ser executadas (resolvidas) simultaneamente – Cada uma destas partes é representada por uma série de instruções, sendo que as instruções de cada parte são executadas concorrentemente em diferentes CPUs.


referencias:

https://www.ime.usp.br/~gold/cursos/2002/mac2301/ep2/ep2/node3.html
https://www.infopedia.pt/dicionarios/lingua-portuguesa/multiprograma%C3%A7%C3%A3o
https://pt.slideshare.net/FabioMouraPereira/programao-concorrente-introduo

