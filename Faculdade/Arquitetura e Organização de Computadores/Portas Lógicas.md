### O que são Portas Lógicas?

Portas Lógicas são blocos da eletrônica digital que compõem as equações básicas que formam a base dos circuitos digitais.

##### As portas lógicas mais comuns incluem:

![[Pasted image 20241018192608.png]]

- **Porta AND**: Retorna 1 apenas quando todas as suas entradas são 1.
- **Porta OR**: Retorna 1 quando pelo menos uma das suas entradas é 1.
- **Porta NOT**: Inverte o valor da entrada; retorna 0 para entrada 1 e 1 para entrada 0.
- **Porta NAND**: Retorna 0 apenas quando todas as suas entradas são 1. É a negação da porta AND.
- **Porta NOR**: Retorna 1 apenas quando todas as suas entradas são 0. É a negação da porta OR.
- **Porta XOR**: Retorna 1 quando um número ímpar de entradas é 1.
- **Porta XNOR**: Retorna 1 quando um número par de entradas é 1. É a negação da porta XOR.

### Portas Lógicas: Tabelas Verdade

As tabelas verdade são usadas para entender e descrever como as portas logicas funcionam. Elas listam as possíveis combinações de entrada e as respetivas saídas.

![[Pasted image 20241018194918.png | 350]]

#### Como funcionam as Portas Lógicas?

- **Sinais de Entrada e Saída:** Portas lógicas operam com sinais digitais, que possuem dois estados possíveis: 0 (baixo, falso) e 1 (alto, verdadeiro). Cada porta lógica recebe um ou mais desses sinais como entrada e gera um único sinal de saída com base em sua função lógica específica.
- **Operação Interna:** A operação de uma porta lógica é definida por uma regra lógica fixa. Essa regra determina como a saída é gerada a partir das entradas. 
- **Implementação Física:** As portas lógicas são implementadas fisicamente usando transistores, que atuam como interruptores eletrônicos. Em circuitos integrados (ICs), uma combinação de transístores MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistors) é usada para construir cada tipo de porta lógica. 
- **Tabela da Verdade:** Cada porta lógica pode ser descrita por uma tabela da verdade, que lista todas as combinações possíveis de entradas e a correspondente saída. 
- **Uso em Circuitos Digitais:** As portas lógicas são usadas como blocos de construção para circuitos digitais complexos. Por exemplo, somadores binários, multiplexadores, flip-flops e outros componentes digitais são construídos a partir de combinações de portas lógicas. Esses circuitos são usados em sistemas de processamento de dados, controle de dispositivos e várias outras aplicações tecnológicas.

#### Porta AND

![[Pasted image 20241018195944.png]]

#### Porta OR

![[Pasted image 20241018200416.png]]

#### Porta NOT

![[Pasted image 20241018200449.png]]

#### Porta NAND

![[Pasted image 20241018200536.png]]

#### Porta NOR

![[Pasted image 20241018200710.png]]

#### Porta XOR

![[Pasted image 20241018200848.png]]

#### Porta XNOR

![[Pasted image 20241018200912.png]]

### Atividades

1. Dado o circuito lógico abaixo, determine a expressão para S:
	
	![[Pasted image 20241018203240.png]]
	
	Resolução:
		S = (A \* B) + $\overline{C}$
	
2. Qual combinação de entradas a seguir trará nível lógico ALTO na saída do circuito dado? (fazer tabela verdade)
	
	![[Pasted image 20241018203742.png]]
	
	A=0, B=0, C=0 
	A=1, B=1, C=1 
	A=0, B=0, C=1 
	A=1, B=1, C=0
	
	Resolução:
		

| A   | B   | C   | S = (($\overline{A * B}$) + $\overline{C}$) + $\overline{B}$ |
| --- | --- | --- | ------------------------------------------------------------ |
| 0   | 0   | 0   | 1                                                            |
| 1   | 1   | 1   | 0                                                            |
| 0   | 0   | 1   | 1                                                            |
| 1   | 1   | 0   | 0                                                            |
	
3. A tabela verdade a seguir corresponde a uma função lógica com 3 entradas (X, Y e Z) e uma saída (S1).
	
|     | X   | Y   | Z   | S1                                     |
| --- | --- | --- | --- | -------------------------------------- |
| 0   | 0   | 0   | 0   |                                        |
| 1   | 0   | 0   | 1   | $\overline{A}$ \* $\overline{B}$  \* C |
| 2   | 0   | 1   | 0   |                                        |
| 3   | 0   | 1   | 1   | $\overline{A}$ \* B  \* C              |
| 4   | 1   | 0   | 0   | A \* $\overline{B}$  \* $\overline{C}$ |
| 5   | 1   | 0   | 1   | A \* $\overline{B}$  \* C              |
| 6   | 1   | 1   | 0   | A \* B  \* $\overline{C}$              |
| 7   | 1   | 1   | 1   |                                        |
	Qual é a expressão lógica mínima, na forma soma de produtos?
	1. S1 = $\overline{A}$ * C + A * $\overline{B}$ + A * $\overline{C}$ 
	2. 