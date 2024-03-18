# SistemasOperacionais
Isabella de Castro Jorge - RA 10409762
Guilherme Garcia LIma - RA 10409637

1)Rode o programa anterior para valores grandes de n. As mensagens sempre estar˜ao ordenadas pelo valor de i?
---> Aparentemente sim. Testamos com o valor de 100.000 e as mensagens ainda apreciam ordenadas pelo o i.

2) O que acontece se o programa anterior escreve-se as mensagens para sys.stdout, usando print, ao inves de para sys.stderr?
---> (sys.stderr) para (sys.stdout, usando print)
---> Ao executarmos o código com as devidas modificações, podemos observar que não houve mudança no funcionamento do programa ao criar processos filho, como exemplificado abaixo:

Filho 0: PID = 4114, PPID = 4113
Pai: PID = 4113, PPID = 4072
Filho 1: PID = 4115, PPID = 4113
Pai: PID = 4113, PPID = 4072
Filho 2: PID = 4116, PPID = 4113
Pai: PID = 4113, PPID = 4072
Filho 3: PID = 4117, PPID = 4113
Pai: PID = 4113, PPID = 4072
Filho 4: PID = 4118, PPID = 4113

--> Com a modificação, o que muda é o local de exibição das mensagens, que passam a ser exibidas na saída padrão do programa.
